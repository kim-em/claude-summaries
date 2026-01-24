---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Constructions/Polish
generated: 2026-01-25T22:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Polish

## Overview

The `Polish/` directory develops the measure-theoretic foundations for Polish spaces (separable, completely metrizable topological spaces) and standard Borel spaces (measurable spaces arising from Polish topologies). It establishes the deep connections between topology and measurability in these spaces, including analytic set theory, Lusin's separation theorem, the Lusin-Souslin theorem on continuous injective images, and culminates in the Borel Isomorphism Theorem. The directory also provides tools for embedding standard Borel spaces into the reals and extends measurability results to strongly measurable functions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory of standard Borel spaces and Polish space measure theory: defines `StandardBorelSpace` typeclass for measurable spaces arising from Polish topologies, develops analytic set theory (`AnalyticSet` as continuous images of Polish spaces), proves Lusin's separation theorem (`AnalyticSet.measurablySeparable` for disjoint analytic sets), establishes Lusin-Souslin theorem (`MeasurableSet.image_of_continuousOn_injOn` showing continuous injective images preserve Borel measurability), proves `isClopenable_iff_measurableSet` characterization, and culminates in Borel Isomorphism Theorem (`PolishSpace.measurableEquivOfNotCountable` proving any two uncountable standard Borel spaces are measurably equivalent, and `PolishSpace.Equiv.measurableEquiv` for spaces of equal cardinality) |
| EmbeddingReal.lean | Embedding standard Borel spaces into reals: proves every standard Borel space is measurably equivalent to a Borel subset of ℝ (`exists_subset_real_measurableEquiv`), constructs measurable embeddings into reals (`exists_measurableEmbedding_real`), defines canonical `embeddingReal` function with proven measurability, handles countable and uncountable cases separately using Cantor-Bendixson theory |
| StronglyMeasurable.lean | Strongly measurable functions on Polish spaces: proves `measurableSet_exists_tendsto` showing convergence sets for strongly measurable function sequences are measurable, establishes `limUnder` preserves strong measurability for completely metrizable codomains, exploits separability of ranges and closure properties to extend measurability results from Polish spaces to strongly measurable functions with complete metric codomains |

## Subdirectories

*(No subdirectories)*

## Search Tags

polish-space standard-borel-space analytic-set lusin-theorem lusin-souslin measurable-separation borel-isomorphism-theorem schroeder-bernstein measurable-embedding embedding-real strongly-measurable clopenable cantor-space projective-hierarchy descriptive-set-theory measurable-equivalence countably-separated
