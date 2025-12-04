---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/NonAssoc/PreLie
generated: 2025-12-04T09:15:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# PreLie

## Overview

The `PreLie/` directory contains the foundational theory of pre-Lie rings and algebras. Pre-Lie structures are non-associative rings where the associator `(x * y) * z - x * (y * z)` satisfies a symmetry condition: left pre-Lie rings have associators symmetric in the first two variables, while right pre-Lie rings have associators symmetric in the last two variables. The directory establishes the equivalence between left and right versions via opposite multiplication, and extends these definitions to algebras over commutative rings with compatible scalar actions.

## Key Files

| File | Purpose |
|------|---------|
| `Basic.lean` | Defines left and right pre-Lie rings and algebras, proves equivalence between left and right versions via opposite multiplication (`op : L ≃* Lᵐᵒᵖ`), includes both ring and algebra (module) versions |

## Subdirectories

*(No subdirectories)*

## Search Tags

pre-lie-ring pre-lie-algebra associator left-symmetric right-symmetric opposite-multiplication nonunital-nonassoc-ring module scalar-tower smul-comm-class
