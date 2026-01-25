---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/ModelTheory/Arithmetic/Presburger
generated: 2026-01-25T20:35:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 1
---

# Presburger

## Overview

The `Presburger/` directory contains a formalization of Presburger arithmetic and its foundational semilinear set theory. Presburger arithmetic is the first-order theory of natural numbers with addition (0, 1, +), a decidable fragment of arithmetic that omits multiplication. The directory defines the language of Presburger arithmetic (`Basic.lean`) and provides a comprehensive theory of semilinear sets (`Semilinear/`), which characterize the definable sets in Presburger arithmetic. The semilinear theory establishes that such sets form a Boolean algebra and includes the proper decomposition theorem, fundamental results for understanding the expressiveness and decidability of Presburger arithmetic.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the language of Presburger arithmetic as (0,1,+), including the inductive type for functions, term structure with zero/one/add instances, natural number casting, scalar multiplication, and summation over finite sets with realization theorems |

## Subdirectories

- [x] `Semilinear/` - Theory of linear and semilinear sets in additive commutative monoids, proving Boolean algebra closure properties and the proper decomposition theorem

## Search Tags

presburger-arithmetic first-order-logic model-theory decidable-arithmetic semilinear-sets linear-sets additive-monoid quantifier-elimination finitely-generated-monoid proper-decomposition ginsburg-spanier
