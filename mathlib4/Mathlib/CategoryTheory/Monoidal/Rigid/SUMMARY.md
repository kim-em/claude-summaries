---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Rigid
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Rigid

## Overview

The `Rigid/` directory formalizes rigid (autonomous) monoidal categories, where every object has left and right duals connected by exact pairings with coevaluation and evaluation morphisms satisfying triangle identities. It defines the core theory of exact pairings, adjoint mates, and type classes for objects with duals, then extends this structure to braided categories (where left/right duals coincide), functor categories from groupoids, and provides transport mechanisms for pulling back rigid structures along monoidal equivalences.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `ExactPairing`, `HasLeftDual`/`HasRightDual` classes, adjoint mates (`fᘁ` and `ᘁf`), tensor hom equivalences (Frobenius reciprocity), adjunctions `tensorLeft Y' ⊣ tensorLeft Y`, and `RightRigidCategory`/`LeftRigidCategory`/`RigidCategory` type classes |
| Braided.lean | Derives `RigidCategory` instances for braided categories that are left or right rigid, proving that exact pairings can be swapped using braiding morphisms (`exactPairing_swap`) |
| FunctorCategory.lean | Proves functor categories `C ⥤ D` from groupoids `C` into rigid categories `D` inherit rigid structure pointwise using adjoint mates of inverse morphisms |
| OfEquivalence.lean | Transport rigid structures along monoidal equivalences: `ExactPairing.ofFaithful`, `ExactPairing.ofFullyFaithful`, and pullback constructions for left/right/rigid category instances |

## Subdirectories

*(No subdirectories)*

## Search Tags

rigid-categories autonomous-categories exact-pairings left-dual right-dual adjoint-mate coevaluation evaluation tensor-adjunctions frobenius-reciprocity braided-rigid functor-categories monoidal-equivalence transport-structure category-theory monoidal-categories
