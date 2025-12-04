---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/SkewPolynomial
generated: 2025-12-04T19:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# SkewPolynomial

## Overview

This directory defines univariate skew polynomials (also called twisted polynomials), a generalization of ordinary polynomials where multiplication is twisted by a ring endomorphism φ. While addition is standard polynomial addition, multiplication is governed by the rule `Xa = φ(a)X`. The implementation builds on `SkewMonoidAlgebra R (Multiplicative ℕ)` and requires a `MulSemiringAction` to specify the endomorphism. This structure is fundamental in areas like the theory of division algebras over finite fields, where φ might be the Frobenius endomorphism.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `SkewPolynomial R` as a synonym for `SkewMonoidAlgebra R (Multiplicative ℕ)`, provides basic algebraic instances (semiring, module), defines support/monomial operations, and establishes the multiplication rule `monomial n r * monomial m s = monomial (n + m) (r * φ^[n] s)` where φ is the ring endomorphism derived from the action |

## Subdirectories

None

## Search Tags

skew-polynomial twisted-polynomial noncommutative-polynomial endomorphism frobenius ore-extension division-algebra finite-field polynomial-generalization skew-multiplication monoid-algebra
