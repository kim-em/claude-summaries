---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Kernel
generated: 2026-01-26T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 15
subdirs_count: 3
---

# Kernel

## Overview

The `Kernel/` directory provides a comprehensive formalization of Markov kernels (probability kernels) in measure theory. A kernel from measurable space α to β is a measurable map `α → Measure β`. This includes core definitions and classifications of kernels (Markov, finite, s-finite), basic kernel operations (deterministic, constant, identity, restriction, composition), kernel composition and product operations, disintegration theory for decomposing measures via kernels, Radon-Nikodym derivatives and Lebesgue decomposition for kernels, conditional distributions and regular conditional probability, posterior distributions (Bayesian inference), and the Ionescu-Tulcea theorem for constructing measures on infinite product spaces.

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

- [x] `Composition/` - Kernel composition operations and properties
- [ ] `Disintegration/` - Disintegration theory (decomposing measures into kernels)
- [ ] `IonescuTulcea/` - Ionescu-Tulcea theorem for constructing measures on infinite products

## Search Tags

markov-kernels probability-kernels measure-theory conditional-distribution conditional-expectation radon-nikodym lebesgue-decomposition disintegration kernel-composition bayesian-inference posterior conditional-probability regular-conditional-probability ionescu-tulcea markov-processes standard-borel deterministic-kernel finite-kernel s-finite-kernel
