---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Order/Hom
generated: 2025-12-05T09:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Hom

## Overview

The `Hom/` directory provides constructions that upgrade algebraic group structures to (semi)normed groups using group (semi)norm homomorphisms with real codomains. It defines ways to construct `SeminormedGroup` and `NormedGroup` instances from `GroupSeminormClass` and `GroupNormClass` respectively, including both commutative and non-commutative variants. Additionally, it includes specialized support for nonarchimedean (ultrametric) normed groups, proving that groups constructed from nonarchimedean homs satisfy the ultrametric triangle inequality.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines abbreviations to construct `SeminormedGroup`, `SeminormedCommGroup`, `NormedGroup`, and `NormedCommGroup` instances from group (semi)norm classes with real codomain; includes additive variants for all constructions |
| Ultra.lean | Proves that seminormed groups constructed from nonarchimedean group seminorms satisfy the ultrametric distance property (`IsUltrametricDist`), enabling ultrametric space constructions from nonarchimedean homs |

## Subdirectories

None

## Search Tags

normed-groups seminormed-groups group-norms group-seminorms homomorphisms ultrametric nonarchimedean isultrametricdist additive-groups commutative-groups norm-constructions distance-structures
