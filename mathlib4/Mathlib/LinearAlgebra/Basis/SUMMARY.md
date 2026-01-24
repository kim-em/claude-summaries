---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Basis
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 12
subdirs_count: 0
---

# Basis

## Overview

This directory contains the core theory of bases in modules and vector spaces. It establishes the fundamental definition of a basis as a linear equivalence `M ≃ₗ[R] ι →₀ R` (via the `repr` function mapping elements to coordinates), provides the key equivalence between bases and linearly independent spanning sets, and develops specialized basis constructions and operations including reindexing, mapping, products, scalar multiplication, and finite-indexed variations. The theory covers both general modules over semirings and specialized results for vector spaces over division rings, with emphasis on coordinate representations, extensionality principles, and relationships with submodules.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Basis ι R M` as structure wrapping `repr : M ≃ₗ[R] ι →₀ R`, basis vectors as `b i = repr.symm (single i 1)`, coordinate functions (`coord`), basis construction from linear equivalences (`ofRepr`, `ofEquivFun`), reindexing (`reindex`), mapping (`map`), and extension via `constr` defining linear maps by specifying values on basis elements |
| Basic.lean | Fundamental properties proving equivalence between bases and linearly independent spanning families: `Basis.linearIndependent`, `Basis.span_eq`, `Basis.mk` constructor from `LinearIndependent v` and `span (range v) = ⊤`, lemmas on basis existence in nontrivial modules (`index_nonempty`), representation support characterization, and membership in span via coordinate support |
| VectorSpace.lean | Vector space specializations over division rings: `Basis.extend` extending linearly independent sets to bases using Zorn's lemma, `Basis.sumExtend` providing sum-indexed extension `ι ⊕ sumExtendIndex`, `Basis.extendLe` for extending within a spanning set, `Basis.ofVectorSpace` proving every vector space has a basis, and `Module.Free.of_divisionRing` establishing free module structure |
| Submodule.lean | Submodule basis theory: `Basis.mem_submodule_iff` characterizing membership as linear combinations of submodule basis vectors (finite variant `mem_submodule_iff'`), `Basis.eq_bot_of_rank_eq_zero` showing submodules with no nontrivial linearly independent sets are trivial, and `Submodule.inductionOnRankAux` for induction on finite-rank submodules by adjoining independent elements |
| Cardinality.lean | Cardinality constraints on bases: `basis_finite_of_finite_spans` showing finite spanning sets imply finite bases over nontrivial rings, `finite_of_span_finite_eq_top_finsupp` for finsupp-valued bases, `union_support_maximal_linearIndependent_eq_range_basis` proving maximal linearly independent sets have representations supported on entire basis index (Lazarus 1973 result for basis cardinality uniqueness) |
| Bilinear.lean | Bilinear map extensionality and evaluation: `LinearMap.ext_basis` proving bilinear maps equal when agreeing on basis pairs, `sum_repr_mul_repr_mulₛₗ` and `sum_repr_mul_repr_mul` expressing `B x y` as sums over basis evaluations `B (b₁ i) (b₂ j)` weighted by coordinates (semi-bilinear and bilinear versions) |
| Exact.lean | Basis construction from split exact sequences: given `0 → K → M → P → 0` with retraction `s : M → K` and basis `v : ι → M`, provides `LinearIndependent.linearIndependent_of_exact_of_retraction` showing images form independent set when kernel conditions met, and span conditions for quotient basis construction from exact sequences |
| Fin.lean | Finite-index basis operations: `Basis.mkFinCons` constructing `Basis (Fin (n+1)) R M` by adjoining independent vector `y` to submodule basis `Basis (Fin n) R N`, extending the basis by one dimension with specified linear independence and spanning conditions |
| Flag.lean | Flag subspaces from ordered bases: `Basis.flag b k` defining subspace spanned by first `k` basis vectors, monotonicity (`flag_mono`) and strict monotonicity over nontrivial rings (`flag_strictMono`), covering relations (`flag_covBy`), relationships with dual coordinate kernels (`flag_le_ker_coord_iff`), and `Basis.toFlag` constructing maximal chains of subspaces |
| MulOpposite.lean | Opposite space bases: `Basis.mulOpposite` mapping basis `b` to opposite basis via `b.mulOpposite i = op (b i)`, representation equivalences (`mulOpposite_repr_eq`, `repr_unop_eq_mulOpposite_repr`), instances proving opposite spaces finite-dimensional and free when original space is, with rank preservation theorems |
| Prod.lean | Product space bases: `Basis.prod` constructing `Basis (ι ⊕ ι') R (M × M')` from bases `Basis ι R M` and `Basis ι' R M'`, coordinate projection lemmas (`prod_repr_inl`, `prod_repr_inr`), component formulas (`prod_apply_inl_fst`, etc.), and `Module.Free.prod` instance for products of free modules |
| SMul.lean | Scalar multiplication of bases: `SMul G (Basis ι R M)` instance acting on each basis vector, `Basis.groupSMul` and `Basis.unitsSMul` constructing scaled bases from group/unit actions with proofs of linear independence and spanning preservation, coordinate transformations (`coord_unitsSMul`, `repr_unitsSMul`), and `Basis.isUnitSMul` for `IsUnit`-valued scaling |

## Subdirectories

(No subdirectories)

## Search Tags

basis bases module vector-space linear-algebra coordinates representation linear-independent spanning finsupp reindex map construct extend product flag submodule bilinear cardinality finite-dimensional free-module exact-sequence scalar-multiplication opposite-space fin-indexed division-ring semiring
