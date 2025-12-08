---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SimpleGraph/Extremal
generated: 2025-12-08T23:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# Extremal

## Overview

The `Extremal/` directory formalizes extremal graph theory, studying graphs that maximize edges subject to forbidden subgraph constraints. The core concept is the extremal number—the maximum edge count in H-free graphs on n vertices. The directory includes Turán's theorem (the complete r-partite graph with balanced parts is the unique extremal Kr+1-free graph), Zykov symmetrisation (proving non-adjacency is an equivalence relation in extremal graphs), and Turán density (the asymptotic limit of extremal numbers). All extremal graphs are characterized through isomorphism to canonical Turán graphs with explicit edge count formulas.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core extremal definitions: `IsExtremal` (maximum-edge graphs satisfying property), `extremalNumber n H` (maximum edges in H-free n-vertex graphs), existence theorems, edge count bounds, comparison lemmas (containment implies extremal number inequality), isomorphism invariance, extremal characterization of H-free graphs |
| Turan.lean | Turán's theorem: `IsTuranMaximal` (extremal Kr+1-free graphs), `turanGraph n r` (canonical complete r-partite balanced construction), Zykov symmetrisation proving non-adjacency forms equivalence classes in extremal graphs, equipartition result (parts have equal size ⌊n/r⌋ or ⌈n/r⌉), isomorphism between any Turán-maximal graph and turanGraph, exact edge count formula `(n² - (n mod r)²)(r-1)/(2r) + (n mod r).choose 2`, edge bound for clique-free graphs |
| TuranDensity.lean | Turán density theory: `turanDensity H` (limit of `extremalNumber n H / n.choose 2` as n→∞), proof of convergence using monotonicity and infimum, asymptotic equivalence `extremalNumber n H ~ turanDensity H · n.choose 2`, antitonicity lemma via double-counting argument on vertex-edge non-incidence |

## Subdirectories

(No subdirectories)

## Search Tags

extremal-graph-theory turan-theorem turan-graph turan-density extremal-number forbidden-subgraph clique-free zykov-symmetrisation equipartition complete-multipartite asymptotic-density graph-maximization edge-count combinatorics extremal-combinatorics ramsey-type
