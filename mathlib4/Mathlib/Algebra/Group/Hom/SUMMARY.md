---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Hom
generated: 2025-12-01T20:00:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# Hom

## Overview

The `Hom/` directory contains the complete definition of bundled homomorphisms for group-like algebraic structures and their supporting theory. It defines the fundamental homomorphism types (`ZeroHom`, `OneHom`, `AddHom`, `MulHom`, `AddMonoidHom`, `MonoidHom`) along with their corresponding typeclass hierarchies (`ZeroHomClass`, `OneHomClass`, etc.) that enable polymorphic reasoning over homomorphisms. The directory provides the core infrastructure for working with structure-preserving maps in the algebraic hierarchy, including composition, identity maps, pointwise operations, algebraic instances on homomorphism spaces, and typeclasses for tracking composition relationships.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core bundled homomorphism definitions and typeclass hierarchy; defines `ZeroHom`, `OneHom`, `AddHom`, `MulHom`, `AddMonoidHom`, `MonoidHom` along with their `*HomClass` typeclasses; includes fundamental lemmas like `map_one`, `map_mul`, `map_zero`, `map_add` with performance-optimized simp priorities; establishes notation `→+` (AddMonoidHom), `→*` (MonoidHom), `→ₙ+` (AddHom), `→ₙ*` (MulHom) |
| Basic.lean | Additional lemmas and operations on homomorphisms; defines power homomorphisms (`powMonoidHom`, `zpowGroupHom`), inversion homomorphism (`invMonoidHom`), pointwise multiplication/addition/inversion on homomorphism spaces (`OneHom` has `Mul` and `Inv` instances), and composition properties |
| Instances.lean | Algebraic structure instances on homomorphism spaces; provides `Monoid`, `CommMonoid`, `Group`, `CommGroup` instances on `OneHom M N` when `N` has appropriate structure; similarly for additive versions; defines `SMul ℕ` and `Pow ℕ` instances; crucially provides `Ring` structure on `AddMonoid.End` |
| CompTypeclasses.lean | Typeclasses for tracking homomorphism composition relationships; defines `MonoidHom.CompTriple φ ψ χ` expressing that `ψ.comp φ = χ`, and `MonoidHom.IsId φ` expressing that `φ = id`; used for equivariant map infrastructure; includes composition associativity and identity properties |
| End.lean | Ring structure on endomorphism monoids; provides `AddMonoidWithOne`, `Semiring`, and `Ring` instances for `AddMonoid.End M` (the type of additive monoid endomorphisms); includes natural number and integer casting as scalar multiplication by identity |

## Subdirectories

(none)

## Search Tags

homomorphism monoid-hom group-hom additive-hom bundled-morphism funlike oneHom mulHom addMonoidHom monoidHom homClass map-one map-mul composition endomorphism ring-structure pointwise-operations equivariant to-additive
