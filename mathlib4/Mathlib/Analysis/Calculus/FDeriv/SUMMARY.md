---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/FDeriv
generated: 2025-12-04T08:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 24
subdirs_count: 0
---

# FDeriv

## Overview

The `FDeriv/` directory contains the formalization of Fréchet derivatives in normed spaces. It defines the fundamental notion of differentiability (`HasFDerivAt`, `HasFDerivWithinAt`, `HasStrictFDerivAt`) and provides derivative formulas for all standard operations: constants, linear maps, bilinear maps, addition, multiplication, composition (chain rule), products, and equivalences. The directory also establishes the relationship between Fréchet derivatives and analytic functions, proving that analytic functions are differentiable with derivatives given by their power series. This is the core multivariable differentiation library in Mathlib, providing both theoretical foundations (uniqueness, continuity, asymptotic characterizations) and practical computation rules.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines the three main notions of differentiability: `HasFDerivAtFilter` (derivative along a filter), `HasFDerivWithinAt` (derivative within a set), `HasFDerivAt` (derivative at a point), and `HasStrictFDerivAt` (strict differentiability for inverse function theorem); also defines `DifferentiableAt`, `DifferentiableOn`, `Differentiable`, and computable derivative functions `fderiv` and `fderivWithin` |
| Basic.lean | Proves fundamental properties of Fréchet derivatives: uniqueness on sets with unique differentials, characterization via tendsto and little-o, monotonicity properties, relationship between different notions (strict → has derivative → differentiable), continuity of differentiable functions, derivatives of identity function, mean value inequality converse, and differentiability on unions of open sets |
| Analytic.lean | Proves that functions with power series expansions are differentiable, with derivatives given by the derivative series; establishes that analytic functions have all iterated derivatives; proves that continuous multilinear maps are smooth with explicit formulas for iterated derivatives; includes the inverse of analytic functions (via open partial homeomorphisms) |
| Comp.lean | Chain rule: proves that composition of differentiable functions is differentiable, with derivative given by composition of derivatives; includes versions for different combinations of `HasFDerivAt`, `HasFDerivWithinAt`, `HasStrictFDerivAt`, and `DifferentiableAt/On` |
| Add.lean | Derivative formulas for additive operations: sum of two functions, sum of finitely many functions, multiplication by scalar constant, negation, subtraction; proves these operations preserve all forms of differentiability |
| Linear.lean | Proves that continuous linear maps are differentiable everywhere with derivative equal to themselves; includes strict differentiability and differentiability at/within/on variants |
| Const.lean | Proves that constant functions have zero derivative everywhere |
| Bilinear.lean | Derivative formulas for bilinear maps: proves `(f g)' = f' g + f g'` (product rule for bilinear maps); includes composition with bilinear maps |
| Mul.lean | Derivative formulas for multiplication and division of functions: product rule, quotient rule, inverse function derivative, power functions; specific to scalar-valued or algebra-valued functions |
| Prod.lean | Derivative formulas for product spaces: proves `(f, g)'(v) = (f'(v), g'(v))`; includes projections, pairing, and equivalence between differentiability of pair and differentiability of components |
| Equiv.lean | Derivative formulas for continuous linear equivalences: proves that linear isomorphisms are differentiable with derivative equal to the isomorphism; shows that composing with an isomorphism preserves differentiability; includes formula for derivative of inverse function (given the inverse exists) |
| Measurable.lean | Proves that Fréchet derivatives are strongly measurable and (ae)measurable under appropriate conditions; includes measurability of `fderiv` and `fderivWithin` as functions |
| Extend.lean | Derivative of extension by constant outside a set |
| Norm.lean | Derivative of the norm function (where differentiable); proves norm is differentiable away from zero |
| Pow.lean | Derivative formulas for power functions `x ↦ x^n` in normed algebras |
| Symmetric.lean | Symmetric differentiability: a function is symmetric differentiable at a point if it has the same derivative from both sides; useful for studying functions on intervals |
| Star.lean | Derivative of the star (conjugation) operation in star algebras |
| RestrictScalars.lean | Derivative under restriction of scalars (change of base field) |
| ContinuousAlternatingMap.lean | Derivatives involving continuous alternating multilinear maps |
| ContinuousMultilinearMap.lean | Derivatives involving continuous multilinear maps (beyond what's in Analytic.lean) |
| Congr.lean | Congruence lemmas: if functions agree on a neighborhood, their derivatives agree |
| CompCLM.lean | Composition with continuous linear maps (specialized version of chain rule) |
| Pi.lean | Derivative formulas for functions into product types `Π i, E i` |
| WithLp.lean | Derivative formulas for functions involving `WithLp` (same type with different norm) |

## Subdirectories

(none)

## Search Tags

frechet-derivative multivariable-calculus differentiable chain-rule product-rule quotient-rule derivatives analytic-functions power-series composition bilinear-maps continuous-linear-maps normed-spaces functional-analysis mean-value-theorem strict-differentiability tangent-cone unique-differentiability asymptotic-analysis little-o big-o inverse-function measurable-derivatives iterated-derivatives smooth-functions multilinear-maps
