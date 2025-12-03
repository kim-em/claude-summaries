---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Lie
generated: 2025-12-02T20:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 34
subdirs_count: 3
---

# Lie

## Overview

The `Lie/` directory contains the complete theory of Lie algebras and their modules in mathlib4, from foundational definitions through the Cartan-Dynkin-Killing classification of semisimple Lie algebras. The implementation establishes the core algebraic hierarchy (`LieRing`, `LieAlgebra`, `LieModule`) with the Jacobi identity and Leibniz rule, develops structural theory (subalgebras, ideals, submodules, quotients), representation theory (modules, morphisms, tensor products, universal enveloping algebras), and classification theory via nilpotent, solvable, and semisimple decompositions. Major results include Engel's theorem (nilpotency via nilpotent endomorphisms), Lie's theorem (common eigenvectors for solvable algebras), Cartan subalgebra existence and properties, and the complete structure theory of semisimple Lie algebras with non-degenerate Killing forms. The directory includes comprehensive treatment of classical Lie algebras (sl/sp/so), sl₂ representation theory, Killing/trace forms, derivations (proving all derivations of Killing algebras are inner), weight space decompositions with root systems for semisimple algebras, and irreducibility results for simple Lie algebras. This represents one of mathlib4's most mathematically sophisticated algebraic hierarchy implementations, authored primarily by Oliver Nash with significant contributions from Andrew Yang, Janos Wolosz, and Johan Commelin.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `LieRing`, `LieAlgebra`, `LieModule` typeclasses with Jacobi identity and Leibniz rule; `LieHom`, `LieEquiv` morphisms; fundamental lemmas for bracket operations with notations `L →ₗ⁅R⁆ L'` and `M →ₗ⁅R,L⁆ N` |
| Subalgebra.lean | `LieSubalgebra` structure as submodules closed under Lie bracket, lattice operations, Lie ring/algebra instances, `map`/`comap` under homomorphisms, `LieHom.range`, equivalences `ofInjective`/`ofEq` |
| Submodule.lean | `LieSubmodule` structure as submodules closed under Lie bracket action, complete lattice structure with Lie-preserving operations, well-foundedness for Noetherian modules, `lieSpan` construction, `map`/`comap` functoriality |
| Ideal.lean | `LieIdeal` as Lie submodules of the adjoint representation, closure under left/right bracket, coercion to `LieSubalgebra`, instances for `LieRing`/`LieAlgebra` structure on ideals |
| IdealOperations.lean | Lattice operations on ideals: arbitrary suprema/infima, normalizer, centralizer, Lie bracket of ideals `⁅I, J⁆`, derived subalgebra `⁅L, L⁆`, ideal product preservation, homomorphism compatibility |
| Quotient.lean | Quotient Lie modules `M ⧸ N` and Lie algebras `L ⧸ I` by Lie submodules/ideals, `lieQuotientLieModule` and `lieQuotientLieAlgebra` instances, quotient maps as Lie algebra homomorphisms |
| Abelian.lean | Trivial Lie modules (`LieModule.IsTrivial` where all brackets vanish), Abelian Lie algebras (`IsLieAbelian` as self-trivial module), equivalence with commutative rings via `commutative_ring_iff_abelian_lie_ring`, `LieModule.ker` and `maxTrivSubmodule`, `LieAlgebra.center` |
| Nilpotent.lean | Nilpotent Lie algebras via lower central series: `LieModule.lowerCentralSeries`, `LieModule.IsNilpotent`, `maxNilpotentSubmodule`, `LieAlgebra.maxNilpotentIdeal`, relationship with Artinian modules |
| Solvable.lean | Solvable Lie algebras via derived series: `LieAlgebra.derivedSeriesOfIdeal`, `LieAlgebra.derivedSeries`, `IsSolvable`, `derivedLength`, `radical` as maximal solvable ideal, `radicalIsSolvable` for Noetherian algebras |
| Engel.lean | Engel's theorem: Lie module `M` over Noetherian algebra `L` is nilpotent iff `toEnd L M` consists of nilpotent endomorphisms (`LieModule.isNilpotent_iff_forall`), Engelian algebras, proof for general coefficients without field assumption |
| EngelSubalgebra.lean | Engelian subalgebras and maximal Engelian subalgebras used in proof of Engel's theorem |
| LieTheorem.lean | Lie's theorem on solvable Lie algebras: finite-dimensional representations over algebraically closed fields have common eigenvectors |
| Normalizer.lean | Normalizer `N.normalizer = {x : L | ⁅x, N⁆ ≤ N}` for Lie submodules, normalizing subalgebras and ideals, properties under homomorphisms |
| CartanSubalgebra.lean | Cartan subalgebras as nilpotent self-normalizing subalgebras (`IsCartanSubalgebra`), upper central series limit characterization, splitting Cartan subalgebras |
| CartanExists.lean | Existence of Cartan subalgebras in finite-dimensional Lie algebras |
| CartanMatrix.lean | Cartan matrices for Lie algebras, generalized Cartan matrices from root data |
| Classical.lean | Classical Lie algebras: `sl(n)` special linear, `sp(n)` symplectic, `so(n)` orthogonal algebras as matrix Lie subalgebras with trace/skew-adjoint conditions, types Aₗ, Bₗ, Cₗ, Dₗ constructions and equivalences |
| Sl2.lean | `IsSl2Triple` structure for elements `(h,e,f)` satisfying sl₂ relations, primitive vectors in sl₂ representations, eigenvalue characterization for finite-dimensional representations |
| SkewAdjoint.lean | Skew-adjoint matrices under bilinear forms, connection to orthogonal and symplectic Lie algebras |
| Matrix.lean | Lie algebra structure on matrices via commutator, connection to endomorphism algebras |
| OfAssociative.lean | Lie ring structure on associative rings via commutator bracket `⁅x,y⁆ = x*y - y*x`, `LieRing.of_associative_ring_bracket` |
| NonUnitalNonAssocAlgebra.lean | Lie algebra structure on non-unital non-associative algebras |
| Free.lean | Free Lie algebras `FreeLieAlgebra R X` as quotient of free non-associative algebra, universal property `lift : (X → L) ≃ (FreeLieAlgebra R X →ₗ⁅R⁆ L)`, `of : X → FreeLieAlgebra R X` |
| UniversalEnveloping.lean | Universal enveloping algebra construction for Lie algebras, Poincaré-Birkhoff-Witt basis |
| BaseChange.lean | Base change for Lie algebras: scalar extension functoriality |
| Extension.lean | Lie algebra extensions: short exact sequences of Lie algebras, extension classification |
| DirectSum.lean | Direct sum constructions for Lie algebras and modules |
| TensorProduct.lean | Tensor products of Lie modules with module structure |
| InvariantForm.lean | Invariant bilinear forms on Lie algebras (associativity property: `B(⁅x,y⁆, z) = B(x, ⁅y,z⁆)`), relationship with Killing form |
| TraceForm.lean | Trace form `traceForm R L M` for representations `L → End(M)` defined as `B(x,y) = Tr(φ(x)∘φ(y))`, vanishing for nilpotent representations, Killing form as special case |
| Killing.lean | Killing form (trace form of adjoint representation), `IsKilling` typeclass for non-degenerate Killing form, semisimplicity and trivial radical results, characteristic zero vs positive characteristic distinctions |
| Character.lean | Characters of Lie algebra representations |
| Cochain.lean | Lie algebra cochains for cohomology theory |
| Rank.lean | Rank theory for Lie algebras |

## Subdirectories

- [x] `Derivation/` - Lie derivations satisfying Leibniz rule `D ⁅a, b⁆ = ⁅a, D b⁆ - ⁅b, D a⁆`, algebraic structure on derivations, adjoint action `ad : L →ₗ⁅R⁆ LieDerivation R L L`, kernel characterization via center, and proof that all derivations of finite-dimensional Killing Lie algebras are inner derivations (complete)
- [x] `Semisimple/` - Theory of simple and semisimple Lie algebras: irreducible Lie modules, simple algebras (irreducible under adjoint action), semisimple algebras (direct sums of simple ideals with Boolean ideal lattice), reductive algebras (trivial or central radical), equivalence of trivial radical with absence of solvable ideals, and representation-theoretic criteria via irreducible faithful representations (complete)
- [x] `Weights/` - Weight space decompositions as simultaneous generalized eigenspaces, weight space independence and completeness, linearity of weights in characteristic zero or for Abelian algebras, chain techniques for root families, complete theory of roots for algebras with non-degenerate Killing forms (Cartan subalgebras are Abelian, roots span dual space, root spaces one-dimensional), root system construction from splitting semisimple algebras, and irreducibility of root systems for simple Lie algebras (complete)

## Search Tags

lie-algebra lie-ring lie-module jacobi-identity bracket subalgebra ideal nilpotent solvable engel-theorem lie-theorem cartan-subalgebra classical-lie-algebras sl2 killing-form trace-form free-lie-algebra universal-enveloping-algebra representation-theory weight-space semisimple abelian quotient homomorphism morphism equivalence derivation cohomology