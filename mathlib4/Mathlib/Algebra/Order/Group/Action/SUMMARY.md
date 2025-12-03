---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Group/Action
generated: 2025-12-01T10:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Action

## Overview

The `Action/` directory provides theory for group actions that are compatible with order structures. It covers three main topics: (1) tautological actions by relation homomorphisms, embeddings, and isomorphisms on their domain types, (2) actions by order isomorphisms on flags (maximal chains in preorders), and (3) transfer of group action instances to order type synonyms like `αᵒᵈ` and `Lex α`. These actions preserve the underlying ordered structure and establish that order automorphisms form natural symmetry groups for ordered types.

## Key Files

| File | Purpose |
|------|---------|
| End.lean | Tautological `MulAction` instances for relation homomorphisms (`r →r r`), embeddings (`r ↪r r`), and isomorphisms (`r ≃r r`) acting on their domain type `α` via application, with faithful action proofs |
| Flag.lean | `MulAction` instance for order isomorphisms `α ≃o α` acting on flags (maximal chains) via the `map` operation, using `SetLike.coe_injective` to establish the action |
| Synonym.lean | Transfer of `MulAction`, `SMulCommClass`, and `IsScalarTower` instances from type `α` to order synonyms `αᵒᵈ` (order dual) and `Lex α` (lexicographic order), enabling actions on reordered versions of types |

## Subdirectories

None

## Search Tags

group-action ordered-action order-isomorphism relation-isomorphism faithful-action flags maximal-chains order-dual lexicographic-order type-synonyms scalar-tower smul-comm-class tautological-action
