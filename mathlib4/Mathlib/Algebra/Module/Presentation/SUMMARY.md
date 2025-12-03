---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Module/Presentation
generated: 2025-12-01T18:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 9
subdirs_count: 0
---

# Presentation

## Overview

The `Presentation/` directory implements module presentations by generators and relations, a foundational concept for describing modules in terms of explicit generators subject to explicit linear relations. It defines the `Relations A` structure (generators indexed by type `G`, relations indexed by type `R`) and `Presentation A M` type (proof that a module `M` satisfies the universal property for a given generators-and-relations system). The theory proves that free modules correspond to presentations with no relations, finitely presented modules correspond to presentations with finitely many generators and relations, and provides constructions for presentations of tensor products, direct sums, cokernels, tautological presentations (using all elements as generators), differentials (from algebra presentations), and scalar restriction. All work is by Joël Riou (2024).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `Relations A` structure (generators `G`, relations `R`, coefficients `relation : R → G →₀ A`), quotient module construction, `Solution M` type (assignments of module elements to generators satisfying relations), `IsPresentation` predicate (solution satisfies universal property), `Presentation A M` bundled type, universal property (`desc`, `linearMapEquiv`, uniqueness) |
| Free.lean | Characterization `free_iff_exists_presentation`: modules are free iff they admit presentations with generators but no relations (`IsEmpty R`), `solutionFinsupp` presentation for `G →₀ A` |
| Finite.lean | Equivalence `finitePresentation_iff_exists_presentation`: modules are finitely presented (in sense of `Module.FinitePresentation`) iff they admit presentations with finitely many generators and finitely many relations |
| Cokernel.lean | Presentation construction for cokernel: given `f : M₁ →ₗ[A] M₂`, presentation of `M₂`, and generators of `M₁`, constructs presentation of `M₂ ⧸ LinearMap.range f`, generalized to exact sequences via `ofExact` |
| Tensor.lean | Presentation of tensor products: given presentations of `M₁` and `M₂`, constructs presentation of `M₁ ⊗[A] M₂` with generators `G₁ × G₂` and two types of relations (one from each factor) |
| DirectSum.lean | Presentation of direct sums: from family of presentations `pres : ∀ i, Presentation A (M i)` constructs presentation of `⨁ i, M i` using `Sigma` types for generators/relations, includes `finsupp` presentation for `ι →₀ M` |
| Tautological.lean | Universal tautological presentation: every module `M` admits presentation with generators `[m]` for each `m : M` and relations `[m₁] + [m₂] - [m₁ + m₂] = 0` and `a • [m] - [a • m] = 0`, proves `tautologicalRelationsSolutionEquiv` identifying solutions with `M →ₗ[A] N` |
| Differentials.lean | Presentation of Kähler differentials: from presentation `pres : Algebra.Presentation R S` of algebra `S`, constructs presentation of `S`-module `Ω[S⁄R]` with generators indexed by algebra generators `ι` and relations from differentials of algebra relations, proved using exactness of cotangent complex |
| RestrictScalars.lean | Scalar restriction: given `A → B`, presentation of `B` as `A`-module, and presentation of `M` as `B`-module, constructs presentation of `M` as `A`-module (requires additional lifting data) |

## Subdirectories

None.

## Search Tags

module-presentation generators-relations free-module finitely-presented universal-property tensor-product direct-sum cokernel tautological-presentation kahler-differentials scalar-restriction exact-sequence quotient-module linear-algebra homological-algebra
