---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/DiophantineApproximation
generated: 2026-01-25T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# DiophantineApproximation

## Overview

This directory contains formalizations of classical Diophantine approximation theory, centered on two landmark theorems: Dirichlet's approximation theorem and Legendre's theorem on rational approximation. Dirichlet's theorem establishes that irrational numbers admit infinitely many "good" rational approximations (within 1/q.den² of the true value), while Legendre's theorem characterizes when a rational approximation is a convergent of the continued fraction expansion. The implementation uses the pigeonhole principle for Dirichlet's proof and provides two parallel formulations of Legendre's theorem using both a simple recursive convergent definition and the general continued fraction library.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core Diophantine approximation theory: Dirichlet's approximation theorem (three variants), proof that irrationals have infinitely many good approximations, Legendre's theorem on rational approximation using simple recursive convergents |
| ContinuedFractions.lean | Alternative formulation of Legendre's theorem using `GenContFract.convs` instead of the simple `Real.convergent` definition, proves equivalence between the two approaches |

## Subdirectories

(No subdirectories)

## Search Tags

diophantine-approximation dirichlet-approximation-theorem legendre-theorem continued-fractions convergents rational-approximation irrational-numbers pigeonhole-principle
