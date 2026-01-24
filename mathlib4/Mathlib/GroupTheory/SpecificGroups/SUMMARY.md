---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/SpecificGroups
generated: 2026-01-24T12:01:46Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 6
subdirs_count: 1
---

# SpecificGroups

## Overview

The `SpecificGroups/` directory contains formalizations of concrete, well-studied families of groups. The main files define cyclic groups (including primality-based cyclicity results and exponent characterizations), dihedral groups (symmetries of regular n-gons), quaternion groups (generalized dicyclic groups of order 4n), Klein four-groups (non-cyclic abelian groups of order 4 and exponent 2), Z-groups (groups whose Sylow subgroups are all cyclic), and alternating groups (even permutations with simplicity results). These implementations provide both the group structure definitions and key classification theorems for these fundamental group families.

## Key Files

| File | Purpose |
|------|---------|
| Cyclic.lean | Cyclic groups: IsCyclic predicate, generator existence, prime order cyclicity, exponent characterizations, finite simple abelian group classification |
| Dihedral.lean | Dihedral groups DihedralGroup n: symmetry groups of regular n-gons with rotations r i and reflections sr i |
| Quaternion.lean | Quaternion groups QuaternionGroup n: generalized dicyclic groups of order 4n with presentation ⟨a, x \| a^(2n) = 1, x^2 = a^n, x^(-1)ax = a^(-1)⟩ |
| KleinFour.lean | Klein four-group: IsKleinFour mixin class for groups of order 4 and exponent 2, isomorphisms between Klein four-groups |
| ZGroup.lean | Z-groups: groups with cyclic Sylow subgroups, semidirect product characterization, cyclic abelianization and commutator results |
| Alternating.lean | Alternating groups: even permutations as kernel of sign homomorphism, index-two characterization, 3-cycle generation, simplicity of A₅ |

## Subdirectories

- [x] `Alternating/` - Additional results on alternating groups: centralizers, Klein four-group in A₄, maximal subgroups

## Search Tags

cyclic-group dihedral-group quaternion-group klein-four z-group alternating-group specific-groups concrete-groups symmetry-group finite-groups prime-order exponent sylow-subgroups
