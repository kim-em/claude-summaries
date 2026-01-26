---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Kernel/Composition
generated: 2026-01-26T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 13
subdirs_count: 0
---

# Composition

## Overview

The `Composition/` subdirectory implements kernel composition operations and related constructions in probability theory. This includes sequential composition (`η ∘ₖ κ`), parallel composition (`κ ∥ₖ η`), composition-product (`κ ⊗ₖ η`), and simple product (`κ ×ₖ η`) of kernels, along with their interaction with measure composition (`κ ∘ₘ μ`). The files provide both definitional infrastructure (notation, basic constructors) and theoretical properties (Lebesgue integrals, Bochner integrals, measurability, absolute continuity, Chapman-Kolmogorov equations for Markov chains).

## Key Files

| File | Purpose |
|------|---------|
| CompNotation.lean | Defines notation `κ ∘ₘ μ` for composition of a measure and a kernel (equivalent to `Measure.bind μ κ`), provides basic lemmas for deterministic kernels and identity |
| Comp.lean | Defines kernel composition `η ∘ₖ κ` (sequential application of kernels), proves Chapman-Kolmogorov equations, establishes monoid structure on `Kernel α α`, shows stability of kernel classes under composition |
| CompMap.lean | (Not fully read, but likely) Maps and comaps of composed kernels |
| CompProd.lean | Defines composition-product `κ ⊗ₖ η : Kernel α (β × γ)` for s-finite kernels, proves Lebesgue integral formula, establishes almost-everywhere properties, restriction lemmas, and stability of kernel classes |
| IntegralCompProd.lean | Proves Bochner integral equality for composition and composition-product (extends Lebesgue integral results to the full integral), shows integrability and measurability properties |
| KernelLemmas.lean | Collection of auxiliary kernel lemmas (likely used by MeasureComp and other composition files) |
| Lemmas.lean | General lemmas about kernel compositions (exact content not examined) |
| MapComap.lean | Defines `map` (pushforward along measurable function) and `comap` (pullback along measurable function) for kernels, proves Lebesgue integral formulas |
| MeasureComp.lean | Proves lemmas about composition `κ ∘ₘ μ` of a measure and a kernel, including associativity `(η ∘ₘ (κ ∘ₘ μ)) = ((η ∘ₖ κ) ∘ₘ μ)`, almost-everywhere properties, finiteness instances |
| MeasureCompProd.lean | (Imported by MeasureComp.lean, likely) Composition-product of a measure and a kernel |
| ParallelComp.lean | Defines parallel composition `κ ∥ₖ η : Kernel (α × γ) (β × δ)` that applies two kernels independently to components of a product space, proves product measure formula |
| Prod.lean | Defines product `κ ×ₖ η : Kernel α (β × γ)` of two kernels from the same source (special case: both kernels start from same space), implements via parallel composition and copy kernel |
| AbsolutelyContinuous.lean | Absolute continuity results for composition-products requiring `CountableOrCountablyGenerated` assumption, proves `μ ⊗ₘ κ ≪ ν ⊗ₘ η ↔ μ ≪ ν ∧ ∀ᵐ a ∂μ, κ a ≪ η a` |

## Subdirectories

(none)

## Search Tags

kernel-composition markov-kernels composition-product parallel-composition kernel-product measure-composition chapman-kolmogorov lebesgue-integral bochner-integral s-finite-kernels measurability absolute-continuity mutual-singularity map-comap pushforward-pullback notation almost-everywhere monoid-structure markov-chains
