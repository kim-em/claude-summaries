---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function/AEEqFun
generated: 2026-01-25T23:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# AEEqFun

## Overview

The `AEEqFun/` subdirectory extends the theory of almost everywhere equal functions (L⁰ space) with group actions. Specifically, it defines how `DomMulAct` and `DomAddAct` act on the space `α →ₘ[μ] β` of almost everywhere equal functions when a group `M` acts on the domain `α` by measure-preserving transformations. The action sends each function `f` to its composition with the group action on the domain.

## Key Files

| File | Purpose |
|------|---------|
| DomAct.lean | Defines scalar multiplication and group actions of `DomMulAct` and `DomAddAct` on AE equivalence classes of functions, with instances for `SMul`, `MulAction`, `DistribMulAction`, and `MulDistribMulAction` when the domain action preserves the measure |

## Subdirectories

(None)

## Search Tags

ae-equal-functions group-action domain-action measure-preserving dommulact domaddact scalar-multiplication mulaction ae-equivalence-class
