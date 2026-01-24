---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/GroupAction/DomAct
generated: 2026-01-24T23:20:15Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# DomAct

## Overview

The `DomAct/` directory defines "domain actions" - a specialized construction where a group acting on a domain `α` induces a right action on functions and homomorphisms from `α`. The key insight is that if `M` acts on `α` on the left, then `DomMulAct M` (notation `Mᵈᵐᵃ`) acts on `α → β` on the right by `(c • f) a = f (c • a)`. This is implemented as a type synonym for `MulOpposite M` to avoid instance conflicts. The directory provides instances for actions on plain functions, monoid homomorphisms `A →* B`, additive homomorphisms `A →+ B`, and equivariant maps `α →[N] β`, enabling domain-shift transformations in functional analysis and ergodic theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `DomMulAct M` type synonym and instances for actions on `α → β`, `A →* B`, `A →+ B` |
| ActionHom.lean | Actions of `Mᵈᵐᵃ` on equivariant homomorphisms `α →[N] β` and `A →+[N] B` |

## Subdirectories

(none)

## Search Tags

domain-action right-action function-action equivariant-homomorphism type-synonym opposite ergodic-theory operator-theory DomMulAct
