---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/RingedSpace
generated: 2026-01-24T18:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: preliminary
files_count: 6
subdirs_count: 2
---

# RingedSpace

## Overview

The `RingedSpace/` directory provides the foundational categorical infrastructure for algebraic geometry, building a hierarchy of spaces equipped with sheaves of rings. It defines presheafed spaces (topological spaces with presheaves), sheafed spaces (where the presheaf is actually a sheaf), ringed spaces (sheafed spaces with commutative ring-valued sheaves), and locally ringed spaces (where all stalks are local rings). The directory also includes the theory of open immersions, stalks, and basic open sets, forming the categorical foundation needed to define schemes.

## Key Files

| File | Purpose |
|------|---------|
| PresheafedSpace.lean | Defines the category of topological spaces equipped with presheaves; includes morphisms, restrictions, global sections functor |
| SheafedSpace.lean | Defines sheafed spaces (presheafed spaces where the presheaf is a sheaf); includes forgetful functors, restrictions, colimit constructions |
| Basic.lean | Defines ringed spaces as `SheafedSpace CommRingCat`; proves key lemmas about units in germs, basic opens, and zero loci |
| LocallyRingedSpace.lean | Defines locally ringed spaces (stalks are local rings) and their morphisms (stalk maps are local ring homomorphisms); includes restrictions, global sections, and isomorphisms |
| OpenImmersion.lean | Comprehensive theory of open immersions for presheafed, sheafed, and locally ringed spaces; includes pullbacks, lifting properties, and stability under base change |
| Stalks.lean | Stalk maps for morphisms of presheafed spaces; restriction isomorphisms showing restriction doesn't change stalks |

## Subdirectories

- [?] `LocallyRingedSpace/` - Additional constructions for locally ringed spaces: colimits and residue fields
- [?] `PresheafedSpace/` - Additional constructions for presheafed spaces: gluing and colimits

## Search Tags

ringed-space locally-ringed-space sheafed-space presheafed-space algebraic-geometry sheaf-of-rings stalk local-ring open-immersion basic-open zero-locus global-sections morphism-of-ringed-spaces pullback restriction scheme-foundation category-theory commutative-ring
