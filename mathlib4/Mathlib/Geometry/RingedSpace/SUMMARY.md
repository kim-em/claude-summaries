---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/RingedSpace
generated: 2026-01-24T21:35:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 2
---

# RingedSpace

## Overview

The `RingedSpace/` directory provides the complete foundational categorical infrastructure for algebraic geometry, building a hierarchy of spaces equipped with sheaves of rings. It defines presheafed spaces (topological spaces with presheaves), sheafed spaces (where the presheaf is actually a sheaf), ringed spaces (sheafed spaces with commutative ring-valued sheaves), and locally ringed spaces (where all stalks are local rings). The core files establish morphisms, restrictions, global sections, open immersions, stalks, units in germs, and basic opens. The subdirectories provide essential categorical constructions: gluing theory for assembling spaces from components via open immersions (critical for scheme construction), colimit existence in presheafed and locally ringed space categories, and the theory of residue fields at points. Together, this forms the complete categorical foundation needed to define and work with schemes in algebraic geometry.

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

- [x] `LocallyRingedSpace/` - Categorical constructions (colimits, coproducts, coequalizers) and algebraic theory (residue fields at points, evaluation maps) for locally ringed spaces
- [x] `PresheafedSpace/` - Gluing theory for assembling presheafed/sheafed/locally ringed spaces via open immersions; colimit existence in PresheafedSpace category

## Search Tags

ringed-space locally-ringed-space sheafed-space presheafed-space algebraic-geometry sheaf-of-rings stalk local-ring open-immersion basic-open zero-locus global-sections morphism-of-ringed-spaces pullback restriction scheme-foundation category-theory commutative-ring
