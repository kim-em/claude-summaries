---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/TensorProduct
generated: 2026-01-25T23:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 16
subdirs_count: 1
---

# TensorProduct

## Overview

The `TensorProduct/` directory contains mathlib4's comprehensive formalization of tensor products of modules and algebras over commutative semirings. Core functionality includes the fundamental construction `M ⊗[R] N` via quotient of free additive monoid with bilinearity relations, universal property (lift, curry/uncurry), structural isomorphisms (associator, left/right identity, commutativity), and basis theory showing tensor products of free modules are free. The directory covers both abstract theory (right-exactness properties, interaction with quotients and direct limits, vanishing criteria) and concrete constructions (products, pi-types, submodules/subalgebras), plus specialized topics including tower structures for algebra extensions, graded tensor products with signed commutativity, and finiteness results for finite generation preservation.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core tensor product construction: defines `TensorProduct R M N` as quotient by bilinearity equivalence relations (zero preservation, additivity, scalar interchange), canonical bilinear map `mk`, universal property via `lift`, basic operations (map, comm, add_comm_monoid/module instances), and notation `M ⊗[R] N` and `m ⊗ₜ[R] n` |
| Associator.lean | Associativity and unit isomorphisms: left identity `lid : R ⊗[R] M ≃ₗ[R] M`, right identity `rid : M ⊗[R] R ≃ₗ[R] M`, associator `assoc : (M ⊗ N) ⊗ P ≃ₗ (M ⊗ (N ⊗ P))`, and compatibility with commutativity |
| Basis.lean | Basis theory for tensor products: `tensorProduct` constructs basis of `M ⊗[R] N` from bases of `M` and `N` (indexed by product), `baseChange` lifts basis under base change, equivalences with finsupp for decomposing elements, proving tensor products of free modules are free |
| Tower.lean | Algebra tower structures: when `M` is both `R`-module and `A`-module with `Algebra R A`, defines `AlgebraTensorModule` morphisms preserving `A`-action (curry/uncurry/lift for `A`-linear maps, map/congr for functoriality, associators and commutators for algebra towers), and base change `A ⊗ f` |
| RightExactness.lean | Right-exactness properties: proves `rTensor` and `lTensor` preserve surjectivity and exactness (`rTensor_exact`, `lTensor_exact` for short exact sequences), computes kernels (`map_ker` for tensor products of exact sequences), and algebra specializations (`Algebra.TensorProduct.ker_map`) - foundational for flatness criteria |
| Submodule.lean | Submodule tensor products: natural map `mulMap : M ⊗[R] N →ₗ[R] S` for submodules in algebra (image is `M * N`), surjective quotient map `mulMap'`, and identity isomorphisms `lTensorOne`/`rTensorOne` for tensoring with scalar image generalizing `lid`/`rid` |
| Subalgebra.lean | Subalgebra tensor products: algebra homomorphism `mulMap : A ⊗[R] B →ₐ[R] S` for subalgebras (image is `A ⊔ B`), surjective `mulMap'`, and algebra isomorphisms `lTensorBot`/`rTensorBot` for tensoring with scalar image (subalgebra versions of `Submodule` results) |
| Quotient.lean | Quotient interaction: isomorphisms between quotients of tensor products and tensor products of quotients (`quotientTensorQuotientEquiv : (M ⧸ m) ⊗ (N ⧸ n) ≃ (M ⊗ N) ⧸ (m ⊗ N ⊔ M ⊗ n)`), one-sided versions, and ideal scalar multiplication quotients (`quotTensorEquivQuotSMul`) |
| Vanishing.lean | Vanishing criteria: characterizes when `∑ mᵢ ⊗ nᵢ = 0` via trivial vanishing (existence of witness matrices proving linear dependence), equational criterion when elements generate (`vanishesTrivially_iff_sum_tmul_eq_zero`), generalization for injective `rTensor`, and connections to flatness |
| Finiteness.lean | Finiteness preservation: every element is finite sum of pure tensors (`exists_multiset`, `exists_finset`), finite subsets contained in finitely generated submodule tensors (`exists_finite_submodule_of_setFinite`), proving finite generation is preserved by tensor products |
| DirectLimit.lean | Direct limit commutation: isomorphisms `directLimitLeft : DirectLimit G f ⊗ M ≃ DirectLimit (G · ⊗ M) (f ▷ M)` and `directLimitRight` showing tensor products commute with direct limits (colimits), with functorial maps and universal properties |
| Pi.lean | Tensor products with pi-types: natural map `piRightHom : N ⊗ (∀ i, M i) →ₗ ∀ i, N ⊗ M i`, which is isomorphism when index type is finite (packaged as `piRight`), and specializations for constant families |
| Prod.lean | Binary product interaction: isomorphisms `prodLeft : (M₁ × M₂) ⊗ N ≃ (M₁ ⊗ N) × (M₂ ⊗ N)` and `prodRight` showing tensor products distribute over binary products (see Pi.lean for arbitrary products) |
| Opposite.lean | Opposite ring distribution: algebra isomorphism `opAlgEquiv : Aᵐᵒᵖ ⊗[R] Bᵐᵒᵖ ≃ₐ[S] (A ⊗[R] B)ᵐᵒᵖ` showing `MulOpposite` distributes over tensor products with appropriate scalar tower structure |
| Matrix.lean | Matrix correspondence: `toMatrix_map` shows tensor product of linear maps corresponds to Kronecker product of matrices (`toMatrix (map f g) = toMatrix f ⊗ₖ toMatrix g`), and converse `toLin_kronecker`, establishing categorical equivalence |

## Subdirectories

- [ ] `Graded/` - Graded tensor products with signed commutativity

## Search Tags

tensor-products bilinear-maps universal-property module-theory associativity basis free-modules right-exactness quotients vanishing-criteria direct-limits finiteness algebra-towers base-change submodules subalgebras graded-algebras matrix-kronecker products pi-types opposite-rings
