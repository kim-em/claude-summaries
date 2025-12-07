---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Equivalence
generated: 2025-12-07T10:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# Equivalence

## Overview

The `Equivalence/` subdirectory contains specialized constructions and properties for category equivalences beyond the basic equivalence definition in the parent directory. Currently, it focuses on functoriality of equivalence operations, proving that symmetry and inverse operations themselves form functors and equivalences. This provides higher-order categorical structure on the space of equivalences between categories, using the calculus of mates from adjunction theory.

## Key Files

| File | Purpose |
|------|---------|
| Symmetry.lean | Functoriality of equivalence symmetry: `symmEquiv` showing `(C ≌ D) ≌ (D ≌ C)ᵒᵖ`, `inverseFunctor` sending equivalence to its inverse functor, and `congrLeftFunctor` for whiskering equivalences |

## Subdirectories

(none)

## Search Tags

category-theory equivalence symmetry functor-category inverse-functor conjugation mates adjunction whiskering congruence higher-category
