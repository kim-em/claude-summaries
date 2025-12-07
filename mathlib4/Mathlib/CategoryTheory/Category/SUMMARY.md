---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Category
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 18
subdirs_count: 1
---

# Category

## Overview

The `Category/` directory contains fundamental category instances and constructions that demonstrate how various mathematical structures can be viewed as categories. This includes the basic definition of categories themselves, several concrete category instances (categories of categories, groupoids, quivers, pointed types, preorders, relations), and important categorical constructions (Kleisli categories, ULift universe adjustments, factorization categories). These files establish the foundational examples and patterns that the rest of the category theory library builds upon.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of the `Category` typeclass with morphisms, identity, and composition; establishes notation `⟶`, `𝟙`, `≫` |
| Init.lean | Aesop rule set declaration for category theory tactics (`aesop_cat`, `cat_disch`) and options for using grind vs aesop |
| Cat.lean | Category `Cat` of categories where objects are categories and morphisms are functors |
| Grpd.lean | Category `Grpd` of groupoids with functors as morphisms; includes forgetful functor to `Cat` |
| Quiv.lean | Category `Quiv` of quivers with prefunctors; establishes free/forgetful adjunction between `Cat` and `Quiv` |
| ReflQuiv.lean | Category `ReflQuiv` of reflexive quivers; free/forgetful adjunction between `Cat` and `ReflQuiv` |
| Pointed.lean | Category `Pointed` of types with a distinguished point; morphisms preserve basepoints |
| Bipointed.lean | Category `Bipointed` of types with two distinguished points |
| TwoP.lean | Category `TwoP` of two-pointed types with distinct points (coalgebra of real interval) |
| Preorder.lean | Category instance on preorders where morphisms are `ULift (PLift (X ≤ Y))`; monotone functions as functors |
| RelCat.lean | Category `RelCat` of types with binary relations as morphisms; includes graph functor and opposite equivalence |
| PartialFun.lean | Category `PartialFun` with partial functions as morphisms; classically equivalent to pointed types |
| Pairwise.lean | Diagram category `Pairwise ι` for pairwise intersections; used in sheaf condition formulations |
| ULift.lean | Category instance on `ULift C` with universe lifting; functors `upFunctor`, `downFunctor`, and equivalence; includes `AsSmall` construction |
| KleisliCat.lean | Kleisli category construction for (control) monads on `Type` |
| Factorisation.lean | Category of factorizations of a morphism with initial and terminal objects |
| GaloisConnection.lean | Galois connections between preorders as adjunctions; converts between order-theoretic and categorical perspectives |

## Subdirectories

- [ ] `Cat/` - Additional constructions and properties for the category of categories (pending)

## Search Tags

category-instances concrete-categories cat grpd quivers pointed-types preorder-categories relations kleisli-category universe-lifting factorizations galois-connections category-definition morphisms functors groupoids partial-functions bipointed-types
