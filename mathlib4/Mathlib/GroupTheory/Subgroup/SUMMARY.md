---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Subgroup
generated: 2026-01-24T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Subgroup

## Overview

The `Subgroup/` directory contains specialized subgroup theory focused on particular classes of subgroups defined by commutativity and structural properties. Topics include centers (elements commuting with all group elements), centralizers (elements commuting with a given set), saturated subgroups (closed under taking roots), and simple groups (groups with exactly two normal subgroups). These files extend the basic subgroup infrastructure found in `Algebra.Group.Subgroup.Basic` with group-theoretic characterizations and classifications.

## Key Files

| File | Purpose |
|------|---------|
| Center.lean | Centers of groups: definition as subgroup of elements commuting with everything, characterization via `Set.center`, characteristic property, conjugacy class bijections, commutative group equivalence |
| Centralizer.lean | Centralizers of sets: subgroups commuting with given elements, relationship to centers, normalizer action on subgroups, homomorphism `N(H) → Aut(H)` with kernel `C(H)` |
| Saturated.lean | Saturated subgroups: property that `g^n ∈ H` implies `n = 0` or `g ∈ H`, characterization via natural/integer powers, kernel saturation for torsion-free targets |
| Simple.lean | Simple groups: `IsSimpleGroup` class for groups with exactly two normal subgroups (⊥ and ⊤), preservation under surjective homomorphisms and isomorphisms, simple order structure for commutative case |

## Subdirectories

None.

## Search Tags

subgroup center centralizer saturated simple-group normal-subgroup commutative conjugacy characteristic automorphism normalizer torsion-free
