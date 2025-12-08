---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SimpleGraph/Connectivity
generated: 2025-12-08T23:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 5
subdirs_count: 0
---

# Connectivity

## Overview

The `Connectivity/` subdirectory provides the core theory of graph connectivity for simple graphs. It defines reachability (existence of walks between vertices), connectivity predicates (preconnected and connected graphs), connected components as equivalence classes under reachability, and bridge edges. The module includes walk manipulation operations (taking/dropping until a vertex, rotation), walk counting and enumeration for locally finite graphs, connectivity properties for subgraphs and induced graphs, and component representation theory for selecting one vertex per component (used in matching theory).

## Key Files

| File | Purpose |
|------|---------|
| Connected.lean | Core connectivity theory: defines `Reachable` (walk existence between vertices), `Preconnected` (all vertices reachable), `Connected` (preconnected + nonempty), `ConnectedComponent` quotient type (equivalence classes under reachability), component support sets, `IsBridge` predicate (edge whose deletion increases components), bridge characterization theorem (bridges are edges not in any cycle) |
| Subgraph.lean | Subgraph connectivity: defines `Subgraph.Preconnected` and `Subgraph.Connected` via coercion to simple graphs, proves singleton and adjacent-pair subgraphs are connected, monotonicity lemmas for connectivity under subgraph inclusion |
| WalkCounting.lean | Walk enumeration: defines `walkLengthTwoEquivCommonNeighbors` (bijection between length-2 walks and common neighbors), `finsetWalkLength` (finset of walks of given length for decidable locally finite graphs), recursive characterization for walk counting |
| WalkDecomp.lean | Walk decomposition operations: defines `takeUntil` (walk prefix up to vertex), `dropUntil` (walk suffix from vertex), `rotate` (rotate loop walk to start at different vertex), proves decomposition lemmas and support membership characterizations |
| Represents.lean | Component representation: defines `ConnectedComponent.Represents` (set of vertices containing exactly one per component via bijection), cardinality lemmas, establishes relationship between representative sets and odd components for matching theory applications |

## Subdirectories

(No subdirectories)

## Search Tags

connectivity reachability connected-components preconnected walks paths bridge-edges equivalence-relation quotient-type walk-decomposition walk-counting locally-finite component-representation graph-connectivity simple-graph
