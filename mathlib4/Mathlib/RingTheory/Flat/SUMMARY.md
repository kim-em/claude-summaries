---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Flat
generated: 2026-01-26T21:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 10
subdirs_count: 1
---

# Flat

## Overview

The `Flat/` directory contains the comprehensive formalization of flat modules and algebras over commutative (semi)rings. This includes the core definition of flatness (preservation of injective maps under tensor products), characterizations via various criteria (equational criterion, character modules, tensor exactness), structural properties (stability under composition, base change, and localization), specialized results for domains and Dedekind domains, and the theory of faithfully flat modules. The formalization covers both theoretical foundations and practical characterizations, including connections to torsion-freeness, projective modules, and exact functors.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of flat modules (`Module.Flat`) as mono-flat (preserving injectivity under tensoring); proves free and projective modules are flat, direct sums preserve flatness, and establishes the fundamental preservation properties for tensor products |
| CategoryTheory.lean | Categorical characterization of flatness: proves tensoring with flat modules is exact (preserves short exact sequences) and establishes equivalence with preserving finite limits |
| Domain.lean | Flatness results specific to integral domains: tensor products of injective maps remain injective under flatness assumptions, and tensor products of linearly independent families remain linearly independent |
| Equalizer.lean | Base change along flat modules preserves kernels and equalizers; constructs canonical maps from `M ⊗ ker(f)` to `ker(M ⊗ f)` and proves they are isomorphisms when M is flat |
| EquationalCriterion.lean | Equational criterion for flatness: module M is flat iff every relation in M is trivial (can be factored through intermediate free modules); proves finitely presented flat modules are projective |
| Localization.lean | Flatness and localization: proves localizations are flat, flatness is preserved and reflected by localization, and flatness can be checked locally at maximal ideals or spanning sets |
| Stability.lean | Stability of flatness under algebraic operations: composition (if S is R-flat and M is S-flat then M is R-flat), base change (S ⊗ M is S-flat when M is R-flat), and localization |
| Tensor.lean | Characterizations of flatness over rings via tensor products with ideals; proves M is flat iff character module is injective (Baer criterion), and establishes equivalence with tensor injectivity for (finitely generated) ideals |
| TorsionFree.lean | Relationship between flatness and torsion-freeness: flat modules are torsion-free; over Dedekind domains, Bézout domains, and rings whose localizations are valuation rings, flatness is equivalent to torsion-freeness |

## Subdirectories

- [ ] `FaithfullyFlat/` - Faithfully flat modules (flat modules M where IM ≠ M for all maximal ideals I)

## Search Tags

flat-module faithful-flatness tensor-product injective-map exact-sequence equational-criterion character-module Baer-criterion torsion-free localization base-change stability domain Dedekind-domain valuation-ring Bezout-domain projective-module composition kernels equalizers finite-limits category-theory
