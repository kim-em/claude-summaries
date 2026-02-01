---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Polynomial/Hermite
generated: 2026-02-01T20:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 2
subdirs_count: 0
---

# Hermite

## Overview

The `Hermite/` directory defines the probabilists' Hermite polynomials and establishes their fundamental properties. These orthogonal polynomials are defined recursively as `hermite (n+1) = X * hermite n - derivative (hermite n)` with integer coefficients, and the main file proves explicit coefficient formulas involving binomial coefficients and double factorials. The second file connects Hermite polynomials to analysis by showing they arise as the polynomial factor in the `n`th derivative of a Gaussian function `exp(-(x^2/2))`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines probabilists' Hermite polynomials recursively over integers; proves coefficients vanish when n+k is odd; gives explicit coefficient formula using double factorials and binomial coefficients; proves each `hermite n` is monic with degree n |
| Gaussian.lean | Proves the analytic characterization: `deriv^[n] exp(-(x^2/2)) = (-1)^n * hermite n(x) * exp(-(x^2/2))`; provides inverse formula expressing Hermite evaluation as scaled iterated derivative of Gaussian |

## Subdirectories

(none)

## Search Tags

Hermite polynomial probabilist orthogonal-polynomial Gaussian derivative recursion monic integer-polynomial double-factorial binomial-coefficient coefficient-formula exp analysis calculus iterated-derivative
