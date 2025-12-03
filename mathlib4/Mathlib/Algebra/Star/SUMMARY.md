---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Star
generated: 2025-12-01T00:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 26
subdirs_count: 0
---

# Star

## Overview

The `Star/` directory provides the foundations of star (involution) algebra, defining the core typeclasses for structures equipped with an involutive antiautomorphism operation (star/adjoint). This includes star monoids where `star (r * s) = star s * star r`, star rings extending these to semirings/rings, star modules with compatible scalar actions, and star algebras combining all three. The directory contains both the fundamental mixin typeclasses (`InvolutiveStar`, `StarMul`, `StarRing`, `StarModule`) and rich theory for specialized elements (self-adjoint, unitary, normal), morphisms preserving the star operation, and substructures closed under star, serving as the algebraic foundation for C*-algebras and quantum mechanics.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core star operation typeclasses: `StarMemClass` for star-closed subsets, `InvolutiveStar` with `star_involutive`, `TrivialStar` for identity star (ℝ), `StarMul` with `star (r * s) = star s * star r`, and extensions to `StarAddMonoid`, `StarNonUnitalSemiring`, `StarRing`, `StarModule` with compatibility axioms |
| Module.lean | Star operation bundled as star-linear equivalence `starLinearEquiv` for star algebras, with scalar multiplication compatibility lemmas (`star_natCast_smul`, `star_intCast_smul`, `star_ratCast_smul`) and `StarModule` instances for ℚ≥0 and ℚ actions |
| StarAlgHom.lean | Morphisms of star algebras: `NonUnitalStarAlgHom` and `StarAlgHom` extending algebra homomorphisms with `map_star'` preservation, composition, identity, equivalences, and connections to continuous functional calculus |
| SelfAdjoint.lean | Self-adjoint elements (`IsSelfAdjoint x` where `star x = x`) forming additive subgroups, skew-adjoint elements (`star x = -x`), and normal elements (`IsStarNormal x` where `star x * x = x * star x`) with module structures and functional calculus support |
| Unitary.lean | Unitary elements as submonoid/group: `unitary R = {U | star U * U = 1 ∧ U * star U = 1}` with group structure using star as inverse, continuous functional calculus, spectrum theory, and matrix specializations |
| Subalgebra.lean | `StarSubalgebra R A` combining `Subalgebra` with `star_mem'` closure, complete lattice structure, centralizer results, adjoin operations, and `StarModule` instance inheritance |
| NonUnitalSubalgebra.lean | Non-unital star subalgebras: `NonUnitalStarSubalgebra R A` extending `NonUnitalSubalgebra` with star closure, lattice operations, centralizer theory, and adjoin constructions without unit requirement |
| NonUnitalSubsemiring.lean | Non-unital star subsemirings without scalar action requirement, providing more general star-closed subsemiring structure |
| Subsemiring.lean | `StarSubsemiring` for semirings with star: subrings/subsemirings closed under star with coercion to `Subsemiring`, instances, and center closure results |
| StarRingHom.lean | Star ring homomorphisms: `StarRingHom` bundling `RingHom` with `map_star'`, `NonUnitalStarRingHom` for non-unital case, extensionality, composition, and equivalences |
| MonoidHom.lean | Star monoid homomorphisms between monoids with star operations, bundling multiplication and star preservation |
| LinearMap.lean | Star-linear maps between star modules with lemmas for addition, scalar multiplication, projection operators, and applications to probability theory |
| CentroidHom.lean | Star-preserving centroid homomorphisms for non-unital semirings with star structure |
| CHSH.lean | Clauser-Horne-Shimony-Holt (CHSH) inequality and Tsirelson's bound in ordered star-rings: proves `A₀*B₀ + A₀*B₁ + A₁*B₀ - A₁*B₁ ≤ 2` (commutative case) and `≤ 2√2` (general case) for self-adjoint involutions, foundational for quantum mechanics vs local hidden variables |
| Free.lean | Star structure on free monoid (`List.reverse`) and free algebra (word reversal via `MulOpposite` construction) |
| Center.lean | Interaction of star operation with `Set.center` and `Set.centralizer`: proves star preserves center and establishes `star s.centralizer = (star s).centralizer` |
| Conjneg.lean | Conjneg operation (conjugate-negate) on star additive groups, combining star with negation |
| Pi.lean | Star structures on Pi types (dependent functions) with pointwise star operation |
| Prod.lean | Star structures on product types with componentwise star operation |
| Pointwise.lean | Pointwise star operation on sets: `star s = {star x | x ∈ s}` with algebraic properties and interactions with set operations |
| BigOperators.lean | Star operation commutes with finite sums and products: `star (∑ i ∈ s, f i) = ∑ i ∈ s, star (f i)` |
| StarProjection.lean | Star projections in rings: idempotent self-adjoint elements with `star p = p` and `p * p = p`, forming a complete lattice |
| UnitaryStarAlgAut.lean | `unitaryStarAlgAut`: the automorphism group of a star algebra given by conjugation with unitary elements |
| Rat.lean | `StarRing ℚ` instance with trivial star (identity) and related instances |
| RingQuot.lean | Star structure on ring quotients `RingQuot s` when the relation is star-invariant |
| TensorProduct.lean | Star structure on tensor products of star algebras with `star (a ⊗ b) = star a ⊗ star b` |

## Subdirectories

(none)

## Search Tags

star-algebra involution adjoint self-adjoint unitary normal star-ring star-module C*-algebra quantum-mechanics CHSH-inequality Tsirelson star-homomorphism star-subalgebra functional-calculus
