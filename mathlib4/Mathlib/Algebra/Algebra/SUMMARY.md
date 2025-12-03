---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Algebra
generated: 2025-12-01T20:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 24
subdirs_count: 3
---

# Algebra

## Overview

The `Algebra/` directory defines the fundamental typeclass for algebras over commutative rings and provides comprehensive theory for working with algebra structures. An algebra `A` over a commutative ring `R` is a ring equipped with a compatible ring homomorphism `R → A` into its center, equivalently a module where scalar multiplication commutes and associates with ring multiplication. This folder contains 24 files covering core definitions (`Algebra`, `AlgHom`, `AlgEquiv`), bundled structures (subalgebras with complete lattice structure via `Algebra.adjoin`, non-unital subalgebras), tower theory for multi-layer algebra constructions, operations on submodules of algebras including pointwise multiplication and quotients, and specialized constructions including unitization, restriction of scalars, product algebras, and opposite algebras. Three subdirectories provide deeper theory: specialized homomorphisms for rational algebras, comprehensive subalgebra theory including closure operations and centralizers, and spectral theory capturing when elements fail to be invertible after scalar shifts.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `Algebra R A` typeclass definition for associative unital algebras, defining the structure as a semiring with a ring homomorphism `algebraMap R A` landing in the center |
| Basic.lean | Further basic results about algebras including instances for `PUnit`, `ULift`, subsemirings/subrings, and fundamental lemmas about `algebraMap` |
| Hom.lean | `AlgHom R A B` - bundled homomorphisms of R-algebras (notation `A →ₐ[R] B`) preserving both ring structure and commuting with `algebraMap` |
| Equiv.lean | `AlgEquiv R A B` - bundled isomorphisms of R-algebras (notation `A ≃ₐ[R] B`) as ring equivalences commuting with scalars |
| NonUnitalHom.lean | `NonUnitalAlgHom R A B` - algebra homomorphisms for non-unital algebras, relaxing the unital requirement |
| NonUnitalSubalgebra.lean | `NonUnitalSubalgebra R A` - subalgebras without unit requirement, defined as substructures that are both non-unital subsemirings and submodules |
| Tower.lean | Algebra tower theory `R → S → A`, including `IsScalarTower` compatibility, canonical algebra homomorphisms between layers, and the `lsmul` representation morphism |
| Operations.lean | Multiplication and division operations on submodules of algebras, making `Submodule R A` into a semiring with pointwise operations and quotient constructions |
| RestrictScalars.lean | `RestrictScalars R S M` - type alias for viewing an S-module as an R-module via an R-algebra structure on S, with equivalences preserving additive/ring structure |
| Bilinear.lean | Bilinear forms and operations on algebras, connecting scalar multiplication with bilinear structures |
| Opposite.lean | Opposite algebra constructions, showing how algebra structures transfer to opposite rings |
| Pi.lean | Product algebra instances for pi types `Π i, A i`, showing how algebra structures work componentwise |
| Prod.lean | Product algebra instances for binary products `A × B` |
| Unitization.lean | `Unitization R A` - minimal unital R-algebra containing non-unital algebra A as an ideal, constructed as `R × A` with modified multiplication `(r₁,a₁)*(r₂,a₂) = (r₁*r₂, r₁•a₂ + r₂•a₁ + a₁*a₂)` |
| Field.lean | Algebra instances and lemmas specific to algebras over fields |
| Rat.lean | Algebra instances for rationals, showing ℚ as an algebra over itself and related structures |
| ZMod.lean | Algebra structures on integers modulo n (`ZMod n`) |
| IsSimpleRing.lean | Properties of simple rings (no nontrivial two-sided ideals) in the context of algebras |
| TransferInstance.lean | Transferring algebra instances via equivalences |
| Shrink.lean | Universe shrinking operations for algebras to manage universe levels |
| StrictPositivity.lean | Integration with the `positivity` tactic for algebra-specific positivity reasoning |

## Subdirectories

- [x] `Hom/` - Specialized theory for algebra homomorphisms, establishing equivalence between ring homomorphisms and ℚ-algebra homomorphisms for rational algebras
- [x] `Spectrum/` - Spectrum and quasispectrum theory for elements in algebras, defining spectrum as scalars where scalar shift yields non-invertible element, with quasispectrum extending to non-unital algebras via quasiregularity and serving as domain for continuous functional calculus
- [x] `Subalgebra/` - Comprehensive theory of subalgebras including complete lattice structure via adjoin operation (minimal subalgebra containing a set), closure operations, maps, centralizers, tower theory with scalar restriction, connections to unitization, pointwise operations, directed suprema, and specialized results for products, opposites, matrices, and rank calculations

## Search Tags

algebra algebraMap algebra-homomorphism algebra-equivalence algebra-tower subalgebra non-unital-algebra unitization restrict-scalars submodule-operations bilinear opposite-algebra product-algebra simple-ring
