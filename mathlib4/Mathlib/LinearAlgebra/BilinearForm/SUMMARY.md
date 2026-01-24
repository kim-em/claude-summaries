---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/BilinearForm
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# BilinearForm

## Overview

The `BilinearForm/` subdirectory provides a comprehensive formalization of bilinear forms on modules, extending the general bilinear map framework to specialize in forms (bilinear maps `M × M → R`). Core theory includes basic properties (reflexivity, symmetry, alternativity, positive semidefiniteness), orthogonality (orthogonal complements, orthogonal sets, linear independence of orthogonal vectors), nondegeneracy (kernel characterization, dual space equivalences), linear adjoints and dual bases for nondegenerate forms, tensor product constructions, and dual lattices. This framework supports both general bilinear forms and important special cases (symmetric, alternating) across commutative semirings, rings, and fields.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Basic bilinear form operations: coercion from BilinMap, linearity properties (add/smul left/right, zero/neg/sub), injectivity and extensionality, flip operation (exchange arguments), restriction to submodules, and tower compatibility for scalar actions |
| Hom.lean | Relationship between bilinear forms and linear maps: conversion to linear maps (toLinHomAux₁, toLinHomFlip), composition operations (comp, compLeft, compRight with identity laws), linear equivalences (congr for argument changes, congrRight₂ for codomain changes), linMulLin constructor (product of two linear forms), basis-based equality and representation theorems, and compBilinForm for output composition |
| Properties.lean | Core properties of bilinear forms: reflexivity (IsRefl: B x y = 0 → B y x = 0), symmetry (IsSymm: B x y = B y x with polarization identity for characteristic ≠ 2), alternativity (IsAlt: B x x = 0), positive semidefiniteness (IsNonneg, IsPosSemidef for symmetric nonnegative forms), nondegeneracy (kernel triviality, toDual equivalence for finite-dimensional spaces, flip nondegeneracy), dual basis construction (satisfies B (dualBasis i) (b j) = δᵢⱼ), linear adjoints (leftAdjointOfNondegenerate with uniqueness), and basis-dependent characterizations |
| Orthogonal.lean | Orthogonality theory: pairwise orthogonality (IsOrtho: B x y = 0 with reflexive/symmetric/alternating commutativity), indexed orthogonality (iIsOrtho for families of vectors), linear independence of orthogonal families with nonzero diagonal entries, orthogonal complement construction (orthogonal N = {m \| ∀ n ∈ N, B n m = 0}), complement relationships (span_singleton_sup_orthogonal_eq_top, isCompl_span_singleton_orthogonal for non-self-orthogonal elements), finite-dimensional orthogonal complement dimension formulas (finrank_add_finrank_orthogonal, orthogonal_orthogonal equals original subspace for nondegenerate forms), and restriction nondegeneracy characterized by disjoint orthogonal complements |
| DualLattice.lean | Dual submodules with respect to bilinear forms over commutative rings and field extensions: dualSubmodule N = {x \| ∀ y ∈ N, B x y ∈ R} (dual lattice definition), natural pairing map (dualSubmoduleParing and bundled dualSubmoduleToDual), injectivity of pairing for nondegenerate forms on spanning sets, dual of lattice spanned by basis equals span of dual basis (dualSubmodule_span_of_basis), and involutive properties (dualSubmodule of dualSubmodule equals original for nondegenerate symmetric forms) |
| TensorProduct.lean | Tensor product constructions for bilinear forms: tensorDistrib operation (B₁ ⊗ B₂ on M₁ ⊗ M₂ evaluates as B₁ m₁ m₁' ⊗ B₂ m₂ m₂' for BilinMap, B₂ m₂ m₂' • B₁ m₁ m₁' for BilinForm), baseChange for scalar extension (extending bilinear form from R-module to A-module via A ⊗ᵣ M), symmetry preservation (tensor product of symmetric forms is symmetric), and tensorDistribEquiv as linear equivalence for finite free modules (evaluates as multiplication B₁ m₁ m₁' * B₂ m₂ m₂' over commutative rings) |

## Subdirectories

(No subdirectories)

## Search Tags

bilinear-forms orthogonality reflexive symmetric alternating nondegenerate positive-semidefinite dual-basis linear-adjoints orthogonal-complement tensor-products dual-lattice basechange finite-dimensional kernel polarization-identity basis-representation
