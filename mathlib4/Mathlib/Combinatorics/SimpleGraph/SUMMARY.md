---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SimpleGraph
generated: 2025-12-08T21:00:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 42
subdirs_count: 6
---

# SimpleGraph

## Overview

The `SimpleGraph/` directory contains formalization of simple graphs (undirected graphs without loops or multiple edges) defined as irreflexive symmetric relations on a vertex type. The module provides comprehensive theory including fundamental structures (adjacency matrices, subgraphs, walks, paths), graph properties (connectivity, bipartiteness, colorability, matchings, cliques), graph operations (products, maps, complements), structural characterizations (Hamiltonian paths, Tutte's theorem), and specialized graph classes (strongly regular, circulant, complete multipartite). The adjacency relation is core: vertices adjacent when related, forming a complete atomic Boolean algebra under subgraph ordering.

## Key Files

| File | Purpose |
|------|---------|
| Init.lean | Declares the `SimpleGraph` Aesop rule set for automated proof tactics; must be imported for `aesop_graph` tactic visibility |
| Basic.lean | Core definitions: `SimpleGraph` structure (irreflexive symmetric adjacency relation), neighbor sets, common neighbors, incidence sets, complete atomic Boolean algebra instance for subgraph lattice; includes custom `aesop_graph` tactics and complete bipartite graph constructor |
| Subgraph.lean | Subgraph theory: defines `Subgraph G` structure (vertex subset with restricted adjacency), neighbor/incidence sets, coercion to simple graphs, spanning/induced subgraph predicates, lattice instances, graph homomorphisms between subgraphs, single-vertex and single-edge subgraphs |
| AdjMatrix.lean | Adjacency matrices: defines `Matrix.IsAdjMatrix` (0-1 symmetric matrix with zero diagonal), conversion between matrices and graphs, proves matrix powers count walks (nth power entry = number of length-n walks) |
| Clique.lean | Clique theory: defines `IsClique` (pairwise adjacent vertex set), `IsNClique` (n-vertex cliques), `cliqueFinset` (enumeration), `CliqueFree` predicate, proves cliques have complete induced subgraphs |
| Matching.lean | Matching theory: defines `Subgraph.IsMatching` (vertices incident to exactly one edge), `IsPerfectMatching`, `IsMatchingFree`, `IsCycles`, `IsAlternating` for alternating paths in matching algorithms; includes Tutte's theorem foundations |
| Coloring.lean | Graph colorings: defines `Coloring α` as homomorphisms to complete graphs, `Colorable n` (n-colorability), `chromaticNumber` (minimal coloring, ℕ∞-valued), color classes and partitions; includes TODO for trees, planar graphs, chromatic polynomials |
| Bipartite.lean | Bipartite graphs: `IsBipartiteWith s t` (edges only between disjoint sets s and t), `IsBipartite` (equivalent to 2-colorable), double-counting proofs relating degree sums to edge counts, `between` subgraph constructor; includes TODO for odd cycle characterization |
| Hamiltonian.lean | Hamiltonian graphs: defines `Walk.IsHamiltonian` (visiting every vertex exactly once), `Walk.IsHamiltonianCycle`, `IsHamiltonian` graph predicate, proves Hamiltonian paths are paths and induce finite vertex sets |
| Tutte.lean | Tutte's theorem: defines `IsTutteViolator` (certifying perfect matching non-existence via odd components after vertex deletion), proves Tutte's theorem (perfect matching exists iff no Tutte violators) |
| StronglyRegular.lean | Strongly regular graphs: `IsSRGWith n k ℓ μ` structure (n vertices, k-regular, ℓ common neighbors for adjacent pairs, μ for non-adjacent), proves complement is strongly regular, parameter equation k(k-ℓ-1)=(n-k-1)μ, matrix equation A²=kI+ℓA+μC |
| Acyclic.lean | Acyclic graphs and tree characterizations |
| Circulant.lean | Circulant graphs (vertex-transitive graphs on cyclic groups) |
| CompleteMultipartite.lean | Complete multipartite graphs and their properties |
| ConcreteColorings.lean | Specific coloring constructions and examples |
| Copy.lean | Graph isomorphism via vertex type changes with adjacency preservation |
| Dart.lean | Darts (half-edges) as directed edge representation |
| DegreeSum.lean | Degree sum formulas including handshaking lemma (sum of degrees = 2×edges) |
| DeleteEdges.lean | Edge deletion operations and properties |
| Density.lean | Graph density measures and edge-counting arguments |
| Diam.lean | Graph diameter (maximum distance between vertices) |
| Finite.lean | Finiteness properties for graphs and subgraphs |
| Finsubgraph.lean | Finite subgraphs with cardinality constraints |
| FiveWheelLike.lean | Five-wheel-like graphs and structural characterizations |
| Girth.lean | Girth (length of shortest cycle) |
| Hall.lean | Hall's marriage theorem application to graphs |
| Hasse.lean | Hasse diagrams as graphs of covering relations |
| IncMatrix.lean | Incidence matrices (vertex-edge incidence) |
| LapMatrix.lean | Laplacian matrices (degree matrix minus adjacency matrix) |
| LineGraph.lean | Line graphs (edges become vertices) |
| Maps.lean | Graph homomorphisms, embeddings, isomorphisms |
| Metric.lean | Graph metrics and distance functions |
| Operations.lean | Graph operations (union, complement, product, etc.) |
| Partition.lean | Vertex partitions and quotient graphs |
| Path.lean | Path module export/organization |
| Paths.lean | Path theory: defines walks (edge sequences), trails (no repeated edges), paths (no repeated vertices), reachability, walk composition, path induction principles |
| Prod.lean | Graph products (Cartesian, tensor, etc.) |
| Sum.lean | Graph sums and disjoint unions |
| Trails.lean | Trail-specific theory and characterizations |
| Turan.lean | Turán graphs and extremal graph theory setup |
| UniversalVerts.lean | Universal vertices (adjacent to all other vertices) |
| Walk.lean | Walk module export/organization |

## Subdirectories

- [x] `Connectivity/` - Connectivity properties: connected components, paths, reachability, walk counting, bridges, cut vertices (complete)
- [x] `Ends/` - Graph ends (equivalence classes of infinite rays) and end spaces (complete)
- [x] `Extremal/` - Extremal graph theory: Turán's theorem, extremal numbers, Turán density, forbidden subgraphs (complete)
- [x] `Regularity/` - Szemerédi's regularity lemma and applications (complete)
- [x] `Triangle/` - Triangle-related properties: triangle-free graphs, triangle counting, local clustering (complete)
- [x] `Walks/` - Walk theory extensions: basic walk structure, operations, traversal, graph mappings, subwalk relation (complete)

## Search Tags

simple-graph undirected-graph adjacency-relation irreflexive symmetric subgraph clique matching coloring chromatic-number bipartite hamiltonian tutte strongly-regular adjacency-matrix walks paths connectivity vertex edge graph-theory combinatorics degree-sum handshaking-lemma
