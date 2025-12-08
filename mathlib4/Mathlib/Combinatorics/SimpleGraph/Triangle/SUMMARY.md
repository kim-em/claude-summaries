---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SimpleGraph/Triangle
generated: 2025-12-08T23:38:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 4
subdirs_count: 0
---

# Triangle

## Overview

The `Triangle/` directory formalizes triangle-related theory in simple graphs, including locally linear graphs (where edges belong to unique triangles), the Triangle Counting Lemma (uniform regular graphs contain many triangles), and the Triangle Removal Lemma (graphs with few triangles can be made triangle-free by removing few edges). It also provides a construction of tripartite graphs from triangle indices, used in both the Ruzsa-Szemerédi problem and the proof of the corners theorem from triangle removal.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines locally linear graphs (edges in exactly one triangle), edge-disjoint triangles, and `FarFromTriangleFree` predicate (requiring removal of ε·n² edges to eliminate triangles); proves edge counts and farness properties |
| Counting.lean | Proves the Triangle Counting Lemma: if G has vertex sets s, t, u that are pairwise ε-uniform and 2ε-dense, then (1-2ε)·ε³·\|s\|·\|t\|·\|u\| triples form triangles |
| Removal.lean | Proves the Triangle Removal Lemma: if G has fewer than `triangleRemovalBound ε · n³` triangles, then removing fewer than ε·n² edges makes G triangle-free; uses Szemerédi regularity to find dense regular pairs |
| Tripartite.lean | Constructs tripartite graphs on α⊕β⊕γ from triangle indices (a,b,c)∈α×β×γ; defines `ExplicitDisjoint` (edge-disjoint explicit triangles) and `NoAccidental` (all triangles are explicit) predicates for applications to Roth numbers and corners theorem |

## Subdirectories

None.

## Search Tags

triangle graph-theory triangle-counting triangle-removal szemerédi-regularity locally-linear edge-disjoint clique-free far-from-triangle-free tripartite-graph ruzsa-szemerédi corners-theorem uniform-regular triangle-lemma extremal-graph-theory
