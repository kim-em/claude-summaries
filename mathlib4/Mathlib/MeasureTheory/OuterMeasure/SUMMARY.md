---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/OuterMeasure
generated: 2026-01-25T22:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# OuterMeasure

## Overview

The `OuterMeasure/` directory provides a complete formalization of outer measures in mathlib4. An outer measure is a countably subadditive monotone function from sets to extended non-negative reals that sends the empty set to zero. This directory contains the core definition, basic properties, algebraic operations (addition, scalar multiplication, suprema), the Carathéodory construction that produces σ-algebras from outer measures, methods for constructing outer measures from arbitrary functions or additive contents on semirings, the "almost everywhere" filter for outer measures, and the Borel-Cantelli lemma. Outer measures do not require the underlying space to have a measurable structure, making them fundamental building blocks for measure theory.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of outer measures as countably subadditive monotone functions sending ∅ to 0, defines the OuterMeasure structure and OuterMeasureClass typeclass for unified API with measures |
| Basic.lean | Basic properties of outer measures: monotonicity lemmas, countable union bounds, measure_union_le, null set characterizations (measure_iUnion_null_iff), locally null implies globally null in second-countable spaces, and general iUnion convergence theorems for sequences approximating a set |
| Operations.lean | Algebraic structure on outer measures: zero/addition/scalar multiplication, complete lattice structure (suprema/infima), pushforward (map) and pullback (comap) along functions, restriction to subsets, dirac and sum constructions, proves OuterMeasure α forms AddCommMonoid and Module over ℝ≥0∞ |
| AE.lean | The "almost everywhere" (ae) filter for outer measures: defines ae μ as the filter of co-null sets (s ∈ ae μ ↔ μ sᶜ = 0), notation ∀ᵐ/∃ᵐ/=ᵐ[μ]/≤ᵐ[μ], proves measure_mono_ae and measure_congr showing the filter respects measure inequalities and equalities |
| Caratheodory.lean | Carathéodory measurability criterion: a set s is Carathéodory-measurable for outer measure m if ∀t, m t = m(t∩s) + m(t∖s), proves Carathéodory-measurable sets form a σ-algebra (m.caratheodory), proves m(⋃ᵢ sᵢ) = ∑ᵢ m(sᵢ) for disjoint measurable sets, establishes caratheodory σ-algebra for specific outer measures (zero, top, dirac, sums) |
| OfFunction.lean | Construct outer measures from arbitrary functions: ofFunction m takes any m : Set α → ℝ≥0∞ with m ∅ = 0 and produces the unique maximal outer measure ≤ m everywhere (defined as infimum over countable covers), boundedBy relaxes the m ∅ = 0 requirement, characterization of infima of outer measure families via sInfGen, proves commutativity with map/comap/restrict operations |
| Induced.lean | Induced outer measures via extend and inducedOuterMeasure: given m defined on subset P ⊆ Set α, construct outer measure via covers by P-sets, proves induced measure equals m on P-sets under monotonicity/subadditivity assumptions, trim operation (forget non-measurable values then take induced measure), proves trim is idempotent and respects algebraic operations, characterizes Carathéodory-measurable sets for induced measures |
| OfAddContent.lean | Carathéodory extension theorem: construct measures from sigma-subadditive additive contents on set semirings, proves all semiring sets and all sets in the generated σ-algebra are Carathéodory-measurable, defines AddContent.measure and AddContent.measureCaratheodory which extend additive content to full measures, proves the constructed measure agrees with the original content on the semiring |
| BorelCantelli.lean | Borel-Cantelli lemma (first part): if sᵢ is a countable family with ∑ᵢ μ(sᵢ) < ∞, then μ(limsup sᵢ) = 0, equivalently a.e. all points belong to finitely many sets, proved for limsup along cofinite and atTop filters, includes variants measure_limsup_eq_zero and ae_eventually_notMem |

## Subdirectories

*No subdirectories*

## Search Tags

outer-measure caratheodory-measurable almost-everywhere borel-cantelli measure-theory countably-subadditive induced-outer-measure trim extend bounded-by of-function additive-content set-semiring dynkin-system ae-filter map-comap-restrict dirac-measure sum-outer-measure
