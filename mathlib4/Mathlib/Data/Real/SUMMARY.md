---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Real
generated: 2025-12-11T22:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 16
subdirs_count: 1
---

# Real

## Overview

The `Real/` directory defines the real numbers `ℝ` as equivalence classes of Cauchy sequences of rationals, along with their fundamental algebraic and order-theoretic properties. This includes the Archimedean property, floor ring structure, conditional completeness (existence of suprema for bounded sets), square roots, the sign function, conjugate exponents for Holder inequalities, and the star-ordered ring structure. Several files are deprecated redirects to `Analysis/Real/` where the content has been moved.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `ℝ` as Cauchy sequence equivalence classes; defines `Real` structure, zero, one, add, neg, mul, inv operations; proves it's a commutative ring |
| Archimedean.lean | Proves `ℝ` is Archimedean, provides `FloorRing` instance, proves conditional completeness (`exists_isLUB`), characterizes Cauchy sequences |
| Sqrt.lean | Defines `NNReal.sqrt` as an `OrderIso` and `Real.sqrt` via `toNNReal`; proves algebraic properties of square root |
| ConjExponents.lean | Defines Holder triples and conjugate exponents (`p⁻¹ + q⁻¹ = r⁻¹`) for L^p space theory; includes `Real.HolderTriple`, `Real.HolderConjugate`, `conjExponent` |
| Embedding.lean | Provides embedding of any Archimedean group into `ℝ` via `Archimedean.embedReal` |
| Pointwise.lean | Relates `sInf`/`sSup` of scalar multiples with scalar multiples of `sInf`/`sSup`; distributes multiplication over indexed infima/suprema |
| Sign.lean | Defines `Real.sign` function: -1 for negative, 0 for zero, 1 for positive |
| ENatENNReal.lean | Coercion from `ℕ∞` to `ℝ≥0∞` as order embedding and ring homomorphism |
| CompleteField.lean | Establishes `ℝ` as a `ConditionallyCompleteLinearOrderedField`; proves uniqueness of ring endomorphisms on `ℝ` |
| Star.lean | Provides trivial star-ring structure on `ℝ` (star is identity) |
| StarOrdered.lean | Proves `ℝ` and `ℝ≥0` are star-ordered rings using square root characterization |
| Cardinality.lean | Deprecated redirect to `Mathlib/Analysis/Real/Cardinality` |
| EReal.lean | Deprecated redirect to `Mathlib/Data/EReal/Basic` |
| Hyperreal.lean | Deprecated redirect to `Mathlib/Analysis/Real/Hyperreal` |
| Irrational.lean | Deprecated redirect to `Mathlib/NumberTheory/Real/Irrational` |

## Subdirectories

- [x] `Pi/` - Deprecated redirect stubs for pi-related content (bounds, irrationality, Leibniz/Wallis formulas), now in `Analysis/Real/Pi/`

## Search Tags

real-numbers cauchy-sequences archimedean floor-ring conditionally-complete square-root sqrt holder-conjugate exponents sign-function star-ring embedding pointwise supremum infimum
