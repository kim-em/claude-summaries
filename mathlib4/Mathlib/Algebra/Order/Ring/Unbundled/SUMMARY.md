---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Ring/Unbundled
generated: 2025-12-01T19:35:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Unbundled

## Overview

The `Unbundled/` directory provides foundational ordered ring theory using unbundled typeclasses (like `Semiring`, `PartialOrder`, `MulPosMono`, `AddLeftMono`) that are later combined into bundled typeclasses like `OrderedSemiring` and `LinearOrderedRing` in the parent directory. This unbundled approach allows expressing precise assumptions for each lemma, with Basic.lean covering general ordered (semi)rings and Rat.lean establishing the linear order on rationals.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core unbundled ordered ring theory: multiplication with nonpositive elements (`mul_le_mul_of_nonpos_left`, `mul_pos_of_neg_of_neg`), monotonicity and antitonicity results, binary rearrangement inequality, sign analysis (`nonneg_and_nonneg_or_nonpos_and_nonpos_of_mul_nonneg`), AM-GM inequality (`two_mul_le_add_sq`, `four_mul_le_sq_add`), and square nonnegativity (`sq_nonneg`, `mul_self_nonneg`) |
| Rat.lean | Linear order on rationals using unbundled typeclasses: `LinearOrder ℚ` instance, `mkRat` sign lemmas (`mkRat_nonneg_iff`, `mkRat_pos_iff`, `mkRat_neg_iff`), ordering characterizations (`divInt_le_divInt`, `div_lt_div_iff_mul_lt_mul`), absolute value structure (`abs_def`, `num_abs_eq_abs_num`), and `OfScientific` instance for nonnegative rationals |

## Subdirectories

(none)

## Search Tags

unbundled-typeclass ordered-ring ordered-semiring linear-order rational-order multiplication-monotonicity nonpositive-multiplication negative-multiplication sign-analysis rearrangement-inequality am-gm-inequality square-nonnegative mkRat divInt scientific-notation absolute-value covariant-class add-left-mono mul-pos-mono pos-mul-mono strict-mono antitone
