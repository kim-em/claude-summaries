---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Condensed/Light
generated: 2025-12-08T15:52:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 14
subdirs_count: 0
---

# Light

## Overview

The `Light/` subdirectory implements light condensed mathematics, a variant of condensed mathematics where objects are defined as sheaves on the essentially small category `LightProfinite` instead of the large category `CompHaus`. This provides a more tractable framework without universe bumps, as light profinite spaces are countable Stone spaces. The implementation includes the core category `LightCondensed C` and `LightCondSet`, their module-theoretic variants with abelian category structure, explicit sheaf conditions via finite-product preservation and equalizer conditions, characterizations of epimorphisms and internal projectivity, monoidal and cartesian closed structures, and adjunctions with topological spaces (fully faithful when restricted to sequential spaces).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of light condensed objects as sheaves on `LightProfinite` with coherent topology; defines `LightCondensed C` and `LightCondSet` (without universe bump) with basic category infrastructure |
| Module.lean | Light condensed R-modules `LightCondMod R` as sheaves of modules over `LightProfinite`; proves they form an abelian category; defines free-forgetful adjunction and light condensed abelian groups `LightCondAb` |
| Explicit.lean | Explicit sheaf conditions for light condensed objects: `ofSheafLightProfinite` constructs light condensed objects from presheaves on `LightProfinite` preserving finite products and satisfying `EqualizerCondition` |
| AB.lean | Proof that light condensed R-modules satisfy the countable version of Grothendieck's AB4* axiom (`CountableAB4Star`) and form a Grothendieck abelian category |
| Epi.lean | Characterization of epimorphisms in light condensed sets and modules as locally surjective morphisms (phrased via continuous surjections of light profinite sets); proves sequential product limits preserve epimorphisms |
| InternallyProjective.lean | Explicit tensor-product characterization of internally projective light condensed modules: `P` is internally projective iff lifting problems `P ⊗ R[S] → B` along epimorphisms can be solved after pulling back along a surjection `S' → S` (300 lines, includes variants for free modules) |
| Monoidal.lean | Closed symmetric monoidal structure on light condensed modules by localizing the presheaf monoidal structure; uses Day's reflection theorem to obtain closed structure |
| Functors.lean | Functor `lightProfiniteToLightCondSet : LightProfinite ⥤ LightCondSet` as the Yoneda sheaf functor; proves it's fully faithful, monoidal, and preserves countable/finite limits; factorization through `TopCat` |
| TopComparison.lean | Functor `topCatToLightCondSet : TopCat.{u} ⥤ LightCondSet.{u}` via Yoneda presheaf, embedding u-small topological spaces into light condensed sets |
| TopCatAdjunction.lean | Adjunction `lightCondSetToTopCat ⊣ topCatToLightCondSet` with counit always bijective (but not continuous inverse in general); restriction to sequential spaces yields fully faithful functor (208 lines) |
| Limits.lean | Limit constructions in light condensed sets and modules: instances for `HasLimitsOfSize` and `HasFiniteLimits` |
| Instances.lean | Sheafification instances `HasSheafify (coherentTopology LightProfinite.{u}) A` obtained via essential smallness of `LightProfinite`; proves `WEqualsLocallyBijective` for concrete categories |
| Small.lean | Equivalence `equivSmall` between light condensed objects and sheaves on a small site equivalent to `LightProfinite`; proves morphism sets are small; compatibility of sheafification and free module functors under this equivalence |
| CartesianClosed.lean | Proves light condensed sets form a cartesian closed category (inheriting from sheaf category structure) |

## Subdirectories

_(none)_

## Search Tags

light-condensed-mathematics sheaf-theory light-profinite coherent-topology clausen-scholze countable-stone-spaces abelian-category module-theory grothendieck-axioms AB4-star internal-projectivity tensor-products monoidal-closed cartesian-closed epimorphisms locally-surjective explicit-sheaf-condition equalizer-condition sequential-spaces topological-adjunction yoneda-embedding essentially-small-site
