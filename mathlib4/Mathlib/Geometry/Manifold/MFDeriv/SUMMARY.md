---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Geometry/Manifold/MFDeriv
generated: 2026-01-24T09:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# MFDeriv

## Overview

The `MFDeriv/` directory contains the formalization of the manifold Fréchet derivative (`mfderiv`) in Mathlib. This is the generalization of the classical Fréchet derivative to maps between smooth manifolds. The derivative is defined by reading functions in extended charts and taking the ordinary Fréchet derivative in the model vector space. The directory provides the core definitions (`MDifferentiableAt`, `MDifferentiableWithinAt`, `mfderiv`, `mfderivWithin`, `HasMFDerivAt`, `HasMFDerivWithinAt`), along with basic properties mimicking the API for Fréchet derivatives, the chain rule, derivatives of specific functions (identity, constants, products, arithmetic operations), and unique differentiability conditions for subsets of manifolds.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `MDifferentiableAt`, `MDifferentiableWithinAt`, `mfderiv`, `mfderivWithin`, `HasMFDerivAt`, `HasMFDerivWithinAt`, `tangentMap`, `UniqueMDiffOn`, `UniqueMDiffWithinAt` |
| Basic.lean | Basic properties of unique differentiability sets, relating manifold differentiability to extended charts, deducing differentiability from smoothness, congruence lemmas, and the chain rule |
| FDeriv.lean | Equivalence between `mfderiv`/`mfderivWithin` and the usual Fréchet derivative `fderiv`/`fderivWithin` for functions between vector spaces |
| SpecificFunctions.lean | Differentiability and derivatives of specific functions: identity, constants, products (`Prod.fst`, `Prod.snd`, `Prod.map`), disjoint unions (`Sum.inl`, `Sum.inr`, `Sum.swap`), and arithmetic operations (addition, subtraction, negation, scalar multiplication, multiplication, sums, products) |
| Atlas.lean | Differentiability of charts, models with corners, and extended charts; shows that differentiable partial homeomorphisms have bijective derivatives; composition lemmas for extChartAt derivatives |
| NormedSpace.lean | Differentiability for functions into normed spaces: composition with differentiable functions, continuous linear map operations (precomp, postcomp, comp, apply, prodMap), continuous linear equivalences (arrowCongr), and scalar multiplication |
| Tangent.lean | Properties requiring the tangent bundle structure: tangent map formulas for charts, coordinate change identities, and the diffeomorphism `tangentBundleModelSpaceDiffeomorph` between the tangent bundle of the model space and the product |
| UniqueDifferential.lean | Properties of unique differentiability sets: preservation under images with dense-range derivatives, preservation under local diffeomorphisms and extended charts, and unique differentiability for preimages under fiber bundle projections |

## Subdirectories

(No subdirectories)

## Search Tags

mfderiv manifold-derivative mdifferentiable mdifferentiableat mdifferentiablewithinat hasmfderivat hasmfderivwithinat mfderivwithin tangent-map unique-mdiff chain-rule fderiv extended-chart coordinate-change differentiable-manifold frechet-derivative tangent-space
