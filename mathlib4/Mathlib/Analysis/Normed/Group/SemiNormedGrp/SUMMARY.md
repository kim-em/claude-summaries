---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Group/SemiNormedGrp
generated: 2025-12-05T08:17:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# SemiNormedGrp

## Overview

The `SemiNormedGrp/` directory provides the categorical infrastructure for seminormed abelian groups. It implements the category `SemiNormedGrp` (and its norm-nonincreasing variant `SemiNormedGrp₁`) as concrete categories, establishes that these categories have kernels and cokernels with appropriate norm properties, and provides a completion functor with its universal property.

## Key Files

| File | Purpose |
|------|---------|
| Kernels.lean | Kernels and cokernels in both `SemiNormedGrp₁` and `SemiNormedGrp`; proves `SemiNormedGrp₁` has cokernels with norm-nonincreasing cokernel maps, and `SemiNormedGrp` has both kernels (as equalizers) and cokernels; provides explicit cokernel constructions with good norm properties using quotient by range |
| Completion.lean | Completion as endofunctor `SemiNormedGrp ⥤ SemiNormedGrp`; includes canonical inclusion morphism, functoriality (map preserves composition), additive structure (proves `Preadditive SemiNormedGrp` and `Functor.Additive completion`), and universal property via `completion.lift` for extending morphisms to complete spaces |

## Subdirectories

(none)

## Search Tags

category-theory seminormedgrp concrete-category kernels cokernels equalizers quotient-norm completion-functor bounded-homomorphisms norm-nonincreasing preadditive-category additive-functor universal-property limits colimits
