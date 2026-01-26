---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Kernel
generated: 2026-01-26T23:40:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 15
subdirs_count: 3
---

# Kernel

## Overview

The `Kernel/` directory provides a comprehensive formalization of Markov kernels (probability kernels) in measure theory. A kernel from measurable space α to β is a measurable map `α → Measure β`. The directory establishes the foundational theory including core definitions and classifications (Markov, finite, s-finite kernels), basic kernel constructors (deterministic, constant, identity, restriction), and several major theoretical components. The Composition subdirectory implements sequential composition (`η ∘ₖ κ`), parallel composition (`κ ∥ₖ η`), composition-product (`κ ⊗ₖ η`), and simple product (`κ ×ₖ η`), with Chapman-Kolmogorov equations for Markov chains. The Disintegration subdirectory provides the full theory of decomposing measures on product spaces into marginals and conditional kernels (`ρ = ρ.fst ⊗ₘ ρ.condKernel`), proved for standard Borel spaces using conditional CDFs, martingale convergence for densities, and measurable embeddings into ℝ. The IonescuTulcea subdirectory constructs measures on infinite product spaces from sequences of history-dependent kernels via Carathéodory extension, providing the foundation for defining Markov processes and stochastic processes. The core files cover Radon-Nikodym derivatives and Lebesgue decomposition for kernels, regular conditional probability distributions, posterior distributions for Bayesian inference, integration and measurability of kernel integrals, and invariance and irreducibility properties.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Kernel α β` as measurable map `α → Measure β`, defines kernel classes: `IsMarkovKernel` (probability measures), `IsFiniteKernel` (uniform bound on total mass), `IsSFiniteKernel` (countable sum of finite kernels) |
| Basic.lean | Basic kernel constructors: `deterministic` (Dirac measures), `id` (identity kernel), `copy`, `discard`, `swap`, `const` (constant kernel), `restrict` (restriction to sets), `comapRight`, `piecewise`, `ofFunOfCountable`, `boolKernel` |
| CompProdEqIff.lean | Equivalence conditions for composition-product equality of kernels |
| CondDistrib.lean | Regular conditional probability distribution `condDistrib Y X μ` for random variables Y given X in standard Borel spaces, satisfies `μ⟦Y⁻¹' s \| X⟧ = condDistrib Y X μ (X ·) s` almost everywhere |
| Condexp.lean | Kernel associated with conditional expectation: `condExpKernel μ m` satisfies `μ[f \| m] =ᵐ[μ] fun ω => ∫ y, f y ∂(condExpKernel μ m ω)` for integrable f |
| Integral.lean | Integration with respect to kernels |
| Invariance.lean | Invariance properties of kernels under transformations |
| Irreducible.lean | Irreducibility theory for Markov kernels |
| MeasurableIntegral.lean | Measurability of kernel integrals with respect to the Bochner integral |
| MeasurableLIntegral.lean | Measurability of kernel Lebesgue integrals (lintegral) |
| Posterior.lean | Posterior kernel `κ†μ` for Bayesian inference: given prior measure μ and likelihood kernel κ, satisfies `(κ ∘ₘ μ) ⊗ₘ κ†μ = (μ ⊗ₘ κ).map Prod.swap`, includes `posterior_eq_withDensity` theorem |
| Proper.lean | Proper kernels (kernels that are tight in the sense of probability theory) |
| RadonNikodym.lean | Radon-Nikodym derivative `rnDeriv κ η` and Lebesgue decomposition for kernels: `κ = withDensity η (rnDeriv κ η) + singularPart κ η`, includes measurability of sets `{a \| κ a ≪ η a}` and `{a \| κ a ⟂ₘ η a}` |
| SetIntegral.lean | Set integration with respect to kernels |
| WithDensity.lean | Kernel with density: `withDensity κ f` maps `a ↦ (κ a).withDensity (f a)`, satisfies `∫⁻ b, g b ∂(withDensity κ f a) = ∫⁻ b, f a b * g b ∂(κ a)` |

## Subdirectories

- [x] `Composition/` - Sequential, parallel, composition-product, and simple product operations with Chapman-Kolmogorov equations, absolute continuity, and integration formulas
- [x] `Disintegration/` - Decomposition of measures into marginals and conditional kernels for standard Borel spaces using CDFs, density via martingale convergence, and uniqueness theorems
- [x] `IonescuTulcea/` - Construction of measures on infinite product spaces from sequences of history-dependent kernels via Carathéodory extension for Markov processes

## Search Tags

markov-kernels probability-kernels measure-theory conditional-distribution conditional-expectation radon-nikodym lebesgue-decomposition disintegration kernel-composition bayesian-inference posterior conditional-probability regular-conditional-probability ionescu-tulcea markov-processes standard-borel deterministic-kernel finite-kernel s-finite-kernel
