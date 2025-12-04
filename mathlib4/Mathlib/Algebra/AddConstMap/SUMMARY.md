---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/AddConstMap
generated: 2025-12-04T13:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# AddConstMap

## Overview

This directory defines bundled maps and equivalences that semiconjugate shifts, i.e., functions `f : G → H` satisfying `f (x + a) = f x + b`. This abstraction provides a framework for studying lifts of circle maps (self-maps of the unit circle) to the real line and more generally for working with maps between additive structures that respect shifted addition. The theory includes both one-way maps (`AddConstMap`) and equivalences (`AddConstEquiv`) with comprehensive algebraic structure.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and theory: `AddConstMap G H a b` (notation `G →+c[a, b] H`) for bundled maps satisfying `f (x + a) = f x + b`, `AddConstMapClass` typeclass, extensive library of lemmas for computing `f (x + n • a)` and `f (x + n)` for natural/integer scalars, monotonicity characterization on fundamental intervals for archimedean ordered groups, monoid structure on endomorphisms `G →+c[a, a] G`, additive actions, scalar multiplication, negation conjugation for additive groups, and floor ring construction `mkFract` defining maps from their values on `[0, 1)` |
| Equiv.lean | Equivalences conjugating shifts: `AddConstEquiv G H a b` (notation `G ≃+c[a, b] H`) combining `Equiv` and `AddConstMap` structures, symmetry/transitivity/composition operations preserving the property, group structure on automorphisms `G ≃+c[a, a] G` with inversion and integer powers, monoid homomorphisms to permutations and `AddConstMap`, and group equivalence between `G ≃+c[a, a] G` and units of `G →+c[a, a] G` |

## Subdirectories

(No subdirectories)

## Search Tags

add-const-map shift-semiconjugacy circle-lifts unit-circle additive-structures bundled-maps equivalences monotonicity archimedean floor-ring fundamental-interval
