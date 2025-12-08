---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SimpleGraph/Walks
generated: 2025-12-08T22:40:15Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 5
subdirs_count: 0
---

# Walks

## Overview

The `Walks/` directory contains comprehensive theory for graph walks in simple graphs. This refines and extends the core walk type defined in the parent directory. Walk theory includes basic properties (structure, length, support, darts, edges), operations for constructing and manipulating walks (copy, append, reverse, take, drop), mappings between graphs (homomorphisms, supergraphs, induced subgraphs), traversal functions for accessing walk vertices, and the subwalk relation for contiguous subsequences. These modules are foundational for path theory, connectivity, and walk-based graph algorithms.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core walk inductive type: `Walk u v` sequences adjacent vertices from `u` to `v`, includes `nil` (empty walk) and `cons` constructors; defines length, support (vertex list), darts, edges, edgeSet; provides pattern aliases `nil'` and `cons'` with explicit vertices |
| Operations.lean | Walk operations: `copy` (change endpoints via equalities), `append` (concatenate walks), `concat` (add edge to end), `reverse` (reverse walk), `drop`/`take` (first n darts), `tail` (remove first dart), `dropLast` (remove last dart); forms basis for walk algebra |
| Traversal.lean | Vertex access functions: `getVert n` (nth vertex, clamped to endpoint), `snd` (second vertex or endpoint), `penultimate` (second-to-last vertex or start), `firstDart`/`lastDart` (edge extraction from non-empty walks); enables indexing into walk structure |
| Maps.lean | Graph homomorphism mapping: `map` (lift walks via graph homomorphism), `mapLe` (map to supergraph), `transfer` (map to graph containing edges), `induce` (map to induced subgraph on vertex set), `toDeleteEdges`/`toDeleteEdge` (map to edge-deleted subgraphs); connects walks across related graphs |
| Subwalks.lean | Subwalk relation: `IsSubwalk p q` (walk `p` is contiguous subwalk of `q`), proves reflexivity, transitivity, length monotonicity, relates subwalks to list infixes of support; enables reasoning about walk containment |

## Subdirectories

(No subdirectories)

## Search Tags

walk graph-walk simple-graph vertices edges darts support length append reverse traverse subwalk map homomorphism induced-subgraph walk-operations walk-theory path-theory connectivity adjacency-sequence
