---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Nat/NthRoot
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 0
---

# NthRoot

## Overview

This folder provides the definition of the natural number nth root function `Nat.nthRoot`. The function computes the floor of the nth root of a natural number, i.e., `Nat.nthRoot n a = ⌊a^(1/n)⌋`. It is implemented using Newton's method for superexponential convergence and is defined purely in terms of natural numbers with no dependencies outside the prelude.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `Nat.nthRoot n a` using Newton's method; handles edge cases (n=0 returns 1, n=1 returns a); includes tail-recursive helper `go` with fuel parameter for termination |

## Subdirectories

(none)

## Search Tags

nth-root natural-numbers floor newton-method integer-root radical
