---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed
generated: 2025-12-05T15:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 10
---

# Normed

## Overview

The `Normed/` directory establishes the complete foundational hierarchy for normed spaces in mathlib4, providing the essential infrastructure for all of functional analysis. It builds from the ground up: starting with normed groups (where distance is given by `dist x y = ‖x - y‖`), then normed rings (with submultiplicative norm `‖x * y‖ ≤ ‖x‖ * ‖y‖`), normed fields (with multiplicative norm `‖x * y‖ = ‖x‖ * ‖y‖`), and finally normed modules/spaces (requiring bounded scalar multiplication `‖a • b‖ ≤ ‖a‖ * ‖b‖`). The directory encompasses both the algebraic perspective (bounded homomorphisms, quotient norms, completeness) and the categorical perspective (`SemiNormedGrp` category with functorial completions). Major theoretical achievements include the Mazur-Ulam theorem, Gelfand-Mazur theorem, Gelfand's spectral radius formula, Hahn-Banach extension theorem, Banach-Alaoglu theorem, Riesz's lemma, Banach open mapping theorem, and Banach-Steinhaus uniform boundedness principle. The directory also provides comprehensive treatment of specialized topics: ultrametric/nonarchimedean norms, L^p spaces with Hölder's inequality, affine geometry (homotheties, barycentric coordinates, simplices), Banach algebras with spectrum theory and exponential maps, bounded linear operators with compact operator theory, ordered normed structures with solid norms, and unbundled seminorms for nonarchimedean analysis. This unified framework supports advanced applications including Banach space theory, operator algebras, differential geometry, and non-Archimedean analysis.

## Key Files

| File | Purpose |
|------|---------|
| MulAction.lean | Defines `IsBoundedSMul` over normed additive groups; proves norm inequalities for scalar multiplication (`‖r • x‖ ≤ ‖r‖ * ‖x‖`); provides `NormSMulClass` for strictly multiplicative norms; shows that non-unital seminormed rings have bounded left/right multiplication actions |

## Subdirectories

- [x] `Affine/` - Normed affine spaces (add torsors with norms, continuous affine maps, Mazur-Ulam theorem, asymptotic cones) (complete)
- [x] `Algebra/` - Normed algebras (Banach algebras, spectrum theory, exponential maps, Gelfand-Mazur theorem, unitization) (complete)
- [x] `Field/` - Normed fields and division rings (multiplicative norms, ultrametric fields, unit balls, absolute values, field completion) (complete)
- [x] `Group/` - Normed (additive) groups and their basic properties (seminorms, bounded sets, completeness, constructions, homomorphisms, categorical infrastructure) (complete)
- [x] `Lp/` - Lp spaces and norms (product and pi types with Lp norms, WithLp construction, Lp equivalences) (complete)
- [x] `Module/` - Normed modules and spaces over normed fields (basic properties, dual spaces, finite-dimensional spaces, Hahn-Banach, multilinear maps, tensor products) (complete)
- [x] `Operator/` - Bounded linear operators and continuous linear maps (operator norm, linear isometries, Banach open mapping theorem, Banach-Steinhaus uniform boundedness principle, compact operators, extension theorems) (complete)
- [x] `Order/` - Ordered normed structures (normed lattices, upper/lower sets, order homomorphisms) (complete)
- [x] `Ring/` - Normed rings (seminormed rings, submultiplicative norms, integer casts, units, ultrametric rings) (complete)
- [x] `Unbundled/` - Unbundled seminorms and norms (ring seminorms, algebra norms, spectral norms, smoothing seminorms) (complete)

## Search Tags

normed-spaces functional-analysis banach-spaces seminorms normed-groups normed-rings normed-fields normed-modules bounded-operators continuous-linear-maps lp-spaces affine-spaces normed-algebras spectrum-theory scalar-multiplication bounded-smul operator-theory dual-spaces hahn-banach finite-dimensional seminormed-groups ultrametric
