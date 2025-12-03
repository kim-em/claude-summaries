---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Field
generated: 2025-12-01T10:10:18Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 10
subdirs_count: 0
---

# Field

## Overview

The `Field/` directory develops comprehensive theory for linearly ordered fields and semifields, where division operations interact with linear order. This is a foundational component of ordered algebra, providing the tools needed for reasoning about division inequalities, fractional arithmetic, and power operations in ordered contexts. The directory focuses on lemmas that are unique to fields (requiring division) and cannot be stated for rings alone.

Key mathematical contributions include: division comparison lemmas relating `a/b` to constants and other divisions; characterizations of positivity and negativity for divisions; integer power (zpow) operations with parity-dependent sign behavior; geometric series bounds for convergence analysis; and specialized constructions like canonically ordered semifields and ordered subfield inheritance. The theory is developed in the unbundled style using `[Field K] [LinearOrder K] [IsStrictOrderedRing K]` rather than bundled typeclasses (which are now deprecated). Applications include interval arithmetic under scalar multiplication, Pi type (function space) lemmas for finite domains, and rational number instances as canonical examples.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Deprecated module for `LinearOrderedSemifield` and `LinearOrderedField` typeclasses (use unbundled `[Semifield K] [LinearOrder K] [IsStrictOrderedRing K]` instead) |
| Basic.lean | Core lemmas for linear ordered semifields: division inequalities (`div_le_self`, `one_lt_div`), halving properties (`half_pos`, `add_div_two_lt_right`), division positivity, and miscellaneous field order results |
| Canonical.lean | Canonically ordered semifields: construction of `LinearOrderedCommGroupWithZero` from canonical order, and truncated subtraction lemma `tsub_div` |
| Power.lean | Integer power operations in ordered fields: even/odd power sign properties (`Even.zpow_nonneg`, `Odd.zpow_neg_iff`), absolute value of powers, and power equality characterizations |
| GeomSum.lean | Geometric series bounds in ordered fields: division formulas for `geom₂_sum` and `geom_sum`, bounds like `geom_sum_lt` for convergence, and inequalities for `geom_sum_Ico` |
| InjSurj.lean | Deprecated module (use `Mathlib.Algebra.Order.Ring.InjSurj` instead) |
| Pi.lean | Pi type (function) lemmas for fields: existence of uniform positive additions (`Pi.exists_forall_pos_add_lt`) in finite domain functions into densely ordered fields |
| Pointwise.lean | Pointwise scalar multiplication on intervals in ordered fields: `smul_Ioo`, `smul_Icc`, etc., showing that scaling by positive element preserves interval structure |
| Rat.lean | Rational number ordered field instances: `LinearOrderedCommGroupWithZero` instance for `NNRat` (nonnegative rationals) |
| Subfield.lean | Ordered instances on subfields: `IsStrictOrderedRing` instance showing that subfields of ordered fields inherit strict ordering |

## Subdirectories

(none)

## Search Tags

ordered-field linear-ordered-field semifield division-inequalities geometric-series integer-powers zpow halving-lemmas canonically-ordered pointwise-intervals subfield rational-numbers nnrat power-sign even-odd-powers field-order
