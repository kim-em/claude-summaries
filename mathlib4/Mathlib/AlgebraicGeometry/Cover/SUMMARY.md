---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/Cover
generated: 2025-12-04T12:39:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Cover

## Overview

The `Cover/` directory provides the fundamental theory of covers of schemes in algebraic geometry, with emphasis on covers with respect to morphism properties. It defines general covers as jointly surjective indexed families of scheme morphisms satisfying a specified property `P`, open covers as the special case where all components are open immersions, and develops the API for cover manipulation including pullbacks, refinements, and categorical structure. The directory includes specialized theories for locally directed covers (which admit compatible transition maps and gluing constructions), covers over a base scheme, and functorial operations like collapsing covers to single-object covers via disjoint unions.

## Key Files

| File | Purpose |
|------|---------|
| MorphismProperty.lean | Core API for covers of schemes: defines `Cover K` as 0-hypercovers, establishes jointly surjective property, provides constructors (`mkOfCovers`, `coverOfIsIso`), and defines affine covers with `AffineCover` structure and categorical structure via `Cover.Hom` refinements |
| Open.lean | API for open covers specifically: defines `OpenCover` as covers where all components are open immersions, provides `affineCover` and `affineOpenCover` constructors, proves compactness properties, finite subcover extraction, and section gluing theorems (`ext_elem`, `zero_of_zero_cover`) |
| Directed.lean | Theory of locally directed covers with compatible transition maps: defines `LocallyDirected` class with transition maps `trans : 𝒰ᵢ → 𝒰ⱼ` for `i ≤ j`, proves gluing properties, constructs colimits via `coconeOfLocallyDirected`, and provides the canonical `directedAffineCover` of all affine opens |
| Over.lean | Covers of schemes over a base `S`: defines `Cover.Over S` typeclass asserting components are `S`-schemes with compatible structure morphisms, provides pullback constructions in the over-category (`pullbackCoverOver`, `pullbackCoverOverProp`), and instances for standard cover operations |
| Sigma.lean | Functorial collapsing of covers to single-object covers: defines `sigma` operation sending cover `𝒰` to single-object cover with component `∐ 𝒰.X` (disjoint union), natural transformation `toSigma : 𝒰 ⟶ 𝒰.sigma`, and functoriality `sigmaFunctor` |

## Subdirectories

*(none)*

## Search Tags

algebraic-geometry schemes covers open-covers affine-covers morphism-properties jointly-surjective precoverage hypercovers zariski-topology directed-covers transition-maps colimits gluing refinements over-category base-change pullbacks disjoint-union categorical-structure
