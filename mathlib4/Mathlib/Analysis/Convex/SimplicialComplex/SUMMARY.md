---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Convex/SimplicialComplex
generated: 2025-12-05T09:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# SimplicialComplex

## Overview

The `SimplicialComplex/` directory contains the theory of simplicial complexes in modules over rings with partial order. A simplicial complex is modeled as a downward-closed collection of affine independent finite sets (vertices) whose convex hulls (faces) "glue nicely" via controlled intersections. This module provides the core structure definition, vertices and facets, underlying space, and a semilattice ordering on complexes.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `SimplicialComplex 𝕜 E` structure with faces (downward-closed, affine independent vertex sets), vertices (zero-dimensional faces), facets (maximal faces), underlying space (union of convex hulls), and semilattice structure (inf, bot); proves intersection properties and face subset characterizations |

## Subdirectories

*(none)*

## Search Tags

simplicial-complex convex-geometry affine-independence faces vertices facets convex-hull gluing-condition downward-closed maximal-faces semilattice-inf
