---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Adjunction/Lifting
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Lifting

## Overview

The `Lifting/` directory formalizes two fundamental constructions for lifting adjoints through commutative squares of functors: the adjoint triangle theorem and the adjoint lifting theorem. These theorems provide conditions under which an adjoint can be "lifted" from a composite functor to one of its components. The directory contains dual versions for lifting left adjoints (through monadic functors) and right adjoints (through comonadic functors).

## Key Files

| File | Purpose |
|------|---------|
| Left.lean | Adjoint triangle theorem and adjoint lifting theorem for left adjoints: given `F ⊣ U` with regular epi counit and reflexive coequalizers in `A`, if `R ⋙ U` has a left adjoint then `R` has a left adjoint; special case for monadic `U`; square lifting theorem for commutative squares where `V` is monadic |
| Right.lean | Dual theorems for right adjoints: given `F ⊣ U` with regular mono unit and coreflexive equalizers in `C`, if `L ⋙ F` has a right adjoint then `L` has a right adjoint; special case for comonadic `F`; square lifting theorem for commutative squares where `V` is comonadic (adapted from Left.lean, kept in sync) |

## Subdirectories

(none)

## Search Tags

adjoint-lifting adjoint-triangle-theorem left-adjoint right-adjoint monadic-functor comonadic-functor regular-epi regular-mono reflexive-coequalizer coreflexive-equalizer commutative-square lifting-theorem
