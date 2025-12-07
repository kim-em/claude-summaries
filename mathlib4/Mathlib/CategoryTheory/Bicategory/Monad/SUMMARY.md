---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory/Monad
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# Monad

## Overview

The `Monad/` directory contains the formalization of comonads in bicategories. Comonads are defined as comonoid objects in the endomorphism monoidal category of an object. The directory establishes the equivalence between comonads in a bicategory `B` and oplax functors from the trivial bicategory to `B`, and shows that comonads form a bicategory structure. Note that monads (the dual concept) are not yet implemented due to missing infrastructure for lax functors.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines comonads in bicategories as comonoid objects with comultiplication and counit morphisms satisfying comonad laws; establishes bijection with oplax functors from trivial bicategory; defines ComonadBicat bicategory structure using oplax natural transformations |

## Subdirectories

None

## Search Tags

comonad bicategory comonoid endomorphism-category comultiplication counit comonad-laws oplax-functor trivial-bicategory locally-discrete comonad-bicategory oplax-transformation monoidal-category
