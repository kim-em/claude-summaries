---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/SModEq
generated: 2026-01-25T22:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# SModEq

## Overview

The `SModEq/` directory formalizes modular equivalence for submodules, providing a predicate `SModEq` (notation `x ≡ y [SMOD U]`) that defines when two elements of a module are equivalent modulo a submodule. The framework establishes that `x ≡ y [SMOD U]` if and only if their difference `x - y` belongs to `U`, which is equivalent to equality in the quotient module `M ⧸ U`. The theory includes reflexivity, symmetry, transitivity, congruence properties for arithmetic operations (addition, scalar multiplication, negation, subtraction), and compatibility with linear maps through `map` and `comap`. For ideals in commutative rings, the framework extends to multiplication, products, powers, and polynomial evaluation.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `SModEq` definition: equivalence relation `x ≡ y [SMOD U]` as equality in quotient `M ⧸ U`, characterization via `sub_mem` (x - y ∈ U), reflexivity/symmetry/transitivity, congruence for addition (add, sum), scalar multiplication (smul, nsmul, zsmul), negation, subtraction, monotonicity (mono), special cases (top, bot, zero), interaction with linear maps (map, comap), and ring operations for ideals (mul, prod, pow, eval for polynomial evaluation) |
| Pointwise.lean | Additional pointwise lemmas: `smul'` variant where scalar belongs to an ideal I and equivalence modulo U implies c • x ≡ c • y [SMOD (I • U)] for c ∈ I |

## Subdirectories

*None*

## Search Tags

smodEq modular-equivalence submodule quotient-module equivalence-relation congruence scalar-multiplication linear-map ideal polynomial-evaluation
