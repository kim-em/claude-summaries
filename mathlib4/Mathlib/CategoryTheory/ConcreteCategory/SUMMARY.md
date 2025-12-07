---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/ConcreteCategory
generated: 2025-12-07T08:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# ConcreteCategory

## Overview

The `ConcreteCategory/` directory provides the foundational infrastructure for concrete categories in mathlib4—categories where objects correspond to types and morphisms correspond to functions between those types. It defines the `ConcreteCategory` and `HasForget` typeclasses that equip a category with a faithful forgetful functor to `Type`, establishes the relationship between categorical properties (epimorphisms, monomorphisms, isomorphisms) and their set-theoretic counterparts (surjections, injections, bijections), and provides utilities for working with bundled types (types equipped with structure). This infrastructure serves as the bridge between abstract categorical reasoning and concrete mathematical structures like groups, rings, topological spaces, and modules.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of concrete categories: `HasForget` class providing faithful functor to `Type`, `HasForget₂` for composable forgetful functors between concrete categories, `ConcreteCategory` typeclass, pointwise morphism equality (`hom_ext`), and basic lemmas about composition and identity in concrete categories |
| Bundled.lean | `Bundled c` structure for uniformly bundling a type with a typeclass instance, providing foundation for defining categories of structured types (will be deprecated in favor of manual category definitions with `ConcreteCategory` instances) |
| BundledHom.lean | Infrastructure for concrete categories using bundled homomorphisms (e.g. `MonoidHom`, `RingHom`): `BundledHom` class capturing functorial properties of bundled hom types, automatic `Category` and `HasForget` instances for `Bundled c` (deprecated in favor of manual implementations) |
| UnbundledHom.lean | Infrastructure for concrete categories using unbundled homomorphisms (bare functions with typeclasses like `IsContinuous`): `UnbundledHom` class for predicates on functions preserving structure, bridge to `BundledHom` via `Subtype` (deprecated in favor of manual implementations) |
| EpiMono.lean | Relationships between categorical and set-theoretic properties in concrete categories: injective morphisms are monomorphisms, surjective morphisms are epimorphisms, characterization of when these coincide, preservation of epi/mono by forgetful functors, functorial factorization into surjection followed by injection |
| Elementwise.lean | Simp lemmas in elementwise form using the `elementwise` tactic attribute, providing pointwise versions of categorical equations for limits, colimits, kernels, and cokernels in concrete categories |
| ReflectsIso.lean | Proof that forgetful functors `forget₂ C D` between concrete categories reflect isomorphisms when the ultimate forgetful functor to `Type` reflects isomorphisms, ensuring that isomorphisms can be detected at the underlying type level |

## Subdirectories

*(No subdirectories)*

## Search Tags

concrete-categories forgetful-functors faithful-functors bundled-types structured-types category-instances algebraic-structures topological-structures epimorphisms monomorphisms surjective injective bijective isomorphism-reflection bundled-homs unbundled-homs elementwise-reasoning
