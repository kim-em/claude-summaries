---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/FreeModule
generated: 2026-01-25T23:52:30Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 1
---

# FreeModule

## Overview

The `FreeModule/` directory formalizes the theory of free modules over rings and principal ideal domains (PIDs), establishing foundational properties and structural decomposition theorems. Core theory begins with the definition of free modules (modules admitting a basis) and construction of canonical bases via the axiom of choice, together with the universal property relating functions from basis elements to linear maps. For PIDs, the directory proves the fundamental structure theorem: submodules of finite-rank free modules are themselves free and finite-rank, with Smith normal form providing explicit diagonal basis representations.

The Finite/ subdirectory specializes to finite-rank free modules, establishing that fintype-indexed bases yield finite modules and that finite free modules have fintype basis indices. For PIDs, quotient decompositions express M⧸N as products of cyclic modules R⧸⟨aᵢ⟩ using Smith coefficients. Integer modules receive detailed treatment: quotient cardinalities are computed via determinants of basis change matrices, subgroup indices relate to Smith coefficients, and G/nG has cardinality n^rank for finite free ℤ-modules. The directory further proves that linear map spaces (M →ₗ N) are free/finite when M and N are, with explicit rank formulas.

Additional specialized results include ideal quotient decompositions, norm characterizations via Smith coefficients for polynomial algebras, and the strong rank condition for commutative rings (ensuring invariant basis number). Determinant theory for free finite modules establishes that zero endomorphisms have zero determinant in nontrivial settings.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core free module theory: `Module.Free R M` class (modules with basis), `ChooseBasisIndex` type and `chooseBasis` construction (via axiom of choice), universal property (`constr` relating functions on basis to linear maps), basic instances (self, prod, pi, ulift, finsupp) |
| Determinant.lean | Determinant for free finite modules: `LinearMap.det_zero''` theorem (determinant of zero endomorphism is zero in nontrivial finite free modules) |
| IdealQuotient.lean | Ideal quotients over PIDs: `quotientEquivPiSpan` (decompose S⧸I as product of R⧸⟨aᵢ⟩ for Smith coefficients), `quotientEquivPiZMod` (for ℤ-algebras), `quotientEquivDirectSum` (direct sum variant), finiteness results for nonzero ideal quotients |
| Int.lean | Submodule index theory for free ℤ-modules: Smith normal form index formulas (`toAddSubgroup_index_eq_pow_mul_prod`), relating additive subgroup index to product of ideal indexes and rank deficiency, with applications to finite index characterization |
| ModN.lean | Quotient by n-multiples: `ModN G n` as G/nG with ZMod n module structure, universal properties (`liftEquiv` for additive homomorphisms, `liftEquiv'` for ZMod-linear maps), `basis` construction from ℤ-basis to ZMod-basis, cardinality formula (n^rank) for finite free ℤ-modules |
| Norm.lean | Norms and Smith coefficients: `associated_norm_prod_smith` (algebra norm associated to product of Smith coefficients for nonzero elements), `finrank_quotient_span_eq_natDegree_norm` (dimension of quotient by principal ideal equals degree of norm for polynomial algebras) |
| PID.lean | Submodules of free modules over PIDs: induction on rank, `exists_basis_of_pid` (submodules are free and finitely generated), `smithNormalForm` (diagonal basis representation bN i = aᵢ • bM i), fundamental structure theorem for modules over PIDs |
| StrongRankCondition.lean | Rank invariance: `commRing_strongRankCondition` instance (nontrivial commutative rings satisfy strong rank condition), ensures injective maps (Fin n → R) →ₗ (Fin m → R) require n ≤ m, guarantees invariant basis number property |

## Subdirectories

- [x] `Finite/` - Finite-rank free modules: fintype basis indices, quotient decompositions via Smith normal form, cardinality formulas via determinants, linear map module structures with rank formulas

## Search Tags

free-modules basis rank principal-ideal-domain PID smith-normal-form submodules quotient-modules determinant integer-modules zmod cardinality universal-property strong-rank-condition invariant-basis-number finitely-generated structure-theorem ideal-quotient norm polynomial-modules
