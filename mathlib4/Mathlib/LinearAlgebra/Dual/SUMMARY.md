---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Dual
generated: 2026-01-25T09:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Dual

## Overview

The `Dual/` directory formalizes dual vector spaces—the space of linear maps from a module M to its base ring R. This foundational construction includes the canonical pairing between a module and its dual, the double dual with evaluation maps, transpose operations on linear maps, dual bases and their characterization, annihilators and coannihilators of submodules with Galois correspondence, and base change properties for duals of finite free modules. The theory covers both general modules over commutative semirings and specialized results for vector spaces (nondegenerate pairings, dimension formulas, order isomorphisms between subspaces and dual annihilators).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: Module.Dual as M →ₗ[R] R, dualPairing (canonical pairing), eval (map to double dual), transpose (dualizes linear maps), dualMap for LinearMap and LinearEquiv, submodule operations (dualRestrict, dualAnnihilator with kernel property), and Galois correspondence between annihilators and coannihilators |
| Lemmas.lean | Extended dual space theory: dual of products (dualProdDualEquivDual), annihilator theorems (ker_dual_map_eq_dualAnnihilator_range, range_dual_map properties), quotient-annihilator equivalences (dualQuotEquivDualAnnihilator, quotDualCoannihilatorToDual), vector space results (dualPairing_nondegenerate, dualAnnihilator_dualCoannihilator_eq, complementary subspace preservation), and finite-dimensional order isomorphisms (orderIsoFiniteCodimDim, orderIsoFiniteDimensional between subspaces and dual subspaces) |
| Basis.lean | Basis theory for dual spaces: toDual (basis → dual map), toDualEquiv (finite basis equivalence), dualBasis (dual basis construction from finite basis), DualBases proposition (characterizing dual pairs e/ε), coord functions as dual basis elements, and proofs that dual pairs form bases in both directions |
| BaseChange.lean | Base change for duals: Dual.congr (equivalent modules have equivalent duals), baseChange (Dual R V →ₗ Dual A (A ⊗[R] V) for algebras A over R), baseChange composition law, IsBaseChange.toDual (base change respects dual structure), and IsBaseChange.dual (taking duals commutes with base change for finite free modules) |

## Subdirectories

*(none)*

## Search Tags

dual-spaces double-dual evaluation transpose annihilator coannihilator galois-correspondence dual-basis perfect-pairing nondegenerate-pairing quotient-dual base-change finite-dimensional subspace-duality order-isomorphism vector-spaces linear-maps
