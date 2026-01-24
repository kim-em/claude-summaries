---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold
generated: 2026-01-24T23:15:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 24
subdirs_count: 10
---

# Manifold

## Overview

The `Manifold/` directory contains Mathlib's comprehensive formalization of smooth manifolds and differential geometry. The architecture is built on three foundational abstractions: **structure groupoids** (sets of open partial homeomorphisms closed under composition and inverse that specify which coordinate changes are allowed), **charted spaces** (topological spaces with atlases of charts to a model space), and **models with corners** (embeddings of model spaces like half-spaces into normed vector spaces that enable manifolds with boundary).

The core smoothness infrastructure lives in `ContMDiff/`, which defines `ContMDiff`, `ContMDiffAt`, and related predicates for C^n maps between manifolds. These leverage a local invariant properties framework to lift smoothness from model spaces to manifolds in a coordinate-independent way. The manifold derivative (`MFDeriv/`) extends the Fréchet derivative to manifolds, working through extended charts into the model vector space.

Geometric structures are built atop this foundation: `VectorBundle/` formalizes smooth vector bundles with C^n transition functions, including the tangent bundle construction; `VectorField/` provides vector fields with Lie brackets and pullbacks; `Riemannian/` defines Riemannian metrics where distance equals the infimum of path lengths; and `IntegralCurve/` formalizes integral curves of vector fields with existence/uniqueness theorems via Picard-Lindelöf.

Algebraic structures on manifolds are developed in `Algebra/`, defining Lie groups (smooth manifolds with smooth group operations), smooth monoids/rings, and left-invariant derivations that model Lie algebras. The sheaf-theoretic perspective in `Sheaf/` shows that smooth manifolds are locally ringed spaces with the structure sheaf of smooth functions.

Concrete instances in `Instances/` include: real manifolds with half-spaces and quadrants for boundaries, closed intervals [x,y] as 1-dimensional manifolds with boundary, unit spheres via stereographic projection, and units of complete normed algebras (including GL(n)) as Lie groups.

Notable results at this level include: bump functions and smooth partitions of unity, the Whitney embedding theorem (compact manifolds embed in Euclidean space), metrizability of finite-dimensional σ-compact manifolds, smooth approximation of continuous functions, diffeomorphisms and local diffeomorphisms, immersions and smooth embeddings, holomorphic functions on complex manifolds with maximum modulus principle, bordism theory foundations, and the statement of the generalized Poincaré conjecture.

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

- [x] `Algebra/` - Lie groups (`LieGroup`), smooth monoids (`ContMDiffMul`), smooth rings (`ContMDiffRing`), left-invariant derivations, and smooth functions as algebras
- [x] `ContMDiff/` - Core `ContMDiff`/`ContMDiffAt` definitions and properties: composition, products, sums, atlas smoothness, equivalence with `ContDiff` for vector spaces
- [x] `Instances/` - Concrete manifolds: real line, intervals `[x,y]` with boundary, spheres via stereographic projection, circle as Lie group, GL(n) and units of normed algebras
- [x] `IntegralCurve/` - Integral curves of vector fields: `IsMIntegralCurve` definitions, local existence/uniqueness via Picard-Lindelöf, translation/scaling transforms, uniform time lemma
- [x] `IsManifold/` - `IsManifold` typeclass, `ModelWithCorners` structure, extended charts `extChartAt`, manifold interior/boundary, `BoundarylessManifold`
- [x] `MFDeriv/` - Manifold Fréchet derivative: `mfderiv`, `MDifferentiableAt`, `HasMFDerivAt`, chain rule, specific function derivatives, unique differentiability
- [x] `Riemannian/` - Riemannian manifolds: `IsRiemannianManifold` typeclass, path length via derivative norm integral, `riemannianEDist` as infimum of path lengths
- [x] `Sheaf/` - Sheaves of smooth functions, `smoothSheaf` construction, locally ringed space structure on manifolds, stalks as local rings
- [x] `VectorBundle/` - Smooth vector bundles: `ContMDiffVectorBundle`, tangent bundle construction, smooth sections, local frames, Hom bundles, pullback bundles, Riemannian bundles
- [x] `VectorField/` - Vector fields: pullback under smooth maps (`mpullback`), Lie bracket (`mlieBracket`), Jacobi identity, bracket preservation under pullback

## Search Tags

manifold smooth-manifold charted-space structure-groupoid atlas chart diffeomorphism local-diffeomorphism immersion smooth-embedding bump-function partition-of-unity contmdiff contmdiffat mfderiv mdifferentiable tangent-bundle tangent-space lie-group lie-algebra vector-bundle smooth-section local-frame riemannian-manifold bordism whitney-embedding poincare-conjecture holomorphic complex-manifold metrizable model-with-corners extchartat integral-curve vector-field lie-bracket pullback sheaf locally-ringed-space
