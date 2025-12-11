---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Sym/Sym2
generated: 2025-12-11T01:16:50Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 0
---

# Sym2

## Overview

This directory contains supplementary functionality for the symmetric square (`Sym2`), which represents unordered pairs. It provides an Aesop rule set for automated tactics, lifting of finitely supported functions to the symmetric square via multiplication, and order-theoretic operations including sorting symmetric squares into canonical ordered pairs.

## Key Files

| File | Purpose |
|------|---------|
| Init.lean | Declares the `Sym2` Aesop rule set for automated reasoning; must be imported to make the rule set visible |
| Finsupp.lean | Lifts `α →₀ M₀` to `Sym2 α →₀ M₀` via `sym2Mul`, composing with `Sym2.mul`; provides support lemmas relating `f.support.sym2` to preimages of multiplication |
| Order.lean | Defines `sup` and `inf` operations on `Sym2` for lattices; provides `sortEquiv : Sym2 α ≃ { p : α × α // p.1 ≤ p.2 }` for linear orders, canonically identifying symmetric squares with sorted pairs |

## Subdirectories

(none)

## Search Tags

symmetric-square unordered-pairs Sym2 aesop finsupp lifting sup inf sorting linear-order lattice equivalence ordered-pairs
