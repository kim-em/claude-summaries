---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Abelianization
generated: 2026-01-24T22:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Abelianization

## Overview

This directory defines the abelianization functor for groups, which constructs the "most abelian" quotient of a group by quotienting out its commutator subgroup. The abelianization is the left adjoint to the forgetful functor from abelian groups to groups. The directory contains the core construction, universal property via the `lift` operation, functorial `map` operation, and finiteness preservation properties. This is a fundamental construction in group theory that captures the "abelian part" of any group.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core abelianization definitions: `Abelianization G` as `G ⧸ commutator G`, canonical projection `of : G →* Abelianization G`, universal property `lift` for homomorphisms to abelian groups, functorial `map` operation, and `MulEquiv.abelianizationCongr` showing equivalent groups have equivalent abelianizations |
| Finite.lean | Finiteness preservation: instances showing that abelianization of finite/fintype groups remains finite/fintype |

## Subdirectories

*(none)*

## Search Tags

abelianization commutator quotient-group universal-property adjunction functor group-theory finite-groups lift
