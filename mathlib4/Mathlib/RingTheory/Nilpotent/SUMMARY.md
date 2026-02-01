---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Nilpotent
generated: 2026-02-01T10:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 5
subdirs_count: 0
---

# Nilpotent

## Overview

This folder develops the theory of nilpotent elements in rings and monoids. An element `x` is nilpotent if `x^n = 0` for some positive integer `n`. The theory covers basic properties (closure under negation, scalar multiplication, addition/subtraction of commuting elements), the nilpotency class (smallest exponent making the power zero), the nilradical ideal (all nilpotent elements in a commutative semiring), reduced rings (rings with no nonzero nilpotent elements), the exponential map for nilpotent elements in ℚ-algebras, and geometrically reduced algebras (reduced after base change to algebraic closure).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `IsNilpotent`, `nilpotencyClass`, `IsRadical`; basic lemmas on mapping nilpotent elements, unit-nilpotent products, reduced type instances |
| Basic.lean | Closure properties: nilpotent elements closed under negation, scalar multiplication; `1 ± nilpotent` is a unit; sums/finitary sums of commuting nilpotents are nilpotent; idempotent nilpotent is zero |
| Lemmas.lean | Ring-theoretic results: nilradical definition and characterization via prime ideals; equivalence of radical ideals and reduced quotients; nilpotency for matrix representations and linear maps |
| Exp.lean | Exponential map `IsNilpotent.exp` on ℚ-algebras; proves `exp(a+b) = exp(a)*exp(b)` for commuting nilpotents, `exp(a)` is a unit, functoriality under ring homomorphisms, derivation compatibility |
| GeometricallyReduced.lean | Geometrically reduced algebras: `IsGeometricallyReduced k A` when `AlgebraicClosure k ⊗[k] A` is reduced; shows property transfers through injective algebra maps and is determined by finitely generated subalgebras |

## Subdirectories

(none)

## Search Tags

nilpotent nilpotency-class nilradical reduced-ring isreduced isradical prime-ideal exponential-map exp geometrically-reduced algebra tensor-product unit commute radical-ideal linear-map matrix quotient
