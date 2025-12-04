---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/DirectSum
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 10
subdirs_count: 0
---

# DirectSum

## Overview

The `DirectSum/` directory implements direct sum constructions for algebraic structures, providing both the basic definition of direct sums of abelian groups as `DirectSum ι β := Π₀ i, β i` (dependent finitely supported functions) and comprehensive theory for graded structures. It covers direct sums of modules with universal properties, additively-graded rings where multiplication maps `A i → A j → A (i + j)`, algebra structures on graded direct sums, internal/external grading correspondence, and constructive decomposition theory. The directory includes specialized results for additive characters, linear maps between direct sums, equivalences with finsupp, and decompositions via orthogonal idempotents.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition `DirectSum ι β := Π₀ i, β i` for direct sums of additive commutative monoids, notation `⨁ i, β i`, basic operations (addition, subtraction, single element injection `of`), extensionality, support theory, and `AddCommGroup` instance |
| Module.lean | Module structure on direct sums with `R`-module instance, universal property via `toModule` and uniqueness, inclusion maps `lof` and `lmk` as linear maps, internal decompositions of modules via `coeLinearMap` for submodules, and basis theory for direct sum decompositions |
| Ring.lean | Additively-graded ring structures with typeclasses `GNonUnitalNonAssocSemiring`, `GSemiring`, `GRing`, `GCommSemiring`, `GCommRing` for multiplication `A i → A j → A (i + j)`, inducing `Semiring`/`Ring`/`CommRing` instances on `⨁ i, A i`, grade zero algebra `GradeZero` with module structures, and `toSemiring` ring homomorphism respecting universal property |
| Algebra.lean | Graded algebra structures via `GAlgebra R A` typeclass requiring algebra map `R →+ A 0` compatible with graded multiplication, producing `Algebra R (⨁ i, A i)` instance with `algebraMap` factoring through grade zero, `SMulCommClass` and `IsScalarTower` instances, and `toAlgebra` algebra homomorphism extending `toSemiring` |
| Internal.lean | Internally graded structures connecting direct sums of subobjects to their carrier types, `SetLike.GradedMonoid` instances for submonoids/subgroups/submodules providing `GSemiring`/`GCommSemiring`, bundled canonical maps `coeRingHom : (⨁ i, A i) →+* R` and `coeAlgHom : (⨁ i, A i) →ₐ[S] R`, and `GradeZero` structures (subsemiring, subring, subalgebra) on the zero component |
| Decomposition.lean | Constructive decomposition theory with `DirectSum.Decomposition ℳ` typeclass providing canonical equivalence `decompose ℳ : M ≃+ ⨁ i, ℳ i` from an additive monoid into submonoids, variants for groups (`AddEquiv`), modules (`LinearEquiv`), rings (`RingEquiv`), and algebras (`AlgEquiv`), and connection to `DirectSum.IsInternal` predicate |
| LinearMap.lean | Linear maps respecting direct sum decompositions with block-diagonal matrix representations via `toMatrix_directSum_collectedBasis_eq_blockDiagonal'`, diagonal vanishing results for maps between different components, trace formulas for endomorphisms on direct sums, and diagonalizability criteria using decompositions into eigenspaces |
| Finsupp.lean | Linear equivalence `finsuppLEquivDirectSum : (ι →₀ M) ≃ₗ[R] ⨁ _ : ι, M` between finitely supported functions and direct sums of modules, compatibility with `single`/`lof` operations, and applications to basis conversions |
| AddChar.lean | Direct sum of additive characters with `AddChar.directSum : (∀ i, AddChar (G i) R) → AddChar (⨁ i, G i) R` constructed via `toAddMonoidHomEquiv` and universal property, and injectivity of the direct sum construction |
| Idempotents.lean | Decomposition of semiring identity into orthogonal idempotents: when `R = V₁ ⊕ ⋯ ⊕ Vₙ` for ideals `Vᵢ`, the decomposition `1 = e₁ + ⋯ + eₙ` with `eᵢ ∈ Vᵢ` yields `IsIdempotentElem eᵢ` and `CompleteOrthogonalIdempotents` structure with `eᵢ * eⱼ = 0` for `i ≠ j` |

## Subdirectories

(none)

## Search Tags

direct-sum graded-structures additive-groups modules algebras internal-grading external-grading decomposition universal-property finsupp dfinsupp graded-rings graded-algebras orthogonal-idempotents additive-characters linear-maps block-diagonal
