---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed
generated: 2025-12-05T08:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 1
subdirs_count: 10
---

# Normed

## Overview

The `Normed/` directory contains the foundational algebraic structures for normed spaces in mathlib4. It provides the basic definitions and theory for normed groups, rings, fields, modules, and their various algebraic constructions. This directory serves as the core infrastructure for functional analysis, defining classes like `SeminormedAddGroup`, `NormedRing`, `NormedField`, and `NormedSpace`, along with bounded scalar multiplication (`IsBoundedSMul`) and norm multiplicativity properties. It includes specialized subdirectories for normed algebras, operators (bounded linear maps), Lp spaces, affine spaces, and unbundled seminorms.

## Key Files

| File | Purpose |
|------|---------|
| MulAction.lean | Defines `IsBoundedSMul` over normed additive groups; proves norm inequalities for scalar multiplication (`‖r • x‖ ≤ ‖r‖ * ‖x‖`); provides `NormSMulClass` for strictly multiplicative norms; shows that non-unital seminormed rings have bounded left/right multiplication actions |

## Subdirectories

- [ ] `Affine/` - Normed affine spaces (add torsors with norms, continuous affine maps, Mazur-Ulam theorem, asymptotic cones) (pending)
- [ ] `Algebra/` - Normed algebras (Banach algebras, spectrum theory, exponential maps, Gelfand-Mazur theorem, unitization) (pending)
- [ ] `Field/` - Normed fields and division rings (multiplicative norms, ultrametric fields, unit balls, absolute values) (pending)
- [ ] `Group/` - Normed (additive) groups and their basic properties (seminorms, bounded sets, completeness, constructions, homomorphisms) (pending)
- [ ] `Lp/` - Lp spaces and norms (product and pi types with Lp norms, WithLp construction, Lp equivalences) (pending)
- [ ] `Module/` - Normed modules and spaces over normed fields (basic properties, dual spaces, finite-dimensional spaces, Hahn-Banach, multilinear maps, tensor products) (pending)
- [ ] `Operator/` - Bounded linear operators and continuous linear maps (composition, completeness, compactness, Banach-Steinhaus theorem) (pending)
- [ ] `Order/` - Ordered normed structures (normed lattices, upper/lower sets, order homomorphisms) (pending)
- [ ] `Ring/` - Normed rings (seminormed rings, submultiplicative norms, integer casts, units, ultrametric rings) (pending)
- [ ] `Unbundled/` - Unbundled seminorms and norms (ring seminorms, algebra norms, spectral norms, smoothing seminorms) (pending)

## Search Tags

normed-spaces functional-analysis banach-spaces seminorms normed-groups normed-rings normed-fields normed-modules bounded-operators continuous-linear-maps lp-spaces affine-spaces normed-algebras spectrum-theory scalar-multiplication bounded-smul operator-theory dual-spaces hahn-banach finite-dimensional seminormed-groups ultrametric
