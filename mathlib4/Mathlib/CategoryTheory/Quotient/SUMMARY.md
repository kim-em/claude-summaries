---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Quotient
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Quotient

## Overview

The `Quotient/` subdirectory contains extensions to the base quotient category construction (defined in `CategoryTheory/Quotient.lean`) for categories with additional algebraic structure. It provides compatibility results showing that when a congruence relation on morphisms is compatible with addition or scalar multiplication, the resulting quotient category inherits preadditive or linear structure respectively. These modules enable quotient constructions to preserve the rich algebraic properties of preadditive and linear categories.

## Key Files

| File | Purpose |
|------|---------|
| Preadditive.lean | Quotient category inherits preadditive structure when congruence respects addition; defines additive group structure on hom-sets and proves quotient functor is additive |
| Linear.lean | Quotient category inherits R-linear structure when congruence respects scalar multiplication; builds on preadditive quotient to add module structure and linear functor compatibility |

## Subdirectories

*(None)*

## Search Tags

quotient-categories preadditive-categories linear-categories congruence-relations homological-algebra category-quotients additive-functors linear-functors module-categories
