---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Field
generated: 2025-12-05T08:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 7
subdirs_count: 0
---

# Field

## Overview

The `Field/` directory establishes the theory of normed division rings and normed fields—algebraic structures where the norm is strictly multiplicative (‖x * y‖ = ‖x‖ * ‖y‖). It provides the foundational definitions (`NormedDivisionRing`, `NormedField`, `NontriviallyNormedField`, `DenselyNormedField`) and proves key topological and algebraic properties including continuity of inversion, completeness criteria, and the discrete-vs-nontrivial dichotomy. The directory also covers specialized topics like ultrametric norms (nonarchimedean fields), algebraic structures on unit balls and spheres (as subsemigroups, submonoids, and groups), proper space properties, field completion via absolute values, and concrete instances for ℝ and ℚ.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `NormedDivisionRing`, `NormedField`, `NontriviallyNormedField`, and `DenselyNormedField`; proves basic properties (norm of inverse/division/powers, norm_mul equality); shows real and rational number instances; provides induced normed field structures from embeddings; defines absolute value to normed field construction |
| Lemmas.lean | Extended theory for normed division rings and fields; proves continuous inversion (`ContinuousInv₀`, `IsTopologicalDivisionRing`); establishes filter equivalences (`inv_cobounded₀`, `inv_nhdsNE_zero`); proves `discreteTopology_or_nontriviallyNormedField` dichotomy and `discreteTopology_of_bddAbove_range_norm`; shows `completeSpace_iff_isComplete_closedBall` for normed fields; provides `DilationEquiv` instances for multiplication |
| Ultra.lean | Characterizes ultrametric (nonarchimedean) norms on division rings; proves `isUltrametricDist_iff_forall_norm_natCast_le_one` (ultrametricity equivalent to ‖n‖ ≤ 1 for all naturals); provides sufficient conditions via binomial expansion bounds and technical lemmas for establishing ultrametric property from norm constraints |
| UnitBall.lean | Defines algebraic structures on metric unit balls and spheres in normed rings/fields; provides `Subsemigroup.unitBall`, `Submonoid.unitClosedBall`, and `Submonoid.unitSphere` with instances for `Semigroup`, `Monoid`, `Group`, `CommGroup`; proves continuous multiplication; shows unit sphere forms a group in normed division rings via `unitSphereToUnits` homomorphism |
| Instances.lean | Proves that normed fields are completable topological fields (`CompletableTopField` instance); establishes cauchy sequences of inverses are cauchy when bounded away from zero; provides the key infrastructure for field completion via uniform completion |
| ProperSpace.lean | Proves nontrivially normed fields are proper spaces when weakly locally compact; shows `ProperSpace.of_nontriviallyNormedField_of_weaklyLocallyCompactSpace` using scaling of compact closed balls by powers of elements with norm > 1; specialized alternative to general finite-dimensional result requiring fewer imports |
| WithAbs.lean | Provides `WithAbs` type synonym for fields equipped with absolute values; defines normed field structure from absolute values; constructs field completions via `AbsoluteValue.Completion` using uniform space completion; proves isometry properties for embeddings that factor absolute values; shows completion inherits local compactness when target is locally compact |

## Subdirectories

*(No subdirectories)*

## Search Tags

normed-fields normed-division-rings multiplicative-norm strictly-multiplicative nontrivially-normed densely-normed ultrametric nonarchimedean unit-ball unit-sphere continuous-inversion topological-division-ring proper-space discrete-topology absolute-value field-completion completable-field cauchy-sequences isometry uniform-completion real-field rational-field norm-one bounded-operators dilation-equiv cobounded-filter separable-algebra WithAbs
