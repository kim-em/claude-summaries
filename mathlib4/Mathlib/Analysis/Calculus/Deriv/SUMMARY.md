---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Calculus/Deriv
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 20
subdirs_count: 0
---

# Deriv

## Overview

The `Deriv/` directory formalizes one-dimensional derivatives for functions `f : 𝕜 → F` where `𝕜` is a normed field (typically ℝ or ℂ) and `F` is a normed space over `𝕜`. This provides the classical notion of derivatives via predicates like `HasDerivAt` and `HasDerivWithinAt`, defined in terms of the Fréchet derivative. The directory includes fundamental derivative rules (sum, product, quotient, chain rule), specific derivatives for elementary functions (powers, polynomials, absolute value), mean value theorems, and the connection to the undergraduate definition via slopes. These are the one-dimensional specializations of the more general Fréchet derivative theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of one-dimensional derivatives: `HasDerivAt`, `HasDerivWithinAt`, `HasDerivAtFilter`, `HasStrictDerivAt` predicates and `deriv`, `derivWithin` functions; shows these coincide with Fréchet derivatives via `fderiv`; includes derivatives of constants and identity |
| Slope.lean | Proves equivalence between derivative and the limit of the slope `(f y - f x) / (y - x)` as `y → x` (excluding `x`); connects formal derivative definition to undergraduate calculus definition; includes estimates on upper/lower limits of slopes |
| Comp.lean | Chain rule for compositions: `f : 𝕜' → 𝕜'` with `g : 𝕜 → 𝕜'` (scalar-scalar), `f : 𝕜' → E` with `g : 𝕜 → 𝕜'` (scalar-vector via `scomp`), and `f : E → F` with `g : 𝕜 → E` (vector-scalar); includes `of_eq` variants for non-definitional equality |
| Add.lean | Derivative rules for addition, negation, subtraction, and finite sums `∑ i, f i x`; proves `(f + g)' = f' + g'` and similar for all notions of derivative |
| Mul.lean | Product rule for multiplication: derivatives of `f x * g x` (scalar multiplication and bilinear products); proves `(f * g)' = f' * g + f * g'` and scalar multiplication variants |
| Inv.lean | Derivative rules for inverse `x ↦ x⁻¹` and division; proves `(x⁻¹)' = -1/x²` and quotient rule `(f/g)' = (f'g - fg')/g²` for fields |
| Pow.lean | Derivatives of natural number powers `x ↦ f x ^ n`; proves power rule `(fⁿ)' = n·f^(n-1)·f'`; includes non-commutative version with sum formula |
| ZPow.lean | Derivatives of integer powers `x ↦ x^m` for `m : ℤ`; extends power rule to negative exponents using inverse derivatives |
| Polynomial.lean | Proves analysis derivatives of polynomials agree with algebraic polynomial derivatives; connects `Polynomial.derivative` to `deriv` |
| Linear.lean | Derivatives of continuous linear maps `f : 𝕜 →L[𝕜] E` and bundled linear maps; proves derivative is `f 1` (evaluation at 1) |
| AffineMap.lean | Derivatives of affine maps `f : 𝕜 →ᵃ[𝕜] E`; proves derivative is `f.linear 1`; includes specialized results for `lineMap` used to transfer one-dimensional MVT to higher dimensions |
| MeanValue.lean | Cauchy's and Lagrange's mean value theorems: existence of `c ∈ (a,b)` with `f' c = (f b - f a)/(b - a)`; derives monotonicity from derivative sign (`strictMono_of_deriv_pos`, etc.) and bounds on function differences from derivative bounds |
| Abs.lean | Derivative of absolute value `\|x\|` on ℝ; proves differentiability away from zero and smoothness properties for `\|f x\|` when `f x ≠ 0` |
| Prod.lean | Derivatives of functions taking values in product types `𝕜 → E × F` and `𝕜 → Π i, E i`; proves component-wise differentiation |
| Pi.lean | One-dimensional derivatives on pi-types; derivatives of `Function.update` and `Pi.single` for functions to finite products |
| Star.lean | Derivatives of star operation (complex conjugation): `(star ∘ f)' = star f'` when base field has trivial star; includes `conj ∘ f ∘ conj` for non-trivial star (ℂ) |
| Shift.lean | Translation invariance of derivatives: if `f` has derivative `f'` at `a + x`, then `f(a + ·)` has derivative `f'` at `x`; includes variants for `a + x`, `x + a`, `a - x`, `x - a` |
| Support.lean | Support properties: proves `support(deriv f) ⊆ tsupport f`, so derivatives of compactly supported functions have compact support |
| CompMul.lean | Derivative of `x ↦ f(cx)` equals `c` times derivative of `f` at `cx`; scaling in domain scales derivative |
| Inverse.lean | Easy half of inverse function theorem: if `f` has nonzero strict derivative at `x` and `g` is a local continuous left inverse, then `g'(f x) = (f' x)⁻¹`; harder half (existence of inverse) is in parent directory's `InverseFunctionTheorem/` |

## Subdirectories

(No subdirectories)

## Search Tags

one-dimensional-derivative deriv has-deriv-at deriv-within slope chain-rule product-rule quotient-rule power-rule polynomial-derivative mean-value-theorem cauchy-mvt lagrange-mvt monotonicity-from-derivative strict-monotone affine-derivative linear-derivative inverse-derivative absolute-value-derivative translation-invariance compact-support composition scalar-derivative real-derivative complex-derivative
