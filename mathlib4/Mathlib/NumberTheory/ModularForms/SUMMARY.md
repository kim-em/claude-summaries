---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/ModularForms
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 27
subdirs_count: 2
---

# ModularForms

## Overview

The `ModularForms/` directory provides a comprehensive formalization of classical modular form theory for the upper half-plane. It develops the foundational machinery (slash actions, invariant forms, arithmetic subgroups, congruence subgroups), defines modular forms and cusp forms with their boundedness properties, and establishes key results including q-expansion theory, Hecke bounds for cusp forms, the Petersson scalar product, and specific examples like Eisenstein series, Jacobi theta functions, and the Dedekind eta function. The implementation covers both the abstract theory (slash invariance, group actions, cusps) and concrete computational aspects (norm bounds, polynomial growth of coefficients).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of modular forms as slash-invariant forms that are bounded at cusps, plus construction of the graded ring structure |
| SlashActions.lean | General slash action framework: right actions of groups parametrized by weight k, with notation `f ∣[k] g` |
| SlashInvariantForms.lean | Functions invariant under slash actions, forming the base type for modular and cusp forms with module structure over ℝ and ℂ |
| ArithmeticSubgroups.lean | Definition and properties of arithmetic subgroups of GL(2, ℝ), including the typeclass for determinant ±1 condition |
| CongruenceSubgroups.lean | Principal congruence subgroups Γ(N), Γ₀(N), Γ₁(N) of SL(2, ℤ) with membership characterizations |
| Cusps.lean | Cusps as fixed points of parabolic elements in OnePoint ℝ, with transitivity results for SL(2, ℤ) action |
| BoundedAtCusp.lean | Definitions of "bounded at cusp c" and "vanishing at c" for functions on the upper half-plane |
| QExpansion.lean | q-expansion theory: cusp functions, convergence on the unit disc, power series coefficients, exponential decay of cusp forms |
| Bounds.lean | Norm bounds for modular forms (O(1/im^k)) and cusp forms (O(1/im^(k/2))), plus Hecke's bound O(n^(k/2)) for q-expansion coefficients |
| Petersson.lean | Petersson scalar product integrand and its slash-invariance properties |
| NormTrace.lean | Trace maps from ModularForm(𝒢 ⊓ ℋ, k) to ModularForm(ℋ, k) for finite index subgroups |
| LevelOne.lean | Results specific to level one (SL(2, ℤ)) modular forms including maximum principle and weight-zero characterization |
| DedekindEta.lean | Dedekind eta function as infinite product η(z) = q^(1/24) ∏(1 - q^(n+1)), proven non-vanishing and differentiable |
| Identities.lean | Collection of useful identities: periodicity under translations, S and T actions, width invariance for Γ(N) |

## Subdirectories

- [~] `EisensteinSeries/` - Eisenstein series definitions, convergence, q-expansions, and boundedness
- [ ] `JacobiTheta/` - Jacobi theta functions in one and two variables with bounds and manifold properties

## Search Tags

modular-forms slash-actions upper-half-plane congruence-subgroups eisenstein-series jacobi-theta dedekind-eta q-expansion cusps petersson-product hecke-bounds arithmetic-subgroups SL2Z level-one cusp-forms graded-ring
