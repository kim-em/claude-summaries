---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Module
generated: 2025-12-01T19:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 30
subdirs_count: 8
---

# Module

## Overview

The `Module/` directory contains the comprehensive theory of modules over rings (and semimodules over semirings), which generalize vector spaces by allowing scalar multiplication from arbitrary semirings rather than just fields. At its core, it defines the fundamental `Module R M` typeclass with axioms for distributive scalar multiplication and extends this with basic properties, specialized module types (bimodules, graded modules), and homological properties (injective and projective modules). The directory provides extensive substructure theory through eight major subdirectories: **Congruence** (quotient modules and the first isomorphism theorem), **Equiv** (linear equivalences and automorphism groups), **LinearMap** (module homomorphisms and semilinear maps with endomorphism ring structure), **Submodule** (submodules with complete lattice structure and kernel/range theory), **LocalizedModule** (localization at multiplicative sets as an exact functor), **Presentation** (modules by generators and relations with universal properties), **Torsion** (torsion submodules and torsion-free modules), and **ZLattice** (ℤ-lattices in normed spaces with covolume theory). This unified framework supports constructions ranging from elementary module theory over ℕ, ℤ, and ℚ to advanced topics including PIDs, Dedekind domains, character modules, the snake lemma, and characteristic polynomial theory for linear endomorphisms.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `Module R M` typeclass definition: extends `DistribMulAction` with `add_smul` and `zero_smul` axioms, making additive commutative monoids into semimodules over semirings |
| MinimalAxioms.lean | Constructor `Module.ofMinimalAxioms` to define module structures by proving minimal axiom set (smul_add, add_smul, mul_smul, one_smul) |
| Basic.lean | Extended module theory: units actions, inverse natural/integer scalar multiplication, support lemmas, function lifting properties |
| Hom.lean | Module instances for bundled homomorphism types (`ZeroHom`, `AddMonoidHom`, domain-acted modules) |
| Bimodule.lean | Theory of bimodules with two-sided scalar actions: modules with compatible left and right actions from different rings, using tensor products `R ⊗[ℕ] Sᵐᵒᵖ` |
| GradedModule.lean | Graded modules: `DirectSum.Decomposition` with `SetLike.GradedSMul` for additively-graded module structures `⨁ i, 𝓜 i` |
| Injective.lean | Injective modules (lifting property for injective maps) and Baer's criterion (extensions from ideals) with equivalence proof |
| Projective.lean | Projective modules: direct summands of free modules with lifting property along surjections, proof that free modules are projective |
| FinitePresentation.lean | Finitely presented modules: finitely generated with finitely generated kernel of presentation map, equivalence with finite generation over Noetherian rings |
| Lattice.lean | Lattice structure on module homomorphisms with pointwise operations |
| PID.lean | Module theory over principal ideal domains: torsion modules, rank, structure theorems |
| DedekindDomain.lean | Module theory over Dedekind domains |
| Rat.lean | Module structure on rational numbers |
| NatInt.lean | Canonical module structures for ℕ and ℤ actions on additive structures |
| ZMod.lean | Module structures on ℤ/nℤ |
| CharacterModule.lean | Character modules (homomorphisms into multiplicative group of base field) |
| SnakeLemma.lean | The snake lemma from homological algebra for module diagrams |
| SpanRank.lean | Span rank theory for modules |
| End.lean | Endomorphism modules: `Module.End R M = M →ₗ[R] M` with ring structure |
| RingHom.lean | Module structures induced by ring homomorphisms |
| Pi.lean | Module instances for dependent products (Pi types) |
| Prod.lean | Module instances for binary products |
| PUnit.lean | Module instance for the unit type |
| PointwisePi.lean | Pointwise module operations on Pi types |
| Opposite.lean | Module structures on opposite rings/modules |
| ULift.lean | Module structures on universe-lifted types |
| Shrink.lean | Universe shrinking for modules |
| Card.lean | Cardinality results for modules |
| TransferInstance.lean | Transferring module instances across equivalences |
| BigOperators.lean | Big sum operations on modules |

## Subdirectories

- [x] `Congruence/` - Congruence relations preserving scalar multiplication and addition: `SMulCon`, `VAddCon`, `ModuleCon` structures, quotient modules with inherited instances, kernel congruences, first isomorphism theorem
- [x] `Equiv/` - Linear equivalences (invertible linear maps): `LinearEquiv` structure with semilinear generalization, automorphism group structure on endomorphisms, scalar restriction, constructors from units/field elements/additive equivalences, opposite modules
- [x] `LinearMap/` - Linear maps (module homomorphisms) and semilinear maps: `LinearMap σ M M₂` with additive and scalar structure, endomorphism rings `Module.End R M`, characteristic polynomials of linear families, linear functionals on division rings, rational/star-linear maps, products
- [x] `LocalizedModule/` - Localization of modules at multiplicative sets: quotient construction `LocalizedModule S M`, `Localization S`-module structure, exactness proofs (localization as exact functor), prime/away localizations, integer elements and denominator clearing, submodule Galois insertion, equivalence with ring localization
- [x] `Presentation/` - Module presentations by generators and relations: `Relations A` structure (generators `G`, relations `R`), `Presentation A M` type with universal property, characterizations of free/finitely-presented modules, constructions for tensor products, direct sums, cokernels, tautological presentation (every module), Kähler differentials from algebra presentations, scalar restriction
- [x] `Submodule/` - Submodules and their lattice structure: `Submodule R M` as closed subsets with `SetLike` interface, complete lattice with `⊓` as intersection and `⊔` as span, kernel/range theory for linear maps, map/comap with Galois insertion/coinsertion, pointwise operations and scalar actions, equality locus, invariant submodules under endomorphisms, union bounds over fields
- [x] `Torsion/` - Torsion submodules and torsion-free modules: torsion ideals `Ideal.torsionOf R M x`, a-torsion/S-torsion submodules, `Module.IsTorsionFree` typeclass (injective scalar multiplication by regular elements), coprime decompositions with internal direct sums, quotient-by-torsion is torsion-free, vector spaces are torsion-free, product preservation
- [x] `ZLattice/` - ℤ-lattices in finite-dimensional normed vector spaces: `ZSpan` for lattices as basis spans, `IsZLattice` typeclass for discrete spanning submodules, fundamental domains with fract/floor/ceil operations, freeness and rank theorems, covolume theory with determinant formulas, lattice index via covolume ratios, p-series convergence over lattice points

## Search Tags

module semimodule vector-space scalar-multiplication bimodule graded-module injective-module projective-module finite-presentation baer-criterion homological-algebra snake-lemma submodule linear-map module-homomorphism torsion localized-module presentation lattice pid dedekind-domain character-module endomorphism
