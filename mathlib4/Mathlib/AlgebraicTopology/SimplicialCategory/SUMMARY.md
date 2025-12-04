---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/SimplicialCategory
generated: 2025-12-04T05:33:32Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# SimplicialCategory

## Overview

The `SimplicialCategory/` directory defines the notion of simplicial categories—categories enriched over the category of simplicial sets. A simplicial category is characterized by having simplicial sets as hom-objects, with ordinary morphisms identified as 0-simplices of the enriched hom. This abstraction is fundamental in homotopy theory, providing a bridge between category theory and homotopy-coherent structures. The directory establishes that the category of simplicial objects (and in particular, simplicial sets themselves) forms a simplicial category.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `SimplicialCategory` as an enriched ordinary category over simplicial sets; introduces `sHom` (enriched hom functor), `sHomComp` (enriched composition), and `homEquiv'` (bijection between ordinary morphisms and 0-simplices of enriched hom); includes TODO list for future developments (simplicial tensor, homotopy between morphisms, adjunction properties) |
| SimplicialObject.lean | Proves that the category of simplicial objects `SimplicialObject D` is a simplicial category by leveraging the general functor enrichment framework; establishes in particular that `SSet` (the category of simplicial sets) is itself a simplicial category |

## Subdirectories

*(none)*

## Search Tags

simplicial-category enriched-category simplicial-sets simplicial-objects enriched-hom hom-enrichment category-theory homotopy-theory functor-category
