---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/RingedSpace/LocallyRingedSpace
generated: 2026-01-24T19:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# LocallyRingedSpace

## Overview

This directory contains additional constructions for locally ringed spaces beyond those in the parent `LocallyRingedSpace.lean` file. It provides two key pieces of categorical and algebraic infrastructure: the existence of all colimits in the category of locally ringed spaces (coproducts and coequalizers), and the theory of residue fields at points. These are essential for algebraic geometry, where colimits enable gluing constructions and residue fields connect geometric points to their local algebraic structure.

## Key Files

| File | Purpose |
|------|---------|
| HasColimits.lean | Proves `LocallyRingedSpace` has all colimits by constructing explicit coproducts and coequalizers; shows the forgetful functor to `SheafedSpace` preserves colimits |
| ResidueField.lean | Defines the residue field at a point (quotient of stalk by its maximal ideal); provides evaluation maps from sections to residue fields and functorial residue field maps for morphisms |

## Subdirectories

*(none)*

## Search Tags

locally-ringed-space colimit coproduct coequalizer residue-field stalk local-ring evaluation-map algebraic-geometry category-theory sheafed-space forgetful-functor germ basic-open
