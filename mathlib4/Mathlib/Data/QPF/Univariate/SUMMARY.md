---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/QPF/Univariate
generated: 2025-12-11T09:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# Univariate

## Overview

Univariate Quotients of Polynomial Functors (QPFs) for type functors `F : Type u → Type v`. This module defines the `QPF` class which represents a functor as a quotient of a polynomial functor via abstraction (`abs`) and representation (`repr`) functions. The key constructions are `Fix` (initial algebra/inductive type) and `Cofix` (final coalgebra/coinductive type), along with composition and quotient operations that preserve the QPF structure.

## Key Files

| File | Purpose |
|------|---------|
| `Basic.lean` | Defines the `QPF` class with `abs`/`repr` operations; constructs `Fix` (initial algebra) as a quotient of W-types under `Wequiv`, and `Cofix` (final coalgebra) as a quotient of M-types under `Mcongr`; proves that QPF composition and quotients preserve QPF structure; provides support set theory (`supp`, `IsUniform`, `LiftpPreservation`, `SuppPreservation`) |

## Subdirectories

(none)

## Search Tags

qpf quotient-polynomial-functor univariate fix cofix initial-algebra final-coalgebra wequiv mcongr functor-composition quotient-functor liftp liftr supp uniform bisimulation coinduction induction
