---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/VectorBundle
generated: 2026-01-24T06:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# VectorBundle

## Overview

The `VectorBundle/` directory formalizes smooth (`C^n`) vector bundles over manifolds in Mathlib. It defines the `ContMDiffVectorBundle` mixin class stating that a topological vector bundle has `C^n` transition functions, and develops the theory of smooth sections, local frames, tangent bundles, and related constructions. The key insight is that a `C^n` vector bundle over a `C^n` manifold is itself a `C^n` manifold, with the total space inheriting a charted space structure from the trivializations. The library supports infinite differentiability indices and provides tools for analyzing smoothness of maps into and out of vector bundles.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `ContMDiffVectorBundle` class, charted space structure on fiber bundles, smoothness of coordinate changes, construction of `C^n` vector bundles from `VectorBundleCore` and `VectorPrebundle`, direct sums of `C^n` bundles |
| FiberwiseLinear.lean | Defines the structure groupoid `contMDiffFiberwiseLinear` of `C^n` fiberwise-linear open partial homeomorphisms, used to specify when coordinate changes are `C^n` |
| Tangent.lean | Constructs the tangent bundle as a `C^n` vector bundle using `tangentBundleCore`, defines `tangentCoordChange`, proves tangent bundle of a `C^{n+1}` manifold is `C^n` |
| SmoothSection.lean | Defines `ContMDiffSection` (bundled `C^n` sections), proves sections form a module over the base field, smoothness lemmas for sums/differences/scalar products of sections |
| MDifferentiable.lean | Characterizations of differentiability into vector bundles, operations on differentiable sections (add, sub, neg, smul, sum), locally finite sums of differentiable sections |
| Hom.lean | Shows the bundle of continuous linear maps `E₁ b →L[𝕜] E₂ b` is a `C^n` vector bundle when `E₁` and `E₂` are, smoothness of applying linear maps to sections |
| LocalFrame.lean | Local frames: `IsLocalFrameOn` predicate for families of sections forming a basis at each point, frame coefficients, smoothness of sections via frame coefficients, construction of local frames from trivializations |
| Riemannian.lean | Riemannian vector bundles: `IsContMDiffRiemannianBundle` class for bundles with smoothly varying inner product, smoothness of inner products of sections |
| Pullback.lean | Pullback bundles: if `E` is a `C^n` vector bundle and `f : B' → B` is `C^n`, then `f *ᵖ E` is a `C^n` vector bundle |

## Subdirectories

(none)

## Search Tags

vector-bundle contmdiff-vector-bundle smooth-vector-bundle tangent-bundle tangent-space smooth-section local-frame riemannian-bundle fiberwise-linear structure-groupoid coordinate-change trivialization pullback-bundle total-space fiber-bundle mdifferentiable
