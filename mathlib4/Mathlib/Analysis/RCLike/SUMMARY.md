---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/RCLike
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 6
subdirs_count: 0
---

# RCLike

## Overview

The `RCLike/` directory provides a typeclass abstraction for fields that behave like either ℝ (real numbers) or ℂ (complex numbers). The `RCLike` typeclass captures properties shared by both fields with an API closely matching that of ℂ, allowing definitions and theorems to be written once and applied to both real and complex cases. This is particularly valuable for defining inner products and Hilbert spaces generically. The directory includes the core typeclass definition, extensions of real-linear maps to RCLike-linear maps, weighted inner products, additional lemmas requiring heavier imports, bounded continuous functions with RCLike values, and relationships between unique differentiability over ℝ and ℂ.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the `RCLike` typeclass with two instances (ℝ and ℂ); includes real/imaginary part functions, imaginary unit I, conjugation, norm squared, and partial order; main abstraction for treating real and complex numbers uniformly |
| Extend.lean | Extends ℝ-linear functionals to 𝕜-linear functionals for RCLike 𝕜; provides `LinearMap.extendTo𝕜` and `ContinuousLinearMap.extendTo𝕜` with the formula `fc x = fr x - fr (I • x) * I` |
| Inner.lean | Defines weighted L2 inner product `wInner` for finite sequences `f g : ι → R` as `∑ i, conj (f i) * g i` (conjugation on left); includes discrete and compact variants with notation `⟪f, g⟫_[𝕜, w]` |
| Lemmas.lean | Additional lemmas about RCLike requiring heavier imports (finite-dimensional modules, real vector spaces); proves convexity equivalence between K and ℝ, polynomial evaluation, span of {1, I} is whole space, and rank bound ≤ 2 |
| BoundedContinuous.lean | Results on bounded continuous functions with RCLike values; proves commutativity of "restrict scalars to ℝ" and "forget boundedness" operations on star subalgebras |
| TangentCone.lean | Relationships between unique differentiability over ℝ and ℂ; proves that unique differentiability sets for ℝ are also unique differentiability sets for ℂ, with applications to convex sets |

## Subdirectories

(none)

## Search Tags

rclike real complex abstraction typeclass inner-product hilbert-space linear-functional extension weighted-inner-product l2-norm bounded-continuous tangent-cone unique-differentiability convexity normed-field finite-dimensional conjugation imaginary-unit
