---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Sites/Point
generated: 2025-12-08T14:41:23Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# Point

## Overview

The `Point/` directory defines the notion of points of a Grothendieck site `(C, J)` as geometric morphisms from the category of sets. A point consists of a fiber functor `C ⥤ Type w` whose category of elements is cofiltered (ensuring exactness) and initially small (allowing colimit constructions), with the property that covering sieves induce jointly surjective maps on fibers. This formalization follows SGA 4 IV 6.3's definition of fiber functors. The file establishes that points induce exact functors on both presheaf and sheaf categories that commute with limits and colimits, and that these fiber functors invert locally bijective morphisms, showing that the fiber of a presheaf identifies with the fiber of its associated sheaf.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `GrothendieckTopology.Point` structure with fiber functor, proves fiber functors on presheaves/sheaves preserve limits and colimits, establishes that locally bijective morphisms become bijections on fibers, and shows sheaf fiber functor is obtained from presheaf fiber functor by localization with respect to locally bijective morphisms (class `J.W`) |

## Subdirectories

(none)

## Search Tags

grothendieck-topology points fiber-functor cofiltered locally-bijective geometric-morphism sheaf-theory topos-theory presheaf-fiber sheaf-fiber localization sga4 covering-sieves jointly-surjective filtered-colimits exact-functor initial-small category-of-elements
