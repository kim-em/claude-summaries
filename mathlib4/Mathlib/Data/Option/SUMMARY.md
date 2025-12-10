---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Option
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 0
---

# Option

## Overview

This folder develops the theory of Lean's `Option α` type, which represents values that may or may not be present (`some a` or `none`). Option types are fundamental for defining partial functions, handling missing values, and serving as prototypes for type extensions (like `WithBot`). The folder provides core definitions, lemmas about the monadic structure of Option, and binary operations (`map₂`) for lifting functions to work with optional values.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Main theory of option types: membership lemmas, `map`/`bind`/`pmap` operations, injectivity properties, `casesOn'` eliminator, `orElse` behavior, monadic operations (`joinM`, `seq`), and `elim` function properties |
| Defs.lean | Extra definitions on Option: `Option.traverse` for applicative traversal, `Option.elim'` (non-dependent eliminator), `iget` (inhabited get with default), and deprecation aliases for `merge` properties |
| NAry.lean | Binary map `Option.map₂ : (α → β → γ) → Option α → Option β → Option γ` that lifts binary functions to options; includes algebraic replacement rules for associativity, commutativity, distributivity, and identity properties |

## Subdirectories

(none)

## Search Tags

option maybe monad partial-function map bind pmap binary-map map2 none some optional monadic applicative elim casesOn traverse iget
