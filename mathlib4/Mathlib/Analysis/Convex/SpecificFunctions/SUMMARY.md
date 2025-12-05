---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Convex/SpecificFunctions
generated: 2025-12-05T08:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# SpecificFunctions

## Overview

This directory contains proofs of convexity and concavity properties for specific mathematical functions. It covers exponential, logarithm, power functions (integer, natural, and real exponents), trigonometric functions (sin, cos), and special combinations like sqrt·log. The proofs are deliberately kept elementary where possible to minimize dependencies, though some results use second derivative tests.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Elementary proofs of convexity/concavity for exp, log, and rpow functions; strict convexity of exp and x^p for p>1, strict concavity of log, Bernoulli's inequality for real exponents; includes helper lemma for exp·cosh·sinh |
| Deriv.lean | Convexity proofs using derivatives and second derivatives; strict convexity of x^n (n≥2) and x^m (integer m≠0,1), strict concavity of sin on [0,π] and cos on [-π/2,π/2], strict concavity of sqrt·log on (1,∞) |
| Pow.lean | Concavity of x^p for p∈[0,1]; strict concavity for p∈(0,1); covers both nonnegative reals (NNReal) and reals on [0,∞); special case for sqrt; uses elementary proofs via order isomorphisms rather than calculus |

## Subdirectories

*(No subdirectories)*

## Search Tags

convexity concavity specific-functions exponential logarithm power-functions rpow bernoulli-inequality trigonometric sin cos sqrt derivatives elementary-proofs strict-convex strict-concave nnreal
