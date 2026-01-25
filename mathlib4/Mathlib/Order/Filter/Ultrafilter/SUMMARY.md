---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Filter/Ultrafilter
generated: 2026-01-26T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Ultrafilter

## Overview

The `Ultrafilter/` subdirectory contains the theory of ultrafilters, which are minimal (maximal in the set order) proper filters. Ultrafilters are a fundamental tool in topology, logic, and analysis, characterized by the property that for any set S, either S or its complement belongs to the ultrafilter. The directory defines the Ultrafilter structure, proves it forms a monad, establishes the ultrafilter lemma (every proper filter extends to an ultrafilter), and provides extensive theory on operations (map, comap, bind), principal ultrafilters (pure), and special ultrafilters like the hyperfilter (extending the cofinite filter on infinite types).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core ultrafilter definitions and basic properties: Ultrafilter structure (minimal proper filter), proof that Filter α is atomic (every filter extends to an ultrafilter), ultrafilter operations (map, comap, bind, pure), monad structure and lawfulness, complement characterization (sᶜ ∉ f ↔ s ∈ f), union membership (s ∪ t ∈ f ↔ s ∈ f ∨ t ∈ f), ultrafilter lemma (exists_le, of), characterization of filters via ultrafilters (mem_iff_ultrafilter) |
| Basic.lean | Extended ultrafilter theory: finite union/intersection characterizations (finite_sUnion_mem_iff, finite_biUnion_mem_iff), eventually_exists lemmas for finite index sets, characterization of ultrafilters on finite types (eq_pure_of_finite), dichotomy theorem (le_cofinite_or_eq_pure), ultrafilter existence from finite intersection property, hyperfilter definition (ultrafilter extending cofinite on infinite types), hyperfilter properties (finite sets not in hyperfilter, cofinite sets in hyperfilter), tendsto_iff_ultrafilter characterization |

## Subdirectories

(none)

## Search Tags

ultrafilter maximal-filter minimal-filter pure principal-ultrafilter map comap bind monad ultrafilter-lemma complement-characterization union-membership finite-union finite-intersection hyperfilter cofinite tendsto filter-convergence atomic-filter Zorn-lemma axiom-of-choice
