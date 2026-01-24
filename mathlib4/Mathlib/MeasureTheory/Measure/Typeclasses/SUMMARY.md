---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Measure/Typeclasses
generated: 2026-01-25T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Typeclasses

## Overview

The `Typeclasses/` directory defines typeclass-based classifications of measures in mathlib4's measure theory framework. These typeclasses provide a systematic hierarchy for describing key measure properties: finite measures (`IsFiniteMeasure`, `IsLocallyFiniteMeasure`, `IsFiniteMeasureOnCompacts`), s-finite measures (`SFinite`, `SigmaFinite`), probability measures (`IsProbabilityMeasure`, `IsZeroOrProbabilityMeasure`), and atomless measures (`NoAtoms`). The typeclasses enable instance inference and proof automation through Lean's typeclass mechanism, allowing properties like "finite measures are σ-finite" to be inferred automatically and supporting powerful generic theorems that work across different measure classes.

## Key Files

| File | Purpose |
|------|---------|
| Finite.lean | Defines finite measure typeclasses: `IsFiniteMeasure` (μ univ < ∞), `IsLocallyFiniteMeasure` (finite in neighborhoods), `IsFiniteMeasureOnCompacts` (finite on compact sets); includes `FiniteSpanningSetsIn` structure for measures with countable finite spanning sets, finite-at-filter predicates, instances for measure operations (restriction, map, comap, sum, scalar multiplication), and extensionality theorems for finite measures on π-systems |
| NoAtoms.lean | Defines `NoAtoms` typeclass for atomless measures where all singletons have measure zero (μ {x} = 0); proves countable sets have measure zero, intervals with endpoints differing by singletons are almost-everywhere equal (Ioo a b =ᵐ Icc a b), and restriction to singleton complements equals the original measure |
| Probability.lean | Defines probability measure typeclasses: `IsProbabilityMeasure` (μ univ = 1) and `IsZeroOrProbabilityMeasure` (μ univ = 0 ∨ μ univ = 1); proves prob_compl_eq_one_sub (μ sᶜ = 1 - μ s for measurable s), ae_iff_prob_eq_one characterization (∀ᵐ a, p a ↔ μ {a | p a} = 1), instances for normalization (finite measure → probability via (μ univ)⁻¹ • μ), map/comap preservation, and convex combinations of probability measures |
| SFinite.lean | Defines s-finite and σ-finite measure typeclasses: `SFinite μ` (measure equals countable sum of finite measures), `SigmaFinite μ` (existence of countable finite measure spanning sets covering univ); constructs canonical spanning sets via `spanningSets μ` (monotone, measurable, with iUnion = univ), `spanningSetsIndex` for locating points, instances proving "finite measures are σ-finite" and "σ-finite measures are s-finite"; proves countability results (only countably many disjoint sets can have positive measure in s-finite spaces), measure approximation via supremum over restricted spanning sets, and existence of finite measures absolutely continuous with s-finite measures |

## Subdirectories

None.

## Search Tags

typeclass measure-theory finite-measure locally-finite-measure sigma-finite s-finite probability-measure no-atoms finite-spanning-sets spanning-sets measure-classification measure-properties isFiniteMeasure isLocallyFiniteMeasure isFiniteMeasureOnCompacts isProbabilityMeasure isZeroOrProbabilityMeasure noAtoms sFinite sigmaFinite measure-instances measure-extensionality countable-additivity
