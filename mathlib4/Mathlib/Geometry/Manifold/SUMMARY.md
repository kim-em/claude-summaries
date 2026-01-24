---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold
generated: 2026-01-24T06:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: preliminary
files_count: 24
subdirs_count: 11
---

# Manifold

## Overview

The `Manifold/` directory contains the formalization of smooth manifolds and differential geometry in Mathlib. It provides the foundational framework for defining manifolds as topological spaces locally modeled on a model space (typically a normed vector space), with smooth transition maps between charts. The library supports both finite-dimensional and infinite-dimensional manifolds, manifolds with boundary, and various structures built on top of manifolds including Lie groups, vector bundles, and Riemannian geometry. Key concepts include charted spaces, structure groupoids, smooth maps (`ContMDiff`), the manifold derivative (`mfderiv`), diffeomorphisms, immersions, and smooth embeddings.

## Key Files

| File | Purpose |
|------|---------|
| StructureGroupoid.lean | Defines structure groupoids (sets of open partial homeomorphisms stable under composition and inverse) used to specify smoothness of coordinate changes |
| ChartedSpace.lean | Defines charted spaces (spaces with an atlas of charts to a model space) and the core framework for manifolds |
| HasGroupoid.lean | Defines `HasGroupoid M G` typeclass requiring coordinate changes belong to a structure groupoid G |
| Notation.lean | Custom elaborators for compact notation: `MDiff`, `CMDiff`, `mfderiv%`, `T%` for sections in fiber bundles |
| Diffeomorph.lean | Defines diffeomorphisms (`≃ₘ^n`) between smooth manifolds, with products and sums |
| LocalDiffeomorph.lean | Defines local diffeomorphisms (maps that are diffeomorphisms in neighborhoods of each point) |
| Immersion.lean | Defines smooth immersions (maps whose differential is locally a linear embedding) |
| SmoothEmbedding.lean | Defines smooth embeddings (immersions that are also topological embeddings) |
| BumpFunction.lean | Smooth bump functions on manifolds (1 on a ball, 0 outside a larger ball) |
| PartitionOfUnity.lean | Smooth partitions of unity subordinate to open covers, existence on σ-compact manifolds |
| LocalInvariantProperties.lean | Framework for lifting local properties (like differentiability) from model spaces to manifolds |
| LocalSourceTargetProperty.lean | Properties of maps defined in terms of local behavior in source/target charts |
| ContMDiffMFDeriv.lean | Smoothness of the manifold derivative operation |
| ContMDiffMap.lean | The type of smooth maps `C^n⟮I, M; J, N⟯` between manifolds |
| DerivationBundle.lean | Derivations on smooth functions as a model for the tangent bundle |
| GroupLieAlgebra.lean | Lie algebra structure on the tangent space at the identity of a Lie group |
| Complex.lean | Holomorphic functions on complex manifolds; maximum modulus principle |
| ConformalGroupoid.lean | The structure groupoid of conformal maps |
| Metrizable.lean | σ-compact Hausdorff finite-dimensional manifolds are metrizable |
| WhitneyEmbedding.lean | Whitney embedding theorem: compact manifolds embed in Euclidean space |
| SmoothApprox.lean | Approximation of continuous functions by smooth functions using partitions of unity |
| Bordism.lean | Singular manifolds and the beginnings of unoriented bordism theory |
| PoincareConjecture.lean | Statement of the generalized Poincaré conjecture (as `proof_wanted`) |

## Subdirectories

- [x] `Algebra/` - Lie groups, smooth monoid structures, left-invariant derivations, and smooth functions as an algebra
- [x] `ContMDiff/` - Core definitions and properties of continuously differentiable maps between manifolds (`ContMDiff`, `ContMDiffAt`, etc.)
- [x] `Instances/` - Concrete manifold instances: real line, unit interval `[0,1]`, spheres, units of normed algebras
- [x] `IntegralCurve/` - Integral curves of vector fields: existence, uniqueness, and transformations
- [x] `IsManifold/` - The `IsManifold` typeclass and properties of manifolds (interior, boundary, extended charts)
- [x] `MFDeriv/` - The manifold derivative `mfderiv`: definitions, basic properties, chain rule, specific functions
- [x] `Riemannian/` - Riemannian geometry: metrics on manifolds, path length via energy functionals
- [x] `Sheaf/` - Sheaf-theoretic perspective on manifolds: sheaves of smooth functions, locally ringed spaces
- [x] `VectorBundle/` - Smooth vector bundles: tangent bundles, smooth sections, local frames, Riemannian metrics on bundles
- [x] `VectorField/` - Vector fields on manifolds: Lie brackets, pullbacks of vector fields

## Search Tags

manifold smooth-manifold charted-space structure-groupoid atlas chart diffeomorphism local-diffeomorphism immersion smooth-embedding bump-function partition-of-unity contmdiff mfderiv tangent-bundle lie-group vector-bundle riemannian bordism whitney-embedding poincare-conjecture holomorphic complex-manifold metrizable model-with-corners
