---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Multilinear
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# Multilinear

## Overview

The `Multilinear/` directory contains mathlib4's formalization of multilinear maps—functions from `∀ (i : ι), M₁ i` to `M₂` that are linear in each coordinate independently. This includes the core `MultilinearMap` structure with its fundamental properties (additivity and scalar compatibility in each argument), currying operations that transform between multilinear maps in n+1 variables and linear maps into multilinear maps in n variables, and specialized constructions for working with multilinear maps on finitely-supported functions, direct sums, pi types, and tensor products. The directory establishes that multilinear maps over finitely-generated free modules are themselves finitely-generated and free, and provides basis constructions when bases are given on domain and codomain.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core multilinear map structure (`MultilinearMap R M₁ M₂`) with linearity axioms (`map_update_add'`, `map_update_smul'`), module structure by pointwise operations, fundamental properties (`map_smul_univ` for simultaneous scalar multiplication, `map_add_univ` for simultaneous addition via piecewise sums, `map_sum` for iterated sums), function application and evaluation constructions, composition operations, and domain/codomain transformations |
| Basis.lean | Multilinear maps in relation to bases: extensionality principle (`Module.Basis.ext_multilinear` proving equality when maps agree on all basis vector inputs), basis construction for spaces of multilinear maps (`Basis.multilinearMap` from finite bases on domain and codomain, yielding basis indexed by `(Π i, κ i) × ι'`), and basis element evaluation formulas (`multilinearMap_apply_apply` scaling codomain basis by product of coordinate representations) |
| Curry.lean | Currying and uncurrying operations: left currying (`curryLeft` transforms `MultilinearMap R M M₂` on `Fin n.succ` variables into `M 0 →ₗ[R] MultilinearMap R (fun i : Fin n => M i.succ) M₂`, with inverse `uncurryLeft`), right currying (`curryRight` produces multilinear map in n variables taking values in linear maps, with inverse `uncurryRight`), and linear equivalences `multilinearCurryLeftEquiv` and `multilinearCurryRightEquiv` establishing isomorphism between spaces |
| DFinsupp.lean | Interactions with dependent finitely-supported functions: extensionality for multilinear maps from DFinsupp (`dfinsupp_ext` proving equality when maps agree on generators via `lsingle`), `dfinsuppFamily` construction satisfying `dfinsuppFamily f x p = f p (fun i => x i (p i))` (bundled as multilinear map `dfinsuppFamily f` and linear map `dfinsuppFamilyₗ`), and `freeDFinsuppEquiv` establishing linear equivalence between multilinear maps over free modules and finitely-supported maps |
| DirectSum.lean | Multilinear maps from direct sums: extensionality (`directSum_ext` proving equality when maps agree on generators via `DirectSum.lof`), and `fromDirectSumEquiv` providing linear equivalence between families of multilinear maps indexed by `p : Π i, κ i` (on `M i (p i)`) and multilinear maps on `fun i => ⨁ j : κ i, M i j`, with evaluation formulas on generators and general elements |
| FiniteDimensional.lean | Multilinear maps over finite-dimensional spaces: proof that multilinear maps over finitely-generated free modules are finitely-generated and free (`Module.Finite.multilinearMap` and `Module.Free.multilinearMap` instances), using induction on arity with currying equivalences to reduce to linear map case |
| Finsupp.lean | Finsupp variant of DFinsupp constructions: `freeFinsuppEquiv` providing linear equivalence between finitely-supported maps `((Π i, κ i) × ι') →₀ R` and `MultilinearMap R (fun i => (κ i →₀ R)) (ι' →₀ R)`, with evaluation formula showing `freeFinsuppEquiv (Finsupp.single p r) x = r • Finsupp.single p.2 (∏ i, (x i) (p.1 i))` |
| Pi.lean | Interactions with (dependent) functions: extensionality for multilinear maps from pi types (`pi_ext` proving equality when maps agree on all point evaluations via `LinearMap.single`), and `piFamily` construction mapping families of multilinear maps `f p` to multilinear maps on function spaces satisfying `piFamily f x p = f p (fun i => x i (p i))`, with `piFamilyₗ` as linear map variant |
| TensorProduct.lean | Constructions relating multilinear maps and tensor products: `domCoprod` combining multilinear maps `(ι₁ → N) → N₁` and `(ι₂ → N) → N₂` into `(ι₁ ⊕ ι₂ → N) → N₁ ⊗ N₂` by coproduct on domain and tensor product on codomain, generalized `domCoprodDep` for dependent families, bundled linear map versions `domCoprod'` and `domCoprodDep'` from tensor products of multilinear map spaces, and compatibility with domain permutations |

## Subdirectories

*(None)*

## Search Tags

multilinear-maps linear-algebra modules semilinear maps basis currying tensor-products finsupp dfinsupp direct-sums pi-types finite-dimensional free-modules function-spaces domain-codomain-transformations universal-properties
