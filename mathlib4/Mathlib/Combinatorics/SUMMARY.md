---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 7
subdirs_count: 13
---

# Combinatorics

## Overview

The `Combinatorics/` directory contains formalized combinatorial mathematics including Ramsey theory, graph theory, enumeration, and optimization. Key results include the Hales-Jewett theorem, Hindman's theorem on finite sums, Alon's combinatorial Nullstellensatz, and various pigeonhole principles. The directory provides foundations for colexicographic ordering, configurations of points and lines, derangements, and specialized structures like matroids, quivers, set families, and simple graphs.

## Key Files

| File | Purpose |
|------|---------|
| Colex.lean | Colexicographic (colex) order on finite sets: a binary-like ordering that avoids large values, with properties like linearity, decidability, monotonicity preservation, and equivalence to geometric sums for ℕ; used in the Kruskal-Katona theorem |
| Configuration.lean | Abstract configurations of points and lines with nondegeneracy conditions; proves that HasLines, HasPoints, and \|P\| = \|L\| are mutually implying properties (any two imply the third) |
| HalesJewett.lean | Hales-Jewett theorem on combinatorial lines: any finite coloring of high-dimensional function space contains a monochromatic combinatorial line; includes multidimensional version for combinatorial subspaces and implies Van der Waerden's theorem |
| Hindman.lean | Hindman's theorem on finite sums: for any finite coloring of a semigroup, there exists a sequence such that all finite sums (without repetition) are monochromatic; uses idempotent ultrafilters on Stone-Čech compactification |
| Nullstellensatz.lean | Alon's combinatorial Nullstellensatz: gives combinatorial constraints for polynomial vanishing on Cartesian products of finite sets, with applications to zero-sum problems and combinatorial existence results |
| Pigeonhole.lean | Collection of 20+ pigeonhole principle variants: basic principle (more pigeons than holes implies collision), variations with weight functions, strict/non-strict inequalities, and bounds on pigeons per hole |
| Schnirelmann.lean | Schnirelmann density for sets of natural numbers: defined as inf_{n>0} \|A ∩ {1,...,n}\| / n, with bounds and calculations; foundational for additive combinatorics |

## Subdirectories

- [x] `Additive/` - Additive combinatorics: comprehensive formalization including sumset theory (Cauchy-Davenport, Plünnecke-Ruzsa), structural theorems (Freiman homomorphisms, approximate subgroups), 3-term arithmetic progressions (Roth numbers, Behrend's construction), and corners theorem connecting to Roth's theorem via Szemerédi's regularity
- [x] `Derangements/` - Derangements (permutations without fixed points): defines derangements on types, proves recursive decomposition via Option types, establishes cardinality formulas, and shows D(n)/n! → 1/e
- [x] `Digraph/` - Directed graphs: formalized as binary relations `V → V → Prop` with self-loops allowed; complete atomic Boolean algebra structure under subgraph ordering; conversion functions to simple graphs via orientation-forgetting maps
- [x] `Enumerative/` - Enumerative combinatorics: Bell numbers (counting set partitions with refinements), Catalan numbers (counting binary trees and Dyck paths with bijections), compositions (ordered partitions), double counting arguments, Dyck words (balanced brackets), incidence algebras with Möbius inversion, inclusion-exclusion principles, integer partitions with generating function theory (infinite product formulas), and Stirling numbers (permutation cycles and set partitions)
- [x] `Extremal/` - Extremal combinatorics: Ruzsa-Szemerédi problem on maximum edges in locally linear graphs (each edge in exactly one triangle), with construction from 3AP-free sets yielding Ω(n² * exp(-4 * √(log n))) lower bound
- [x] `Graph/` - Multigraphs with vertices and edges as embedded sets: defines `Graph α β` structure with incidence predicates (`IsLink`, `Inc`, `Adj`), loop classification, adjacency API, and extensionality principles; uses compact notation `V(G)` and `E(G)`
- [x] `Hall/` - Hall's Marriage Theorem: formalized in two versions (finite index type using strong induction, generalized version using inverse limit compactness to remove finiteness constraint); states that indexed families of finite sets have systems of distinct representatives iff every k-union has ≥k elements
- [ ] `Matroid/` - Matroid theory (pending)
- [ ] `Optimization/` - Combinatorial optimization (pending)
- [ ] `Quiver/` - Quivers (directed multigraphs) and their paths (pending)
- [ ] `SetFamily/` - Families of sets and their properties (pending)
- [ ] `SimpleGraph/` - Simple graphs (undirected graphs without loops or multiple edges) (pending)
- [ ] `Young/` - Young tableaux and related combinatorial structures (pending)

## Search Tags

combinatorics ramsey-theory graph-theory enumeration colex colexicographic-order hales-jewett hindman ultrafilter nullstellensatz pigeonhole schnirelmann-density configuration matroid quiver set-family simple-graph young-tableau derangement extremal-combinatorics additive-combinatorics van-der-waerden
