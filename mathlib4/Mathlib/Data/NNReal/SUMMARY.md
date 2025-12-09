---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/NNReal
generated: 2025-12-09T00:00:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 3
subdirs_count: 0
---

# NNReal

## Overview

This directory defines and develops the theory of non-negative real numbers (`ℝ≥0`, or `NNReal`), which is the type of real numbers in the interval `[0, ∞)`. The implementation defines `NNReal` as a subtype `{r : ℝ // 0 ≤ r}` and establishes its algebraic structure (conditionally complete linear ordered archimedean commutative semifield), order properties, coercions to/from reals, and operations including arithmetic, suprema/infima, and star structure. This type is fundamental for working with quantities that are inherently non-negative (like distances, norms, measures, probabilities).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `NNReal` as a subtype of reals; establishes algebraic instances (semiring, semifield, ordered structures), coercion to ℝ, conversion from ℝ via `Real.toNNReal`, Galois insertion, conditionally complete linear order properties, arithmetic operations and their coercion lemmas |
| Basic.lean | Extended theory of `NNReal` including floor semiring instance, coercion lemmas for finite sums/products, interactions with suprema/infima (including distributivity over multiplication), subtraction, and division properties |
| Star.lean | Star ring structure on `ℝ≥0` with trivial star (identity) operation; establishes `StarRing`, `TrivialStar`, and `StarModule` instances for compatibility with mathlib's star algebra framework |

## Subdirectories

*(No subdirectories)*

## Search Tags

nonnegative-reals nnreal subtype ordered-semiring semifield conditionally-complete-lattice galois-insertion supremum infimum coercion real-numbers star-ring archimedean canonical-order
