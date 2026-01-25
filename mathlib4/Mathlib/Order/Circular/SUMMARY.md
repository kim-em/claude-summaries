---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Circular
generated: 2026-01-25T21:26:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 1
subdirs_count: 0
---

# Circular

## Overview

The `Circular/` subdirectory provides a concrete instance of circular order on `ZMod n` types, demonstrating how the abstract circular order framework from the parent module applies to modular arithmetic. The directory shows how circular orders on `ℤ`, `Fin n`, and `ZMod n` are all derived from their underlying linear orders using the "loop around" construction.

## Key Files

| File | Purpose |
|------|---------|
| ZMod.lean | Circular order instance for `ZMod n`: provides `CircularOrder` instances for integers, finite types, and modular integers by converting their linear orders using `LinearOrder.toCircularOrder`; includes explicit characterizations of `btw` and `sbtw` relations |

## Subdirectories

*(none)*

## Search Tags

circular-order ZMod modular-arithmetic betweenness cyclic-order finite-types Fin
