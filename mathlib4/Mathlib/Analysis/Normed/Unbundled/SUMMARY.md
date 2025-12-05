---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Unbundled
generated: 2025-12-05T08:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 9
subdirs_count: 0
---

# Unbundled

## Overview

The `Unbundled/` directory provides an alternative "unbundled" approach to seminorms and norms on rings and algebras, where the norm is treated as a standalone function rather than packaged with algebraic structure. This directory contains the theoretical foundations for working with multiple (semi)norms on the same ring, focusing on nonarchimedean analysis. It includes fundamental constructions for ring seminorms, algebra norms, smoothing seminorms, spectral norms, and various norm extension theorems from non-Archimedean analysis literature (particularly Bosch-Güntzer-Remmert).

## Key Files

| File | Purpose |
|------|---------|
| RingSeminorm.lean | Core definitions of ring seminorms and norms (subadditive, submultiplicative functions preserving zero and negation); includes multiplicative variants equivalent to absolute values |
| AlgebraNorm.lean | Algebra norms on R-algebras (ring norms compatible with scalar multiplication); includes multiplicative algebra norms |
| SpectralNorm.lean | Spectral norm construction and norm extension theorem for algebraic extensions of nonarchimedean fields; proves unique extension of p-adic norms to algebraic closures |
| SmoothingSeminorm.lean | Smoothing construction (BGR Prop 1.3.2/1): converts nonarchimedean seminorms to power-multiplicative ones via `iInf (μ(x^n))^(1/n)`; proves convergence and nonarchimedean preservation |
| SeminormFromBounded.lean | Constructs ring seminorms from multiplicatively bounded group seminorms (BGR Prop 1.2.1/2); creates seminorm via supremum `sup_y f(xy)/f(y)` |
| SeminormFromConst.lean | Constructs power-multiplicative seminorms from existing ones by making a constant multiplicative (BGR Prop 1.3.2/2); uses limit of `f(x·c^n)/(f c)^n` |
| FiniteExtension.lean | Basis.norm construction for finite extensions (BGR Lemma 3.2.1/3); proves existence of power-multiplicative K-algebra norms on finite extensions of nonarchimedean fields |
| InvariantExtension.lean | Algebra norm constructions invariant under field automorphisms; `algNormOfAlgEquiv` and `invariantExtension` (maximum over all automorphisms); proves power-multiplicativity and nonarchimedean properties |
| IsPowMulFaithful.lean | Equivalent power-multiplicative norms (BGR Prop 3.1.5/1); proves uniqueness: if two power-multiplicative algebra norms agree on all subrings R[y], they are equal |

## Subdirectories

*(none)*

## Search Tags

unbundled-norms ring-seminorm algebra-norm spectral-norm nonarchimedean power-multiplicative smoothing-seminorm norm-extension finite-extension invariant-extension multiplicatively-bounded bosch-guntzer-remmert BGR non-archimedean-analysis ultrametric p-adic algebraic-extension field-automorphism
