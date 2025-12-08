---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Quiver/Path
generated: 2025-12-08T07:55:24Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# Path

## Overview

The `Path/` subdirectory extends the core path theory from `Quiver.Path` with additional operations and lemmas. It provides three main modules: decomposition lemmas for splitting paths at set boundaries, vertex operations for reasoning about the vertices along a path, and weight calculations for computing multiplicative or additive measures along paths. These are all authored by Matteo Cipollina (2025) and build directly on the foundational `Path` type defined in the parent directory.

## Key Files

| File | Purpose |
|------|---------|
| Decomposition.lean | Boundary-crossing lemmas for paths: proves that paths from outside a set `S` to inside `S` (or vice versa) must contain an edge crossing the boundary; provides `exists_notMem_mem_hom_path_path_of_notMem_mem` and its dual for decomposing paths at set boundaries |
| Vertices.lean | Operations on path vertices: defines `Path.end` (terminal vertex), `Path.vertices` (list of all vertices including endpoints), membership predicates, and decomposition theorems including splitting paths at arbitrary vertices (`exists_eq_comp_of_mem_vertices`) and at the last occurrence of a vertex (`exists_eq_comp_and_notMem_tail_of_mem_vertices`) |
| Weight.lean | Path weight computations: defines `Path.weight` (multiplicative product of edge weights) and `Path.addWeight` (additive sum), with `to_additive` infrastructure; includes `weightOfEPs` variant where edge weights are functions of endpoints; proves weight composition (`weight_comp`) and positivity/non-negativity preservation for ordered semirings |

## Subdirectories

*(No subdirectories)*

## Search Tags

quiver path decomposition boundary-crossing vertices vertex-list path-splitting weight multiplicative-weight additive-weight edge-weights path-composition positivity ordered-semiring
