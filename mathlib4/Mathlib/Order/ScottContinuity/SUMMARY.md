---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/ScottContinuity
generated: 2026-01-26T12:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# ScottContinuity

## Overview

The `ScottContinuity/` directory contains theory for Scott continuity, a topological notion from domain theory where a function is continuous if it preserves suprema of directed sets. This directory provides characterizations of Scott continuous functions on complete lattices and product spaces. The key result establishes that a function is Scott continuous if and only if it commutes with supremum operations on directed sets. For complete linear orders, it also proves that meet (infimum) operations are Scott continuous.

## Key Files

| File | Purpose |
|------|---------|
| Complete.lean | Scott continuity on complete lattices: `scottContinuous_iff_map_sSup` (Scott continuous ↔ commutes with `sSup` on directed sets), Scott continuity of meet operations on complete linear orders |
| Prod.lean | Scott continuity on product spaces: `ScottContinuous.fromProd` (function is Scott continuous on product if Scott continuous in each variable), `ScottContinuous.prod` (product map of Scott continuous functions is Scott continuous) |

## Subdirectories

(none)

## Search Tags

Scott-continuity domain-theory directed-sets supremum complete-lattice product-spaces topology upper-topology meet-operation monotone-functions
