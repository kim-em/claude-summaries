---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function/StronglyMeasurable
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# StronglyMeasurable

## Overview

This directory contains the foundational theory of strongly measurable and finitely strongly measurable functions, which form the basis for Bochner integration in measure theory. A function is strongly measurable if it can be approximated by a sequence of simple functions, and finitely strongly measurable if those approximating simple functions have supports with finite measure. The directory includes both the basic definitions and API, almost everywhere variants, connections to Lp spaces, and specialized results for inner product spaces and ENNReal-valued functions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `StronglyMeasurable` and `FinStronglyMeasurable` functions, basic API including closure under algebraic operations, composition with continuous functions, and relationships with measurability in second countable spaces |
| AEStronglyMeasurable.lean | Almost everywhere strongly measurable functions: defines `AEStronglyMeasurable` and `AEFinStronglyMeasurable` (functions equal almost everywhere to strongly measurable functions), includes the key result `AEFinStronglyMeasurable.exists_set_sigmaFinite` showing such functions are supported on sigma-finite sets |
| Lemmas.lean | Additional lemmas and results for strongly measurable functions, including results about measure-preserving maps, continuous linear maps, normed spaces, and withDensity measures |
| Lp.lean | Connection between Lp spaces and finite strong measurability: proves that functions in Lp (for 0 < p < ∞) are finitely strongly measurable, key theorems `MemLp.aefinStronglyMeasurable` and `Lp.finStronglyMeasurable` |
| Inner.lean | Strong measurability of inner products: proves inner products of strongly measurable functions are strongly measurable, includes real and imaginary parts for RCLike-valued functions |
| ENNReal.lean | Finite strong measurability for ENNReal-valued functions: shows measurable functions with finite Lebesgue integral can be approximated by simple functions with finite support measure |

## Subdirectories

*(No subdirectories)*

## Search Tags

strongly-measurable finitely-strongly-measurable ae-strongly-measurable simple-function-approximation bochner-integral measure-theory sigma-finite lp-space inner-product measurable-function ennreal-valued ae-equality finite-support
