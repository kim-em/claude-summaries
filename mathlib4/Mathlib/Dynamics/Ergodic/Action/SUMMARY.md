---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics/Ergodic/Action
generated: 2026-01-24T10:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Action

## Overview

The `Action/` directory formalizes ergodicity for group and monoid actions on measure spaces. It defines the `ErgodicSMul` and `ErgodicVAdd` typeclasses for actions where a.e.-invariant sets are either null or conull, proves that a group's left and right regular actions on itself are ergodic, and establishes that scalar multiplication by elements with dense powers yields ergodic maps. The directory also connects ergodic actions to minimal actions, showing that minimal group actions on compact spaces imply ergodicity with respect to Haar measure.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `ErgodicSMul` and `ErgodicVAdd` typeclasses for ergodic group/monoid actions; provides theorems showing a.e. invariant sets under ergodic actions are null or conull; proves equivalence between `ErgodicSMul` for `IterateMulAct` and `Ergodic` for the underlying map |
| Regular.lean | Proves that the left regular action (`g • x = g * x`) and right regular action of a group on itself are ergodic with respect to left/right invariant measures |
| OfMinimal.lean | Proves ergodicity from minimality: if powers of an element are dense in a monoid acting continuously on a space with ergodic action, then scalar multiplication by that element is ergodic; shows the converse for topological groups; proves surjective endomorphisms with dense identity preimages are ergodic |

## Subdirectories

*None*

## Search Tags

ergodic-action group-action smul-invariant-measure ergodic-smul ergodic-vadd regular-action minimal-action dense-powers haar-measure topological-group compact-group monoid-homomorphism preergodic
