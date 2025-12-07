---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/Limits
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Limits

## Overview

The `Limits/` directory establishes the interaction between limits/colimits and monoidal structure in monoidal categories. It proves that the limit functor `lim : (J ⥤ C) ⥤ C` has a canonical lax monoidal structure, constructs morphisms from tensor products of limits to limits of tensor products, and provides preservation results showing how tensor functors interact with limits in braided categories. This machinery is essential for understanding how categorical constructions commute with monoidal operations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Lax monoidal structure on limit functor with unit and tensor morphisms satisfying coherence |
| Preserves.lean | Preservation instances for limits/colimits under tensor products in braided monoidal categories |

## Subdirectories

*(No subdirectories)*

## Search Tags

limits colimits monoidal-categories lax-monoidal-functor limit-functor tensor-products preserves-limits preserves-colimits braided-categories tensorLeft tensorRight curriedTensor
