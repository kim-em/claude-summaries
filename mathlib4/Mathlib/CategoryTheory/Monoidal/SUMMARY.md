---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 89
subdirs_count: 14
---

# Monoidal

## Overview

The `Monoidal/` directory contains the comprehensive formalization of monoidal category theory in mathlib4. It implements monoidal categories (categories equipped with tensor products, associators, and unitors), monoidal functors and natural transformations, internal algebraic structures (monoid, comonoid, bimonoid, and Hopf objects), braided and symmetric monoidal structures, closed monoidal categories, and specialized constructions including Day convolution, the Drinfeld center, and rigid monoidal categories. This framework provides the categorical foundation for tensor categories, representation theory, quantum algebra, and other areas requiring monoidal structure.

## Key Files

| File | Purpose |
|------|---------|
| Category.lean | Core definition of monoidal categories with tensor product, associator, unitors, and coherence axioms |
| Functor.lean | Lax, oplax, and strong monoidal functors with unit and tensorator morphisms |
| NaturalTransformation.lean | Monoidal natural transformations between monoidal functors with compatibility conditions |
| Mon_.lean | Monoid objects in monoidal categories with unit and multiplication morphisms |
| Comon_.lean | Comonoid objects with counit and comultiplication, dual to monoid objects |
| Bimon_.lean | Bimonoid objects combining monoid and comonoid structures with compatibility |
| Hopf_.lean | Hopf monoids in braided categories with antipode maps |
| Grp_.lean | Group objects in monoidal categories (monoids with inverses) |
| CommMon_.lean | Commutative monoid objects in braided monoidal categories |
| CommGrp_.lean | Commutative group objects combining commutativity and inverses |
| Mod_.lean | Module objects over monoid objects (left/right actions) |
| Bimod.lean | Bimodule objects over pairs of monoid objects with compatible left/right actions |
| CommComon_.lean | Commutative comonoid objects in braided categories |
| Center.lean | Drinfeld center construction producing braided monoidal category from half-braidings |
| DayConvolution.lean | Day convolution monoidal structure on functor categories via left Kan extensions |
| End.lean | Monoidal category structure on endofunctor categories with composition as tensor |
| FunctorCategory.lean | Pointwise monoidal structure on functor categories `C ⥤ D` when `D` is monoidal |
| Opposite.lean | Monoidal structure on opposite categories with reversed tensor order |
| Discrete.lean | Monoidal structure on discrete categories from commutative monoids |
| Skeleton.lean | Monoidal structure on skeletal subcategories |
| Subcategory.lean | Full monoidal subcategories preserving monoidal structure |
| Transport.lean | Transporting monoidal structures along equivalences of categories |
| Linear.lean | Linear monoidal categories (monoidal enriched over modules) |
| Preadditive.lean | Preadditive monoidal categories with additive hom-groups compatible with tensor |
| OfHasFiniteProducts.lean | Constructing Cartesian monoidal structure from finite products |
| Multifunctor.lean | Multifunctors (functors of multiple variables) in monoidal categories |
| CoherenceLemmas.lean | Consequences of monoidal coherence including `λ_ (𝟙_ C) = ρ_ (𝟙_ C)` |
| Conv.lean | Convolution structures for bimonoid morphisms |
| Tor.lean | Torsors in monoidal categories |
| Limits.lean | Import for limits in monoidal categories |
| ExternalProduct.lean | External tensor products between different monoidal categories |
| Yoneda.lean | Yoneda embedding for monoidal categories |

## Subdirectories

- [x] `Action/` - Actions of monoidal categories on arbitrary categories with coherence axioms
- [ ] `Braided/` - Braided and symmetric monoidal categories (pending)
- [ ] `Cartesian/` - Cartesian monoidal categories from products (pending)
- [ ] `Closed/` - Closed monoidal categories with internal hom (pending)
- [ ] `DayConvolution/` - Additional Day convolution constructions (pending)
- [ ] `ExternalProduct/` - External product functors and constructions (pending)
- [ ] `Free/` - Free monoidal categories (pending)
- [ ] `Functor/` - Additional monoidal functor properties (pending)
- [ ] `Internal/` - Internal structures in monoidal categories (pending)
- [ ] `Limits/` - Limits and colimits in monoidal categories (pending)
- [ ] `OfChosenFiniteProducts/` - Monoidal structure from explicitly chosen products (pending)
- [ ] `Opposite/` - Additional opposite category constructions (pending)
- [ ] `Rigid/` - Rigid monoidal categories with duals (pending)
- [ ] `Types/` - Monoidal structure on Type category (pending)

## Search Tags

monoidal-categories tensor-products monoidal-functors monoid-objects comonoid-objects bimonoid-objects hopf-algebras braided-monoidal symmetric-monoidal closed-monoidal rigid-monoidal day-convolution drinfeld-center internal-hom cartesian-monoidal coherence monoidal-natural-transformations module-objects action-categories representation-theory quantum-algebra
