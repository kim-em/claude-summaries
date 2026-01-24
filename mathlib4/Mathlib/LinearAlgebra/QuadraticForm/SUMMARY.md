---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/QuadraticForm
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 10
subdirs_count: 2
---

# QuadraticForm

## Overview

The `QuadraticForm/` directory formalizes quadratic maps and quadratic forms on modules over commutative rings. A quadratic map `Q : M → N` satisfies `Q(a • x) = (a * a) • Q(x)` and has a companion bilinear map (the polar form). The directory includes fundamental theory (isometries, equivalences, tensor products), basis-dependent constructions, and classification results for real and complex quadratic forms. Key results include correspondence with symmetric bilinear forms (when 2 is invertible), Sylvester's law of inertia for real quadratic forms, and equivalence to sum of squares for complex forms. Also includes categorical perspectives through the `QuadraticModuleCat` category.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core quadratic map structure: definition as maps `Q : M → N` with `Q(a • x) = (a * a) • Q(x)` and companion bilinear map, polar form `polar Q x y = Q(x + y) - Q(x) - Q(y)` (associated bilinear map up to factor 2), correspondence with symmetric bilinear forms via `QuadraticMap.associated` (requires invertible 2), anisotropic forms, positive definite forms (`PosDef`), discriminant, orthogonality predicate (`IsOrtho`), and composition/scalar multiplication operations |
| Basis.lean | Basis-dependent bilinear map construction: `QuadraticMap.toBilin` produces triangular bilinear form from ordered basis (works in characteristic 2 unlike `associated`), expansion formulas for quadratic maps on linear combinations (`apply_linearCombination` expressing `Q(∑ lᵢ • bᵢ)` as sum of diagonal terms plus polar cross-terms), and proof that every quadratic map on free modules comes from a bilinear form (`BilinMap.toQuadraticMap_surjective`) |
| Dual.lean | Dual space quadratic forms: `QuadraticForm.dualProd` on `Module.Dual R M × M` defined as `(f, x) ↦ f x`, associated symmetric bilinear form `LinearMap.dualProd`, separating-left characterization via dual evaluation injectivity, and form-preserving map `QuadraticForm.toDualProd : (Q.prod <| -Q) →qᵢ dualProd R M` |
| Isometry.lean | Isometric linear maps: `QuadraticMap.Isometry Q₁ Q₂` structure for linear maps preserving quadratic forms (notation `Q₁ →qᵢ Q₂`), composition, identity, and zero isometries, coercion to linear maps with extensionality, and isometry transfer under equivalences |
| IsometryEquiv.lean | Isometric equivalences: `QuadraticMap.IsometryEquiv Q₁ Q₂` for linear equivalences preserving quadratic forms, propositional equivalence `Equivalent Q₁ Q₂` (nonempty isometric equivalence), equivalence relation properties (reflexivity, symmetry, transitivity), basis change isometries, and canonical forms (`equivalent_weighted_sum_squares`: finite-dimensional quadratic forms are equivalent to weighted sum of squares) |
| Prod.lean | Product and pi-type quadratic forms: `QuadraticForm.prod Q₁ Q₂` on product types (applying `Q₁`, `Q₂` componentwise), `QuadraticForm.pi` for indexed products, equivalence results (`Equivalent.prod`, `Equivalent.pi` showing component equivalence implies total equivalence), and characterization of positive definiteness/semidefiniteness on products (`posDef_prod_iff`, `nonneg_pi_iff`) |
| TensorProduct.lean | Tensor product of quadratic forms: `QuadraticForm.tensorDistrib (Q₁ ⊗ₜ Q₂)` constructing quadratic form on `M₁ ⊗ M₂` from forms on factors (requires invertible 2), tensor product of isometries, compatibility with associated bilinear forms, and equivalences under tensor product |
| Real.lean | Real quadratic form classification: Sylvester's law of inertia (`equivalent_one_neg_one_weighted_sum_squared` showing every real quadratic form is equivalent to weighted sum of squares with weights ±1 or 0), nondegenerate case with weights ±1 only, and isometry `isometryEquivSignWeightedSumSquares` normalizing arbitrary weights to their signs |
| Complex.lean | Complex quadratic form classification: `equivalent_sum_squares` proving nondegenerate complex quadratic forms are equivalent to unweighted sum of squares, `isometryEquivSumSquares` normalizing arbitrary weights to 0 or 1, and `complex_equivalent` showing all nondegenerate quadratic forms over ℂ of the same dimension are equivalent |
| QuadraticModuleCat.lean | Category of quadratic modules: `QuadraticModuleCat R` structure combining module with quadratic form, morphisms as isometries (`Hom V W` wrapping `QuadraticMap.Isometry`), category structure with composition and identities, forgetful functor to `ModuleCat`, and categorical framework for studying quadratic forms |

## Subdirectories

- [x] `QuadraticModuleCat/` - Categorical structures for quadratic modules
- [ ] `TensorProduct/` - Additional tensor product theory for quadratic forms

## Search Tags

quadratic-forms quadratic-maps polar-form bilinear-forms isometry isometric-equivalence basis-construction tensor-products dual-forms product-forms real-quadratic-forms complex-quadratic-forms sylvester-law-inertia canonical-forms weighted-sum-squares positive-definite anisotropic discriminant orthogonality category-theory module-categories
