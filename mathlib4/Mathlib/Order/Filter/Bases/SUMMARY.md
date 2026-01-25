---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Filter/Bases
generated: 2026-01-26T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Bases

## Overview

The `Bases/` subdirectory provides the core theory of filter bases in Lean. A filter basis is a nonempty collection of sets such that the intersection of any two sets in the collection contains some set in the collection. Filter bases provide a convenient way to define filters: any filter basis generates a unique filter where a set belongs to the filter if and only if it contains a basis element. The directory includes basic definitions and constructions (`FilterBasis`, `IsBasis`, `HasBasis`), basis combinators for filter operations (inf, sup, map, comap, product), and finiteness results for bases involving finite intersections.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core filter basis theory: `FilterBasis` structure (nonempty downward-directed set collection), `IsBasis` (indexed basis with predicate), `HasBasis` (characterization of existing filter via basis); conversions between filters and bases; basis combinators for inf, sup, map, comap, product, tendsto; antitone bases (`IsAntitoneBasis`, `HasAntitoneBasis`) |
| Finite.lean | Finiteness results for filter bases: `hasBasis_generate` (generated filters have basis of finite intersections), `FilterBasis.ofSets` (smallest basis containing a collection), finite intersection bases for infima (`HasBasis.iInf'`, `hasBasis_iInf_principal_finite`), pairwise disjoint basis element existence for disjoint filters |

## Subdirectories

(None)

## Search Tags

filter-basis FilterBasis IsBasis HasBasis downward-directed generate principal nonempty intersection inf sup map comap product tendsto antitone finite-intersections pairwise-disjoint
