---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Flat
generated: 2026-01-26T21:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 10
subdirs_count: 1
---

# Flat

## Overview

The `Flat/` directory contains the comprehensive formalization of flat modules and algebras over commutative (semi)rings, representing one of the fundamental homological properties in commutative algebra. The theory begins with the core definition of flatness (preservation of injective maps under tensor products) and develops multiple equivalent characterizations: the equational criterion (factoring relations through free modules), categorical exactness (preserving finite limits and short exact sequences), tensor characterizations via character modules (Baer criterion), and algebraic criteria involving torsion-freeness. The formalization establishes structural stability results (composition, base change, localization) and specialized theorems for integral domains, Dedekind domains, and Bézout domains. A major component is the theory of faithfully flat modules, which refines flatness by adding the faithfulness condition (IM ≠ M for maximal ideals I), enabling both preservation and reflection of exactness, zero detection, and descent properties for ring homomorphisms. The combination provides both the theoretical foundations for homological algebra and practical tools for checking flatness in concrete situations.

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

The subdirectory extends the theory to **faithfully flat modules**, which add the faithfulness condition (proper ideals remain proper) to flatness, enabling stronger results including exactness reflection, zero detection for modules and maps, descent of ring homomorphism properties, algebra-specific characterizations via prime spectrum surjectivity, and local ring criteria.

## Subdirectories

- [x] `FaithfullyFlat/` - Faithfully flat modules and algebras: theory of modules that are both flat and faithful (IM ≠ M for maximal ideals I), with characterizations via exact sequence reflection, zero detection, descent properties for ring homomorphisms, and algebra-specific results including prime spectrum surjectivity and local ring criteria

## Search Tags

flat-module faithful-flatness tensor-product injective-map exact-sequence equational-criterion character-module Baer-criterion torsion-free localization base-change stability domain Dedekind-domain valuation-ring Bezout-domain projective-module composition kernels equalizers finite-limits category-theory
