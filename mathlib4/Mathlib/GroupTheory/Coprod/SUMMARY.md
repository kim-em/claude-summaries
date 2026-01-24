---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Coprod
generated: 2026-01-24T23:21:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Coprod

## Overview

The `Coprod/` directory contains the formalization of the coproduct (free product) of two monoids or groups, denoted `M ∗ N`. This construction provides the universal property: for any monoid homomorphisms `f : M →* P` and `g : N →* P`, there exists a unique homomorphism `M ∗ N →* P` that factors through the canonical embeddings. The implementation is built from scratch using congruence relations on free monoids rather than as a special case of indexed coproducts, enabling cleaner API, better universe handling, and more computationally efficient code.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Complete theory of binary coproducts: construction via congruence on `FreeMonoid (M ⊕ N)`, universal property (`lift`), canonical embeddings (`inl`, `inr`), mapping functoriality (`map`), swap isomorphism, projections to components and products, group structure, associativity, and unit laws |

## Subdirectories

None.

## Search Tags

coproduct free-product monoid group universal-property lift embedding congruence free-monoid associativity functoriality swap projection
