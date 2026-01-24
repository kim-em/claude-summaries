---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function/L1Space
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# L1Space

## Overview

The `L1Space/` directory defines integrable functions and the L¹ space of equivalence classes of integrable functions. It introduces the predicate `HasFiniteIntegral` for functions with finite integral (∫⁻ a, ‖f a‖ₑ < ∞), the predicate `Integrable` for almost everywhere strongly measurable functions with finite integral, and establishes the API between integrable functions and L¹ space (a special case of Lp spaces for p=1). This includes constructing L¹ functions from integrable functions, computing norms and distances in L¹, and proving basic properties like additivity, scalar multiplication, and dominated convergence.

## Key Files

| File | Purpose |
|------|---------|
| HasFiniteIntegral.lean | Definition of `HasFiniteIntegral f μ` (∫⁻ a, ‖f a‖ₑ < ∞), basic properties including monotonicity, measure operations, dominated convergence theorem for sequences, and relationship with summability for counting measure |
| Integrable.lean | Definition of `Integrable f μ` (AEStronglyMeasurable f μ ∧ HasFiniteIntegral f μ), equivalence with `MemLp 1`, monotonicity and congruence properties, dominated convergence for integrable functions, basic operations (addition, negation, scalar multiplication), and integration on subspaces |
| AEEqFun.lean | API between integrable functions and L¹ space: integrability for almost everywhere equal function classes, construction `Integrable.toL1` mapping integrable functions to L¹ elements, L¹ norm and distance formulas as Lebesgue integrals, measurability properties of L¹ functions |

## Subdirectories

(none)

## Search Tags

l1-space integrable has-finite-integral lebesgue-integral measure-theory normed-group ae-equal lp-space dominated-convergence finite-integral measurable-function
