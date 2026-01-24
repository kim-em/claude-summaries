---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Alternating
generated: 2026-01-25T08:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 3
subdirs_count: 1
---

# Alternating

## Overview

The `Alternating/` directory provides the theory of alternating multilinear maps - multilinear maps that vanish when two arguments are equal and change sign when two arguments are swapped. The core type `AlternatingMap R M N ι` represents R-linear alternating maps from `ι → M` to `N`, extending the multilinear map framework with alternating properties. The directory includes basic structural theory, currying operations for splitting off the first variable, and the exterior product construction (domCoprod) that combines two alternating maps into a tensor product via signed sums over permutation equivalence classes.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `AlternatingMap` as multilinear maps with `map_eq_zero_of_eq'` property, fundamental lemmas (`map_swap`, `map_perm` relating to permutation signs), algebraic structures (AddCommMonoid, AddCommGroup, Module), domain permutation operations (`domDomCongr`), and alternatization construction (converting multilinear maps to alternating maps) |
| Curry.lean | Currying operations for alternating maps: `curryLeft` splits n+1 variable alternating map into linear map M →ₗ[R] (M [⋀^Fin n]→ₗ[R] N), with homomorphism properties (curryLeft_add, curryLeft_smul), composition lemmas, and `curryLeft_same` showing double currying with same element gives zero |
| DomCoprod.lean | Exterior product of alternating maps: `domCoprod` combines `Mᵢ [⋀^ιa]→ₗ[R'] N₁` and `Mᵢ [⋀^ιb]→ₗ[R'] N₂` into `Mᵢ [⋀^ιa ⊕ ιb]→ₗ[R'] (N₁ ⊗[R'] N₂)` via signed sum over permutation quotient `ModSumCongr`, bundled version `domCoprod'` as linear map on tensor products, and relationship to alternatization of multilinear domCoprod |

## Subdirectories

- [x] `Uncurry/` - Uncurrying operations (inverse of currying)

## Search Tags

alternating-maps multilinear-maps exterior-product wedge-product domcoprod curry currying permutations sign antisymmetric tensor-products alternatization linear-algebra
