---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Polynomial/Resultant
generated: 2026-02-01T19:23:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 1
subdirs_count: 0
---

# Resultant

## Overview

The `Resultant/` directory contains the theory of resultants and discriminants of polynomials over commutative rings. The resultant `Res(f, g)` of two polynomials is defined as the determinant of their Sylvester matrix, and serves as a fundamental tool for detecting when two polynomials share a common root. The discriminant of a polynomial `f` is derived from the resultant of `f` and its derivative, providing information about repeated roots. This file includes the Sylvester matrix construction, comprehensive algebraic properties of resultants (commutativity up to sign, multiplicativity, evaluation formulas), the Sylvester map characterization, and explicit discriminant formulas for quadratic and cubic polynomials.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Complete theory of resultants and discriminants: Sylvester matrix `sylvester f g m n`, resultant `resultant f g` as its determinant, discriminant `discr f` for repeated root detection; key theorems include `resultant_comm` (symmetry up to `(-1)^{mn}`), `resultant_mul_right/left` (multiplicativity), `resultant_eq_prod_roots_sub` (product formula over roots), `resultant_X_sub_C_left` (resultant with linear factor equals evaluation), `isUnit_resultant_iff_isCoprime` (resultant unit iff coprime), Sylvester map linear algebra, and explicit discriminant formulas `discr_of_degree_eq_two` (quadratic: `b^2 - 4ac`) and `discr_of_degree_eq_three` (cubic) |

## Subdirectories

(none)

## Search Tags

resultant discriminant Sylvester-matrix polynomial common-root coprime determinant linear-algebra quadratic-formula cubic-discriminant derivative evaluation roots product-formula ring-theory
