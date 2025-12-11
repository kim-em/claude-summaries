---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/W
generated: 2025-12-11T09:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 0
---

# W

## Overview

W-types (well-founded trees) are inductively defined types parameterized by a type `α` of node labels and a family `β : α → Type*` of arities. A `WType β` represents finitely branching trees where nodes labeled by `a : α` have children indexed by `β a`. This folder provides the core definition, proves encodability and cardinality results, and demonstrates that common inductive types like `Nat` and `List` can be represented as W-types.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `WType` inductive definition with bijection to sigma type (`equivSigma`), eliminator (`elim`), depth function, and encodability instance for encodable fintypes |
| Cardinal.lean | Cardinality bounds for W-types; main result `cardinalMk_le_max_aleph0_of_finite` shows W-types over finite arities have cardinality at most `max #α ℵ₀` |
| Constructions.lean | Concrete examples: natural numbers as W-type (`equivNat` via `Natα`/`Natβ`) and lists as W-type (`equivList` via `Listα`/`Listβ`) |

## Subdirectories

(none)

## Search Tags

W-type well-founded trees inductive types polynomial functor WType encodable cardinal finitely-branching Nat List construction fixed-point
