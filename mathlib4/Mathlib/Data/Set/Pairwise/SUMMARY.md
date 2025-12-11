---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Set/Pairwise
generated: 2025-12-11T18:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 4
subdirs_count: 0
---

# Pairwise

## Overview

The `Pairwise/` directory develops the theory of pairwise relations on sets, with a focus on pairwise disjointness. The central concept is `Set.PairwiseDisjoint s f`, which states that images under `f` of distinct elements of `s` are disjoint. This is defined as `s.Pairwise (Disjoint on f)` but uses a separate definition to permit dot notation. The directory provides lemmas for unions, intersections, products, chains, and interactions with lists, building the infrastructure for working with disjoint families of sets throughout mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and lemmas: `Set.PairwiseDisjoint`, pairwise relations for singletons, pairs, unions, inserts; equivalences with `InjOn`; fiber pairwise disjointness; product and pi set lemmas; elimination principles for pairwise disjoint sets |
| Lattice.lean | Pairwise relations and the set lattice: lemmas for indexed unions (`iUnion`, `sUnion`), bind operations for `PairwiseDisjoint`, product lattice results with `Frame`, equivalence `biUnionEqSigmaOfDisjoint` between disjoint unions and sigma types |
| Chain.lean | Pairwise results for chains: when a chain of sets satisfies pairwise relations iff each member does; lemmas for `IsChain` on `iUnion` and `sUnion` |
| List.lean | Translating between `Set.Pairwise` and `List.Pairwise`: for lists with no duplicates, the two notions are equivalent |

## Subdirectories

(none)

## Search Tags

pairwise pairwise-disjoint disjoint relation set sets union intersection fiber lattice chain list nodup directed
