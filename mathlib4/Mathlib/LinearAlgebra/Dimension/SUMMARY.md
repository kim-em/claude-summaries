---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Dimension
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 14
subdirs_count: 1
---

# Dimension

## Overview

The `Dimension/` subdirectory contains mathlib4's formalization of dimension theory for modules and vector spaces. Core definitions include `Module.rank` (cardinal-valued dimension as supremum of cardinalities of linearly independent subsets) and `Module.finrank` (natural-number-valued dimension for finite-dimensional spaces, 0 by convention for infinite-dimensional spaces). The directory establishes fundamental dimension theorems: rank-nullity theorem (`HasRankNullity` typeclass with instances for division rings and commutative domains), tower law for field extensions (rank_F(A) = rank_F(K) × rank_K(A)), dimension formulas for constructions (products, quotients, direct sums, tensor products, finsupp), and the Erdős-Kaplansky theorem (infinite-dimensional dual spaces have dimension equal to their cardinality). Files cover dimension theory under various ring conditions: strong rank condition (cardinality bounds for linearly independent sets vs spanning sets), invariant basis number (all bases have same cardinality), free modules (bases exist, dimension well-defined), division rings (full rank-nullity theorem), and commutative domains (rank-nullity via localization to fraction fields).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition: `Module.rank R M` as supremum of cardinalities of linearly independent subsets, basic inequalities (rank_le_card, rank bounds for injective/surjective maps), and foundational lemmas for working with rank as a cardinal |
| Finrank.lean | Natural number rank: `Module.finrank R M = Cardinal.toNat (Module.rank R M)`, conversions between cardinal rank and natural number rank (finrank_eq_of_rank_eq, rank_eq_ofNat_iff_finrank_eq_ofNat), and inequalities relating finrank to rank |
| Constructions.lean | Dimension formulas for module constructions: quotients (rank_quotient_add_rank_le), products (rank_prod for free modules), finsupp (rank_finsupp = #ι × rank M), direct sums (rank_directSum = ∑ rank Mᵢ), tensor products (rank_tensorProduct = rank M × rank N), and subalgebras/submodules |
| RankNullity.lean | Rank-nullity theorem typeclass: `HasRankNullity R` asserting (1) every module has linearly independent subset of cardinality equal to its rank, (2) rank(M/N) + rank(N) = rank(M) for all submodules N, main consequence `LinearMap.lift_rank_range_add_rank_ker` (rank nullity for linear maps) |
| DivisionRing.lean | Rank-nullity for division rings: `DivisionRing.hasRankNullity` instance proving division rings satisfy HasRankNullity, `rank_quotient_add_rank_of_divisionRing` (exact equality for quotients), and dimension-preserving properties of linear maps over fields |
| Localization.lean | Dimension of localizations: `IsLocalizedModule.lift_rank_eq` (rank_Rₚ Mₚ = rank_R M), `IsLocalization.rank_eq` (base change preserves rank), rank-nullity for commutative domains (`IsDomain.hasRankNullity` via reduction to fraction field), and universe-polymorphic formulations |
| Free.lean | Dimension of free modules: tower law (rank_mul_rank for field extensions), `LinearEquiv.nonempty_equiv_iff_lift_rank_eq` (free modules isomorphic iff same rank), `Module.finBasis` (arbitrary Fin n basis given finrank = n), and rank formulas specific to free modules over rings with strong rank condition |
| StrongRankCondition.lean | Strong rank condition theory: `linearIndependent_le_span` (linearly independent family has cardinality ≤ spanning set for finite spanning), `mk_eq_mk_of_basis` (dimension theorem: all bases have same cardinality under invariant basis number), Basis.le_span (basis cardinality ≤ spanning set cardinality), and `Algebra.IsQuadraticExtension` (rank 2 algebra extensions) |
| Finite.lean | Finite dimension characterization: `rank_le` (bounding rank via finite linear independence), `rank_eq_zero_iff` (rank zero iff all elements torsion), `rank_eq_one_iff` (rank one iff cyclic module), and conditions for rank to be finite (rank_lt_aleph0 equivalences) |
| FreeAndStrongRankCondition.lean | Free modules over strong rank condition rings: `Basis.ofRankEqZero` (basis construction for zero-dimensional spaces), `le_rank_iff_exists_linearIndependent` (rank characterized by existence of independent sets), `rank_le_one_iff` (dimension ≤1 iff all vectors are scalar multiples of single vector), generalizations of division ring results to strong rank condition setting |
| LinearMap.lean | Rank of linear maps: `LinearMap.rank f` defined as dimension of range f, inequalities `rank_le_range` and `rank_le_domain`, basic properties (rank_zero, rank composition bounds), and relationship between map rank and module dimension |
| ErdosKaplansky.lean | Erdős-Kaplansky theorem: `rank_dual_eq_card_dual_of_aleph0_le_rank` stating that infinite-dimensional dual space over division ring has dimension equal to its cardinality (#(V →ₗ[K] K) = #(V →ₗ[K] K)), key lemma `max_aleph0_card_le_rank_fun_nat` establishing lower bound for function spaces |
| OrzechProperty.lean | Dimension under Orzech property: `linearIndependent_of_top_le_span_of_card_eq_finrank` (spanning set of cardinality = finrank is basis), `basisOfTopLeSpanOfCardEqFinrank` constructions (basis from spanning sets for rings satisfying Orzech property), characterization `linearIndependent_iff_card_eq_finrank_span` |
| Subsingleton.lean | Trivial module dimension: rank_subsingleton' (rank of subsingleton module over nontrivial ring is 0), rank_punit, and rank_bot lemmas establishing dimension zero for trivial modules |

## Subdirectories

- [ ] `Torsion/` - Dimension theory for torsion modules

## Search Tags

dimension rank finrank module vector-space basis cardinal linear-independence rank-nullity quotient product tensor-product direct-sum free-module strong-rank-condition invariant-basis-number division-ring field localization tower-law erdos-kaplansky dual-space finite-dimensional torsion orzech-property subsingleton linear-map
