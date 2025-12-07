---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian/Projective
generated: 2025-12-07T08:50:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Projective

## Overview

The `Projective/` directory provides the theory of projective objects in abelian categories, including characterizations via the preadditive co-Yoneda functor, projective dimension as a homological invariant, and the construction of projective resolutions. Projective objects are dual to injective objects and play a central role in computing left derived functors and Ext groups.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Characterizes projective objects in abelian categories: P is projective iff preadditiveCoyonedaObj P preserves finite colimits (equivalently, preserves homology or epimorphisms) |
| Dimension.lean | Defines projective dimension via Ext vanishing: HasProjectiveDimensionLT X n when Ext X Y i = 0 for all i ≥ n; proves projective objects have dimension ≤ 1, dimension transfers across exact sequences, and dimension computes as infimum in WithBot ℕ∞ |
| Resolution.lean | Constructs projective resolutions in abelian categories with enough projectives; proves any morphism lifts to chain maps between resolutions (unique up to homotopy), resolutions are homotopy equivalent, and provides functorial projectiveResolutions to the homotopy category |

## Subdirectories

(none)

## Search Tags

projective-objects abelian-categories preadditive-coyoneda preserves-colimits projective-dimension ext-groups vanishing-ext projective-resolutions homotopy-equivalence chain-complexes derived-functors enough-projectives homological-algebra
