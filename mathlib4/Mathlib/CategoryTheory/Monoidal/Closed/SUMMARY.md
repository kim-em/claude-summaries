---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Closed
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 9
subdirs_count: 1
---

# Closed

## Overview

The `Closed/` directory implements the theory of closed monoidal categories—categories where each object `X` has an "internal hom" functor `X ⟹ -` that is right adjoint to tensoring with `X`. This generalizes the notion of function spaces/exponentials to arbitrary monoidal categories. The directory provides both the general framework for monoidal closed categories and specializations to Cartesian closed categories (where the tensor is the product), including curry/uncurry operations, exponential comparison for functors, and enrichment structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of closed objects and monoidal closed categories with internal hom functor `ihom`, curry/uncurry operations, evaluation and coevaluation natural transformations, and enrichment structure |
| Cartesian.lean | Cartesian closed categories where closed structure uses products instead of tensor, defining exponentiable objects and exponential functors with notation `A ⟹ B` |
| Functor.lean | Cartesian closed functors and exponential comparison maps, Frobenius morphism relating preservation of products to preservation of exponentials |
| Ideal.lean | Exponential ideals: reflective subcategories where `B ∈ D` implies `A ⟹ B ∈ D`, with equivalence to reflector preserving binary products |
| Enrichment.lean | Scoped instance making any monoidal closed category enriched over itself using internal hom as hom-objects |
| FunctorToTypes.lean | Proof that functor categories `C ⥤ Type` are monoidal closed using `functorHom` as the internal hom |
| Transport.lean | Transport of monoidal closed structure along categorical equivalences |
| Types.lean | Proof that `Type` and presheaf categories are Cartesian closed using coyoneda as exponential |
| Zero.lean | Proof that any Cartesian closed category with a zero object is trivial (equivalent to the terminal category) |

## Subdirectories

- [x] `FunctorCategory/` - Additional constructions for closed structures on functor categories

## Search Tags

closed-monoidal-categories internal-hom exponentials cartesian-closed exponentiable-objects curry uncurry evaluation coevaluation adjunction enrichment functor-categories exponential-comparison frobenius-morphism exponential-ideals reflective-subcategories transport type-theory presheaves zero-object
