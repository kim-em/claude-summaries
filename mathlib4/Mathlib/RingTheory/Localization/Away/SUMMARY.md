---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Localization/Away
generated: 2026-02-01T20:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 3
subdirs_count: 0
---

# Away

## Overview

This directory formalizes localization of a commutative ring R "away from" a single element x, meaning localization at the submonoid of powers of x. The central definition `IsLocalization.Away x S` is an abbreviation for `IsLocalization (Submonoid.powers x) S`. Key constructs include `invSelf` (the inverse of the localized element), `selfZPow` (integer powers in the localization), the universal property via `lift`, and operations for composing localizations away from products. The development also establishes the equivalence with adjoining a formal inverse via `AdjoinRoot`, proving finite presentation of localizations away from an element.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory: `IsLocalization.Away` abbreviation, `invSelf`, `sec` for reduced fractions, `lift` for the universal property, `map` between localizations, `awayToAwayLeft/Right` for product localizations, `mul`/`mul'` showing localization at y*x equals iterated localization, `selfZPow` for integer powers, `exists_reduced_fraction'` for UFD elements, product ring instances, sheaf condition `existsUnique_algebraMap_eq_of_span_eq_top` |
| AdjoinRoot.lean | Equivalence `awayEquivAdjoin` between `Away r` and `AdjoinRoot (C r * X - 1)`, proving localization away equals formally adjoining an inverse; `finitePresentation` instance for localizations away |
| Lemmas.lean | Additional lemmas: `mulNumerator` for combining numerators across a cover, `span_range_mulNumerator_eq_top` for ideal span preservation, `quotient_of_isIdempotentElem` showing quotient by idempotent is localization |

## Subdirectories

(none)

## Search Tags

localization away IsLocalization.Away Submonoid.powers invSelf selfZPow lift awayLift awayMap awayEquivAdjoin AdjoinRoot finitePresentation reduced-fraction algebraMap-isUnit mulNumerator idempotent quotient
