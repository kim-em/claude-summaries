---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics/Circle/RotationNumber
generated: 2026-01-24T00:00:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# RotationNumber

## Overview

This folder contains the formalization of translation numbers (rotation numbers) for monotone maps of the real line that commute with integer translation. The central type `CircleDeg1Lift` represents lifts of degree-one circle maps: monotone functions `f : ℝ → ℝ` satisfying `f(x + 1) = f(x) + 1`. The translation number `τ(f) = lim_{n→∞} (f^n(x) - x)/n` is proven to exist and be independent of the starting point `x`.

## Key Files

| File | Purpose |
|------|---------|
| `TranslationNumber.lean` | Defines `CircleDeg1Lift` structure with monoid/lattice instances; defines translation number via auxiliary sequence `f^{2^n}(0)/2^n`; proves key properties including: conjugacy invariance, additivity under composition of commuting maps, rational values characterize periodic orbits, and semiconjugacy theorem for maps with equal translation numbers (Ghys's Proposition 5.4) |

## Subdirectories

*(none)*

## Search Tags

translation-number rotation-number circle-homeomorphism degree-one-lift CircleDeg1Lift monotone-map periodic-orbit rational-rotation semiconjugacy Ghys Poincare circle-dynamics orientation-preserving
