---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/SimplicialSet
generated: 2025-12-04T05:40:54Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 23
subdirs_count: 1
---

# SimplicialSet

## Overview

The `SimplicialSet/` directory contains the formalization of simplicial sets and their fundamental theory. Simplicial sets are Type-valued presheaves on the simplex category, providing a combinatorial approach to homotopy theory. The directory includes basic definitions (simplicial sets as functors, truncated simplicial sets, skeleton and coskeleton functors), geometric constructions (standard simplices, boundaries, horns, subcomplexes), structural theory (degenerate and non-degenerate simplices, composition structures, monoidal products), categorical constructions (nerve of a category, nerve adjunction to the homotopy category), path and homotopy theory (paths in simplicial sets, homotopy category construction, strict Segal condition), and specialized topics (Kan complexes, quasicategorical structures, anodyne extensions for model category theory).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines simplicial sets as `Type`-valued simplicial objects (presheaves on `SimplexCategory`), provides category instances, limits/colimits, truncation functors, skeleton/coskeleton adjunctions, and augmented simplicial sets |
| StdSimplex.lean | Defines the standard n-simplex `Δ[n]` as the representable presheaf `yoneda.obj [n]`, provides the fundamental building blocks for simplicial set constructions |
| Boundary.lean | Defines the boundary `∂Δ[n]` of the standard simplex as the subcomplex of non-surjective simplices, foundational for CW-complex and cell attachment theory |
| Horn.lean | Defines horns `Λ[n, i]` as subcomplexes of the standard simplex with the i-th face removed, essential for the Kan complex and quasicategory horn-filling conditions; includes constructors for edges, triangles, and primitive elements |
| KanComplex.lean | Defines Kan complexes as fibrant objects with respect to Kan fibrations (right lifting property against all horn inclusions), the simplicial analogue of topological spaces |
| Subcomplex.lean | General theory of subcomplexes of simplicial sets as subpresheaves, provides infrastructure for defining and working with boundaries, horns, and other geometric subcomplexes |
| SubcomplexColimits.lean | Proves that subcomplexes of simplicial sets have colimits, enabling constructions via gluing and pushouts |
| Simplices.lean | Defines n-simplices of a simplicial set and provides API for working with individual simplices |
| NonDegenerateSimplices.lean | Characterizes non-degenerate simplices and their properties, important for skeletal and minimal representations |
| NonDegenerateSimplicesSubcomplex.lean | Defines the subcomplex of non-degenerate simplices |
| Degenerate.lean | Defines degenerate and non-degenerate simplices, proves unique factorization of any simplex through degeneracy maps from a non-degenerate simplex |
| NerveNondegenerate.lean | Studies non-degenerate simplices in the nerve of a category |
| Nerve.lean | Defines the nerve of a category as a simplicial set with n-simplices being composable arrows (functors `Fin(n+1) → C`), provides the fundamental functor from categories to simplicial sets |
| NerveAdjunction.lean | Proves the nerve functor is right adjoint to the homotopy category functor, establishing the fundamental adjunction between categories and simplicial sets |
| Path.lean | Defines paths in simplicial sets as sequences of composable edges with vertex identifications, provides interval restrictions and path operations |
| HomotopyCat.lean | Constructs the homotopy category of a simplicial set by quotienting the free category on 1-simplices by 2-simplex composition relations |
| StrictSegal.lean | Defines the strict Segal condition (simplices uniquely determined by their spines), characterizes simplicial sets that behave like nerves of categories |
| CompStruct.lean | Defines composition structures for edges in simplicial sets via 2-simplices, formalizing when three edges compose |
| CompStructTruncated.lean | Composition structures for truncated simplicial sets |
| Coskeletal.lean | Proves that strict Segal simplicial sets are 2-coskeletal (determined by their 2-truncation), relating to nerves of categories |
| Monoidal.lean | Provides monoidal category structure on simplicial sets via Cartesian products, establishes simplicial sets as a monoidal closed category |
| CategoryWithFibrations.lean | Defines the Quillen model category structure on simplicial sets with Kan fibrations |
| Op.lean | Studies the opposite of a simplicial set |

## Subdirectories

- [ ] `AnodyneExtensions/` - Theory of anodyne extensions and weak factorization systems for the model category structure on simplicial sets (pending)

## Search Tags

simplicial-sets simplicial-objects presheaves simplex-category standard-simplex boundary horn kan-complex nerve nerve-adjunction homotopy-category paths strict-segal monoidal-category subcomplexes degenerate-simplices composition-structure anodyne-extensions model-category quasicategory fibrations
