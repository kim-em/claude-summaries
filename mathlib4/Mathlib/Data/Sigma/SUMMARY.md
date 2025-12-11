---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Sigma
generated: 2025-12-11T10:45:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 4
subdirs_count: 0
---

# Sigma

## Overview

This folder provides comprehensive support for sigma types (dependent pair types) `Σ i, α i`. Sigma types are disjoint unions of type families: given `α : ι → Type*`, an element of `Σ i, α i` is a pair `⟨i, a⟩` where `i : ι` and `a : α i`. The folder covers basic operations and properties, two distinct orderings (disjoint sum order and lexicographic order), finite interval support, and parallel results for `PSigma` (the universe-polymorphic variant).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core sigma type API: decidable equality, injectivity/surjectivity of `fst`, `map` function for transforming both components, `curry`/`uncurry` for converting between functions on sigma types and dependent functions, conversion from `Prod` to `Sigma` |
| Lex.lean | Lexicographic order on sigma types: defines `Sigma.Lex r s` relating `⟨i,a⟩` and `⟨j,b⟩` when either `r i j` or `i = j` and `s i a b`; provides monotonicity, decidability, and instances for reflexivity, transitivity, symmetry, antisymmetry, trichotomy; parallel results for `PSigma.Lex` |
| Order.lean | Two order structures on sigma types: (1) disjoint sum order where `⟨i,a⟩ ≤ ⟨j,b⟩` iff `i = j` and `a ≤ b`, (2) lexicographic order (via `Σₗ i, α i` notation) where summand index is compared first; provides `Preorder`, `PartialOrder`, `LinearOrder`, bounded order instances, and density properties |
| Interval.lean | `LocallyFiniteOrder` instance for sigma types with disjoint sum order; enables finite interval operations (Icc, Ico, Ioc, Ioo) when each summand is locally finite; provides cardinality formulas for intervals |

## Subdirectories

(none)

## Search Tags

sigma dependent-pairs disjoint-union lexicographic-order locally-finite-order intervals curry uncurry PSigma type-families
