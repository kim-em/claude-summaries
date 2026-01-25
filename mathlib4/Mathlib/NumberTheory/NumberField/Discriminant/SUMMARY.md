---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/NumberField/Discriminant
generated: 2026-01-25T20:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Discriminant

## Overview

The `Discriminant/` directory contains the formalization of the absolute discriminant of number fields and related invariants. The discriminant is a fundamental arithmetic invariant defined as `Algebra.discr ℤ (RingOfIntegers.basis K)`, which measures the "size" of the number field. The directory includes basic definitions and properties, major theorems like Hermite-Minkowski (discriminant > 2 for nontrivial fields) and Hermite's Theorem (finiteness of number fields with bounded discriminant), as well as the relationship between discriminants and different ideals in field extensions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of absolute discriminant `NumberField.discr`, basic properties (non-zero, independence of basis choice, invariance under field isomorphism), rational field discriminant = 1, and equivalence theorem for discriminants of integral bases |
| Basic.lean | Major discriminant theorems: Hermite-Minkowski Theorem (`abs_discr_gt_two`: nontrivial number field has |discr| > 2), Hermite Theorem (`finite_of_discr_bdd`: finiteness of number fields with bounded discriminant), volume/covolume formulas for mixed embeddings, Minkowski bounds, and relationship to canonical embeddings |
| Different.lean | Relationship between discriminant and different ideal: `absNorm_differentIdeal` (norm of different ideal equals absolute discriminant), discriminant formulas for field extensions, linear disjointness from coprime discriminants, and compositum discriminant formula for linearly disjoint fields |

## Subdirectories

*(none)*

## Search Tags

discriminant absolute-discriminant different-ideal hermite-minkowski hermite-theorem minkowski-bound volume covolume field-extension linear-disjoint compositum ring-of-integers number-field-invariants algebraic-number-theory fundamental-domain lattice-basis
