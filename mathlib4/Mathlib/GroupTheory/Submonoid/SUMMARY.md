---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Submonoid
generated: 2026-01-24T23:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Submonoid

## Overview

The `Submonoid/` directory contains specialized theory for submonoids (multiplicative substructures with identity) focusing on structural properties that distinguish them from general subgroups. The three files cover fundamental submonoid constructions: the center (elements commuting with everything), centralizers (elements commuting with a given subset), and left inverses (the submonoid of elements having right inverses within a given submonoid). These provide the multiplicative analogs of additive submonoid theory and serve as building blocks for more specialized group-theoretic constructions.

## Key Files

| File | Purpose |
|------|---------|
| Center.lean | Center of a monoid: `Submonoid.center` as elements commuting with all elements, CommMonoid instance for the center, relationship to subsemigroup centers, decidability, isomorphisms between centers of isomorphic monoids |
| Centralizer.lean | Centralizer of a subset: `Submonoid.centralizer` as elements commuting with a given subset, relationship between center and centralizers, decidability, subset ordering properties |
| Inverses.lean | Left inverses submonoid: `S.leftInv` as the submonoid of left inverses of elements in S, MulEquiv between `S.leftInv` and `S` when S consists of units, Group instance on `IsUnit.submonoid M`, relationship to pointwise inverse in groups |

## Subdirectories

*(No subdirectories)*

## Search Tags

submonoid center centralizer left-inverse commute units monoid-homomorphism multiplicative-structure isomorphism
