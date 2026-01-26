---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Probability/Independence/Kernel
generated: 2026-01-26T19:58:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Kernel

## Overview

The `Kernel/` directory provides kernel-based definitions of independence concepts that generalize both unconditional independence and conditional independence. These definitions work with respect to a kernel `κ : Kernel α Ω` and a measure `μ` on `α`, where conditional independence uses `condExpKernel` and unconditional independence uses `Kernel.const Unit μ`. The directory contains the fundamental machinery used by the main independence concepts defined in the parent directory.

## Key Files

| File | Purpose |
|------|---------|
| Indep.lean | Core kernel-based independence definitions for families of sets/σ-algebras: `iIndepSets` (π-systems independent under kernel), `iIndep` (σ-algebras), `iIndepSet` (sets); pairwise variants `IndepSets`, `Indep`, `IndepSet`; π-system lemma (independent π-systems generate independent σ-algebras); independence of suprema of directed/monotone families of σ-algebras |
| IndepFun.lean | Kernel-based independence for random variables: `iIndepFun` (family of functions), `IndepFun` (pair of functions); characterizations via preimage measures and joint distributions; independence preserved under composition and arithmetic operations (addition, multiplication, division); independence of finite products and tuples; conditional probability factorization for independent random variables |

## Subdirectories

(none)

## Search Tags

kernel independence conditional-independence markov-kernel pi-system sigma-algebra random-variables indepfun indepset indepsets generating-systems preimage-measures joint-distribution composition product-measures supremum directed-families monotone-families conditional-expectation probability-theory measure-theory
