---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/OreLocalization
generated: 2026-01-24T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# OreLocalization

## Overview

The `OreLocalization/` directory implements Ore localization for non-commutative monoids, providing a construction analogous to fraction fields but applicable in non-commutative settings. The core content includes the definition of Ore sets (submonoids satisfying the Ore condition that allows common factors/summands to be rearranged), the construction of localized monoids `R[S⁻¹]` as quotients with division notation `r /ₒ s`, the monoid/module structure on localizations with universal mapping properties, and cardinality bounds for localized structures. This machinery extends classical commutative localization to settings where multiplication doesn't commute, essential for non-commutative ring theory and algebraic geometry.

## Key Files

| File | Purpose |
|------|---------|
| OreSet.lean | Ore set definition: typeclass for submonoids satisfying the Ore condition (common factors/summands can be rearranged), oreNum/oreDenom functions, instances for trivial submonoids and commutative monoids |
| Basic.lean | Core Ore localization construction: quotient type `R[S⁻¹]` with division notation `/ₒ`, monoid/module structure, scalar multiplication, universal mapping property, lift functions for defining maps from localizations |
| Cardinality.lean | Cardinality bounds: surjectivity of `x /ₒ 1` maps under finiteness assumptions, cardinality inequality `#(R[S⁻¹]) ≤ #R`, bounds in terms of max of `#S` and `#X` |

## Subdirectories

*(none)*

## Search Tags

ore-localization ore-set non-commutative localization fraction monoid-localization universal-property numerator denominator ore-condition cardinality
