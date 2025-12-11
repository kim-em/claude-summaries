---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/SetLike
generated: 2025-12-11T10:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 0
---

# SetLike

## Overview

The `SetLike/` directory provides the `SetLike` typeclass, a unified interface for types that have set-like extensionality properties. The main use case is algebraic subobjects (such as `Submonoid`, `Submodule`, `Subgroup`) whose non-proof data consists only of a carrier set. When a type `A` is `SetLike` with elements of type `B`, it has an injective map to `Set B`, automatically gaining membership, coercion to sort (as subtype), partial ordering (by inclusion), and extensionality lemmas.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `SetLike` typeclass definition and standard infrastructure: `Membership` instance, `CoeSort` to subtype, `PartialOrder` by inclusion, extensionality lemmas (`ext`, `ext'`), monotonicity lemmas, and helper instances for subtypes of SetLike types |
| Fintype.lean | `Fintype` and `Finite` instances for SetLike types: if `SetLike A B` and `Fintype B` (or `Finite B`), then `A` is also `Fintype` (or `Finite`) via the injective coercion |

## Subdirectories

*(none)*

## Search Tags

setlike subobject carrier membership extensionality submonoid submodule subgroup algebraic-substructure coercion partial-order fintype
