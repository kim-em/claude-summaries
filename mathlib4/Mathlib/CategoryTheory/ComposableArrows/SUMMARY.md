---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/ComposableArrows
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# ComposableArrows

## Overview

The `ComposableArrows/` directory defines the category of composable arrows in category theory, providing the type `ComposableArrows C n` which represents functors `Fin (n + 1) ⥤ C` - equivalently, chains of `n` composable morphisms in category `C`. This construction corresponds to `n`-simplices in the nerve of a category and provides infrastructure for working with sequences of composable arrows with well-behaved definitional properties. The API includes constructors for small cases (`mk₁`, `mk₂`, `mk₃`), functors to extract specific arrows from chains, and utilities for working with simplicial faces in categorical contexts.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `ComposableArrows C n` as functors from `Fin (n + 1)`, with `.left`, `.right`, `.hom` accessors and `precomp` operation for shifting arrows rightward, plus constructors `mk₀`, `mk₁`, `homMk`, `isoMk` |
| One.lean | Functors to `ComposableArrows C 1` including `functorArrows` which extracts the `i`-to-`j` arrow from an `n`-composable chain, and natural transformations between such functors |
| Two.lean | API for 2-simplices: given `f ≫ g = fg`, defines face maps `twoδ₂Toδ₁ : mk₁ f ⟶ mk₁ fg` and `twoδ₁Toδ₀ : mk₁ fg ⟶ mk₁ g` corresponding to simplicial degeneracy operations |

## Subdirectories

*(No subdirectories)*

## Search Tags

composable-arrows simplicial-nerve functors fin-categories arrow-chains simplicial-sets category-theory degeneracy-maps face-maps
