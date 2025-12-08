---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Graph
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# Graph

## Overview

The `Graph/` directory provides a foundational formalization of multigraphs (graphs allowing multiple edges between vertices and self-loops). Unlike simple graphs, multigraphs model vertices and edges as sets within ambient types rather than as types themselves, following the "embedded set" design pattern used in matroid theory. This design enables subgraphs, minors, and other graph constructions to coexist naturally without needing separate coercion machinery.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core multigraph structure `Graph α β` with vertex type `α` and edge type `β`; defines incidence predicates (`IsLink`, `Inc`, `Adj`), loop classification (`IsLoopAt`, `IsNonloopAt`), incidence/adjacency API, extensionality principles, and fundamental lemmas for edge-vertex relationships; uses compact notation `V(G)` and `E(G)` for vertex and edge sets |

## Subdirectories

None.

## Search Tags

multigraph graph-theory incidence adjacency loops vertex-set edge-set graph-structure embedded-set-design islink inc adj extensionality
