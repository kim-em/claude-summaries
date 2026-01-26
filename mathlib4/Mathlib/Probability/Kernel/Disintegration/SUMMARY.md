---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Kernel/Disintegration
generated: 2026-01-26T22:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Disintegration

## Overview

The `Disintegration/` directory provides the complete theory of measure and kernel disintegration in probability theory. Disintegration decomposes a measure on a product space `α × Ω` into a marginal measure on `α` and a conditional kernel from `α` to `Ω`, satisfying `ρ = ρ.fst ⊗ₘ ρ.condKernel`. This construction is fundamental for conditional probability and is proven to exist for standard Borel spaces. The implementation proceeds by first handling the real line case using conditional CDFs (cumulative distribution functions), then extending to arbitrary standard Borel spaces via measurable embeddings into ℝ. The directory includes tools for building measurable Stieltjes functions (CDFs), converting them to kernels, computing kernel densities via martingale convergence, proving uniqueness of conditional kernels, and computing integrals with respect to conditional kernels.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core disintegration predicates: `Measure.IsCondKernel ρ ρCond` (measure disintegration `ρ.fst ⊗ₘ ρCond = ρ`) and `Kernel.IsCondKernel κ κCond` (kernel disintegration `κ.fst ⊗ₖ κCond = κ`), includes `condKernelCountable` for countable spaces |
| CDFToKernel.lean | Builds Markov kernels from conditional CDFs: defines `IsCondKernelCDF` for functions `f : α × β → StieltjesFunction ℝ` satisfying integral conditions, defines `IsRatCondKernelCDF` for rational CDFs `f : α × β → ℚ → ℝ`, provides `toKernel` construction and proves `ν ⊗ₖ hf.toKernel f = κ` |
| CondCDF.lean | Conditional cumulative distribution functions for measures on `α × ℝ`: defines `condCDF ρ : α → ℝ → ℝ` with monotonicity and limit properties, defines auxiliary measure `IicSnd r` satisfying `ρ.IicSnd r s = ρ (s ×ˢ Iic r)`, proves integral formula `∫⁻ a in s, ENNReal.ofReal (condCDF ρ a x) ∂ρ.fst = ρ (s ×ˢ Iic x)` |
| Density.lean | Kernel density construction via martingale convergence: for `κ : Kernel α (γ × β)` with `κ.fst ≤ ν`, builds `density κ ν : α → γ → Set β → ℝ` satisfying `∫ x in A, density κ ν a x s ∂(ν a) = (κ a).real (A ×ˢ s)`, uses countable partition filtration and Doob's L1 convergence theorem, defines intermediate `densityProcess` martingale for each partition level |
| Integral.lean | Integration formulas for conditional kernels: proves `∫ b, ∫ ω, f (b, ω) ∂(Kernel.condKernel κ (a, b)) ∂(Kernel.fst κ a) = ∫ x, f x ∂(κ a)` for both Lebesgue and Bochner integrals, includes set integral versions and integrability criteria for functions involving `condKernel` |
| MeasurableStieltjes.lean | Measurable parametric Stieltjes functions: builds measurable `α → StieltjesFunction ℝ` from measurable `α → ℚ → ℝ`, defines `IsRatStieltjesPoint f a` (monotonicity, limits, right-continuity), defines `IsMeasurableRatCDF f` (measurable with Stieltjes property everywhere), provides `toRatCDF` and `stieltjesOfMeasurableRat` to extend rational CDFs to full Stieltjes functions |
| StandardBorel.lean | Main existence theorem for standard Borel spaces: defines `Kernel.condKernel κ : Kernel (α × β) Ω` and `Measure.condKernel ρ : Kernel β Ω` for standard Borel `Ω`, proves `fst κ ⊗ₖ condKernel κ = κ` and `ρ.fst ⊗ₘ ρ.condKernel = ρ`, works under `CountableOrCountablyGenerated α β` assumption (either `α` countable or `β` countably generated), constructs conditional kernel for ℝ using density and CDFs, then extends to arbitrary standard Borel via `embeddingReal` |
| Unique.lean | Almost everywhere uniqueness of conditional kernels: proves `eq_condKernel_of_measure_eq_compProd` (finite kernel satisfying disintegration is a.e. equal to `condKernel`), proves `eq_condKernel_of_kernel_eq_compProd` (uniqueness for kernel conditional kernels), proves `condKernel_apply_eq_condKernel` (kernel and measure conditional kernels coincide a.e.) |

## Subdirectories

(No subdirectories)

## Search Tags

disintegration conditional-kernel conditional-cdf cumulative-distribution-function standard-borel markov-kernel measure-disintegration kernel-disintegration stieltjes-function measurable-cdf density-process martingale-convergence radon-nikodym countably-generated conditional-probability product-measure kernel-composition uniqueness-ae almost-everywhere-unique doob-convergence
