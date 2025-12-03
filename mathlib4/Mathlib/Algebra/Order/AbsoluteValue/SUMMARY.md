---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/AbsoluteValue
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# AbsoluteValue

## Overview

The `AbsoluteValue/` directory defines absolute value functions on ordered algebraic structures. It provides both bundled (`AbsoluteValue R S`) and unbundled (`IsAbsoluteValue`) approaches to absolute values, establishing their core properties (nonnegativity, positive definiteness, triangle inequality, multiplicativity) and interactions with algebraic operations. The directory includes the standard absolute value on rings, the trivial absolute value, nontriviality criteria, and specialization to Euclidean absolute values that preserve the structure of Euclidean domains.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core absolute value theory: bundled `AbsoluteValue R S` structure extending `MulHom` with nonnegativity/triangle inequality/positive definiteness, homomorphism class instances, standard absolute value `AbsoluteValue.abs`, trivial absolute value (1 on nonzero elements), nontriviality predicate, and unbundled `IsAbsoluteValue` typeclass with conversions |
| Euclidean.lean | Euclidean absolute values: `AbsoluteValue.IsEuclidean abv` predicate asserting compatibility with `EuclideanDomain` structure (`abv x < abv y ↔ x ≺ y`), with proof that standard integer absolute value `abs : ℤ → ℤ` is Euclidean |

## Subdirectories

(none)

## Search Tags

absolute-value bundled-absolute-value unbundled-absolute-value triangle-inequality multiplicative-norm positive-definite nonnegative-homomorphism trivial-absolute-value nontrivial-absolute-value euclidean-absolute-value euclidean-domain integer-absolute-value monoid-with-zero-hom mul-ring-norm subadditive standard-absolute-value IsAbsoluteValue
