---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Cartesian
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 11
subdirs_count: 0
---

# Cartesian

## Overview

The `Cartesian/` directory formalizes Cartesian monoidal categories, which are monoidal categories where the tensor product is given by categorical products and the unit is a terminal object. This includes the core definition via `CartesianMonoidalCategory` (bundling explicit choices of finite products), semicartesian structures where only the unit is terminal, and numerous instances for concrete categories (Cat, Over, functor categories, meet-semilattices). The directory also characterizes internal algebraic objects (monoid, comonoid, commutative monoid, group, commutative group, and module objects) in the Cartesian setting, showing that comonoid objects are equivalent to the category itself via diagonal maps, and establishing Yoneda embeddings for these structured objects.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `SemiCartesianMonoidalCategory` (unit is terminal) and `CartesianMonoidalCategory` (explicit choices of terminal object and binary products); `ofChosenFiniteProducts` constructor; projection maps `fst` and `snd`; pentagon coherence for products; and default braided/symmetric structures |
| Cat.lean | Cartesian monoidal structure on the category `Cat` using categorical products of categories as tensor product and singleton category as unit |
| Over.lean | Cartesian monoidal structure on slice categories `Over X` via pullbacks; includes simp lemmas for tensor objects, associators, unitors; `MonObj`, `GrpObj`, and related instances for objects in `Over X` |
| FunctorCategory.lean | Cartesian monoidal structure on functor categories `J ⥤ C` constructed pointwise from underlying category `C`; chosen terminal functor and chosen product functors |
| Mon_.lean | Characterization of monoid objects in Cartesian monoidal categories via Yoneda embedding `Mon C ⥤ Cᵒᵖ ⥤ MonCat`; shows monoid objects correspond to presheaves of monoids; instances for `IsMonHom` on projections, lifts, and unit maps; Cartesian structure on `Mon C` itself when `C` is braided |
| Grp_.lean | Group objects in Cartesian categories via Yoneda embedding `Grp C ⥤ Cᵒᵖ ⥤ GrpCat`; construction of `GrpObj` from representable presheaf of groups with inverses; `Grp.homMk` helper for morphisms |
| Comon_.lean | Comonoid objects in Cartesian categories are equivalent to the category itself (`comonEquiv : Comon C ≌ C`) via forgetful functor; every object has canonical comonoid structure with diagonal comultiplication; simplification lemmas showing `comul = lift (𝟙 _) (𝟙 _)` and `counit = toUnit` |
| CommMon_.lean | Commutative monoid objects characterized via Yoneda: `IsCommMonObj.ofRepresentableBy` shows objects representing presheaves of commutative monoids are commutative monoid objects |
| CommGrp_.lean | Commutative group objects in braided Cartesian categories (imports only, minimal additional content) |
| Mod_.lean | Module objects in Cartesian categories; `ModObj.trivialAction` showing every object is a module over any monoid object via the trivial action (second projection) |
| InfSemilattice.lean | Cartesian monoidal structure on preorder categories of meet-semilattices with top element (`SemilatticeInf` with `OrderTop`), where tensor is meet (`⊗ = ⊓`) and unit is top (`𝟙_ C = ⊤`) |

## Subdirectories

*(None)*

## Search Tags

cartesian-monoidal-categories chosen-finite-products semicartesian products terminal-object yoneda-embedding monoid-objects comonoid-objects group-objects commutative-monoid module-objects functor-categories slice-categories over-categories cat diagonal-map lift-operations cartesian-closed meet-semilattices preorder-categories
