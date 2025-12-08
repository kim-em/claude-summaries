---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SimpleGraph/Ends
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Ends

## Overview

The `Ends/` directory formalizes the concept of graph ends for simple graphs. An end is an equivalence class of infinite rays in a graph, defined rigorously as sections of a cofiltered inverse system. For each finite set of vertices K, the system tracks the connected components in the complement of K. Ends capture the "infinite directions" of a graph - intuitively, two infinite paths belong to the same end if they eventually stay in the same infinite component after removing any finite set of vertices. The formalization proves that locally finite preconnected infinite graphs have at least one end, and that finite graphs have no ends.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `ComponentCompl K` (components outside vertex set K), `componentComplMk` constructor, component support sets with `SetLike` instance, adjacency preservation, `ComponentCompl.hom` morphisms for K⊆L, `componentComplFunctor` (cofiltered functor from finite sets to component sets), and `SimpleGraph.end` as functor sections; proves components are disjoint, boundaries exist in preconnected graphs, and infinite components stay in all eventual ranges |
| Properties.lean | Properties of graph ends: proves finite graphs have empty end space (no ends), components chosen by ends are all infinite, locally finite preconnected infinite graphs have nonempty end space (at least one end exists) |

## Subdirectories

None - this is a leaf directory.

## Search Tags

graph-ends infinite-rays cofiltered-system inverse-system connected-components component-complement locally-finite preconnected functor-sections categorical-limit end-space boundary-vertices infinite-graph
