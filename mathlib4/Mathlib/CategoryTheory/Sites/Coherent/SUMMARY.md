---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Sites/Coherent
generated: 2025-12-08T14:36:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 15
subdirs_count: 0
---

# Coherent

## Overview

The `Coherent/` directory contains the formalization of coherent, regular, and extensive Grothendieck topologies along with their associated sheaves and structural properties. These three related topologies arise from different categorical conditions on effective epimorphic families: coherent (finite effective epi families pullback), regular (single effective epis pullback), and extensive (finite coproducts preserved by pullbacks). The directory provides complete characterizations of covering sieves, sheaf conditions via equalizer diagrams or finite product preservation, equivalences between sheaf categories under various functors, and specialized results including preservation of locally surjective/bijective properties, sequential limits of epimorphisms, and relationships between the three topologies (extensive + regular generates coherent).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `Precoherent`, `Preregular`, `FinitaryPreExtensive` classes and their corresponding coverages and topologies (coherent, regular, extensive) |
| CoherentTopology.lean | Characterization of coherent topology covering sieves: sieve covers iff contains finite effective epi family |
| CoherentSheaves.lean | Sheaf condition for coherent topology: presheaf is sheaf iff satisfies sheaf condition for all finite effective epi families; coherent topology is subcanonical |
| RegularTopology.lean | Characterization of regular topology covering sieves: sieve covers iff contains effective epi; stability of effective epis under composition |
| RegularSheaves.lean | Sheaf condition for regular topology via equalizer diagrams: `EqualizerCondition` characterizes sheaves; every presheaf is sheaf when all objects projective |
| ExtensiveTopology.lean | Characterization of extensive topology covering sieves: sieve covers iff contains finite family exhibiting target as coproduct |
| ExtensiveSheaves.lean | Sheaf condition for extensive topology: presheaf is sheaf iff preserves finite products |
| ExtensiveColimits.lean | Colimit properties in extensive categories |
| Comparison.lean | Relationships between topologies: `Precoherent` implies `Preregular` with finite coproducts; `FinitaryPreExtensive + Preregular` implies `Precoherent`; extensive ⊔ regular generates coherent |
| Equivalence.lean | Preservation under categorical equivalence: `Precoherent` and `Preregular` preserved by equivalences; equivalences of sites induce equivalences of sheaf categories |
| SheafComparison.lean | Major equivalence theorem: for fully faithful functor F : C → D preserving/reflecting effective epi families with `EffectivelyEnough`, coherent sheaves on C and D equivalent; regular topology version; coherent sheaf iff preserves finite products and satisfies equalizer condition |
| LocallySurjective.lean | Characterization of locally surjective morphisms: for regular topology, locally surjective iff locally lifts to effective epi; for coherent topology in preregular extensive categories, same as regular; for extensive topology, locally surjective iff objectwise surjective |
| SequentialLimit.lean | Limits of epimorphisms: sequential limit of epimorphisms is epimorphic in coherent topoi (under hypotheses: preregular, finitary extensive, sequential limits of effective epis are effective) |
| ReflectsPrecoherent.lean | Functors reflecting the precoherent property |
| ReflectsPreregular.lean | Functors reflecting the preregular property |

## Subdirectories

_(no subdirectories)_

## Search Tags

coherent-topology regular-topology extensive-topology precoherent preregular finitary-extensive effective-epimorphic-families covering-sieves sheaf-conditions equalizer-condition finite-products grothendieck-topology subcanonical locally-surjective locally-bijective dense-subsite sheaf-equivalences pullback-stability topos-theory condensed-mathematics
