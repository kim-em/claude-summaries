---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/RingedSpace/PresheafedSpace
generated: 2026-01-24T21:30:00Z
git_sha: cb392c137f92523b6c137ee117b3ee1a2c245230
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# PresheafedSpace

## Overview

This directory contains advanced constructions for the category of presheafed spaces: gluing theory and colimits. The gluing file provides a comprehensive framework for gluing presheafed spaces, sheafed spaces, and locally ringed spaces together along open immersions, which is a fundamental operation in algebraic geometry (needed for constructing schemes by gluing affine schemes). The colimits file establishes that the category of presheafed spaces has colimits when the base category has limits, with the forgetful functor to TopCat preserving these colimits.

## Key Files

| File | Purpose |
|------|---------|
| Gluing.lean | Comprehensive gluing theory for presheafed, sheafed, and locally ringed spaces via open immersions; defines `GlueData` structures and proves that glued spaces satisfy universal properties including open immersion of components and pullback diagrams |
| HasColimits.lean | Proves that `PresheafedSpace C` has colimits when `C` has limits; colimits are computed by taking the colimit of underlying topological spaces and the limit of pushforward presheaves |

## Subdirectories

No subdirectories.

## Search Tags

gluing glue-data presheafed-space sheafed-space locally-ringed-space open-immersion colimits category-theory multicoequalizer algebraic-geometry scheme-construction pullback-cone pushforward componentwise-diagram limits topological-colimit sheaf-gluing intersection-of-opens jointly-surjective universal-property
