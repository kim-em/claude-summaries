---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Condensed
generated: 2025-12-08T20:05:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 12
subdirs_count: 2
---

# Condensed

## Overview

The `Condensed/` directory implements condensed mathematics, a modern categorical framework introduced by Clausen-Scholze that unifies continuous and discrete mathematics through sheaves on compact Hausdorff spaces. The implementation defines condensed objects as sheaves on `CompHaus` with the coherent Grothendieck topology, establishes categorical equivalences with sheaves on `Stonean` and `Profinite` spaces, and provides explicit sheaf conditions via finite-product preservation and equalizer conditions. The directory includes specialized support for condensed sets, condensed modules (which form an abelian category satisfying Grothendieck's AB axioms), and solid modules. Two important specializations are developed in subdirectories: **discrete condensed objects** provide functorial relationships between ordinary categories and their condensed counterparts via adjunctions (discrete ⊣ underlying), with characterizations through locally constant functors and colimit preservation; **light condensed objects** offer a universe-efficient variant using sheaves on the essentially small category `LightProfinite` (countable Stone spaces), with full abelian structure, internal projectivity characterizations, monoidal/cartesian closed structures, and adjunctions with topological spaces.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of condensed objects as sheaves on `CompHaus` with coherent topology; defines `Condensed C` and `CondensedSet` with basic category infrastructure |
| Module.lean | Condensed R-modules as sheaves of modules over CompHaus; proves they form an abelian category with free-forgetful adjunction; defines condensed abelian groups as condensed Z-modules |
| Equivalence.lean | Categorical equivalences between sheaves on Stonean/Profinite/CompHaus: `StoneanCompHaus.equivalence`, `ProfiniteCompHaus.equivalence`, exploiting Stonean as dense subsite |
| Explicit.lean | Explicit sheaf conditions for condensed objects via three equivalent characterizations: finite-product-preserving presheaves on Stonean, Profinite (with equalizer condition), or CompHaus (with equalizer condition) |
| AB.lean | Proof that condensed R-modules satisfy Grothendieck's axioms AB5, AB4, and AB4* using coherent-extensive topology equivalence and exact colimit/limit preservation |
| TopComparison.lean | Functor `topCatToCondensedSet : TopCat.{u+1} ⥤ CondensedSet.{u}` via Yoneda presheaf; proves equalizer and finite product preservation conditions for sheafification |
| TopCatAdjunction.lean | Adjunction between condensed sets and topological spaces (210 lines) |
| Epi.lean | Characterization of epimorphisms in condensed sets and condensed modules as objectwise surjective morphisms on Stonean |
| Solid.lean | Definition of solid modules (`CondensedMod.IsSolid R`), a key notion from Scholze's condensed mathematics (with TODOs for proving profinite solidity results) |
| Functors.lean | Functors between categories of condensed objects and related constructions (82 lines) |
| Limits.lean | Limit constructions in categories of condensed objects (55 lines) |
| CartesianClosed.lean | Cartesian closed structure on condensed objects (29 lines) |

## Subdirectories

- [x] `Discrete/` - Discrete condensed objects: functorial relationships between ordinary categories and condensed counterparts via adjunctions (discrete ⊣ underlying); characterizations through locally constant functors, colimit preservation, and 5-7 equivalent TFAE conditions; applies to condensed sets, modules, and light variants
- [x] `Light/` - Light condensed objects as sheaves on essentially small `LightProfinite` (countable Stone spaces) without universe bumps; includes abelian category structure with AB4* axioms, internal projectivity via tensor products, monoidal/cartesian closed structures, epimorphism characterizations, explicit sheaf conditions, and fully faithful adjunction with sequential topological spaces

## Search Tags

condensed-mathematics sheaf-theory compact-hausdorff grothendieck-topology coherent-topology clausen-scholze stonean-spaces profinite category-theory abelian-category module-theory solid-modules dense-subsite effective-epimorphism yoneda-presheaf categorical-equivalence AB-axioms discrete-condensed light-condensed
