---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Digraph
generated: 2025-12-08T16:00:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Digraph

## Overview

The `Digraph/` directory provides formalization of directed graphs (digraphs) on a vertex type `V`, treated as binary relations `V → V → Prop`. Unlike `SimpleGraph`, digraphs may have self-loops and edges without requiring symmetry or irreflexivity. The type `Digraph V` forms a `CompleteAtomicBooleanAlgebra` under the subgraph relation, representing the complete lattice of spanning subgraphs. The module includes conversions between digraphs and simple graphs through orientation-forgetting maps.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core digraph structure: defines `Digraph V` as adjacency relation wrapper; establishes complete Boolean algebra structure with lattice operations (⊔, ⊓, ⊤, ⊥, complement); provides decidability instances; includes complete/empty digraphs and complete bipartite digraphs |
| Orientation.lean | Graph orientation conversions: defines `toSimpleGraphInclusive` (edge if either orientation exists) and `toSimpleGraphStrict` (edge if both orientations exist); proves monotonicity and relationships with lattice operations |

## Subdirectories

None.

## Search Tags

digraph directed-graph relation adjacency-relation graph-theory boolean-algebra lattice subgraph orientation simple-graph complete-digraph bipartite-graph quiver
