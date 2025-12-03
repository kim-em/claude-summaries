---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Pointwise/Finset
generated: 2025-12-01T22:00:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# Finset

## Overview

The `Finset/` subdirectory implements pointwise algebraic operations on finite sets (`Finset`), providing the finite analogue of pointwise operations on sets. This includes definitions of pointwise addition/multiplication (`s + t`, `s * t`), negation/inversion (`-s`, `s⁻¹`), subtraction/division (`s - t`, `s / t`), and scalar operations (`a • s`, `s • t`). The instances are placed in the `Pointwise` scope to avoid conflicts with the natural monoid structure on finsets. The development includes basic operations, compatibility with big operators, density preservation theorems, interval subset relationships, and comprehensive scalar action definitions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of pointwise operations: singleton `0`/`1`, negation/inversion, addition/multiplication, subtraction/division on finsets with semigroup/monoid instances |
| BigOperators.lean | Interaction between pointwise operations and big operators: `coe_prod` for products over finsets, index rewriting for inverted/negated index sets |
| Density.lean | Density preservation theorems showing that pointwise operations (inversion, scalar multiplication) preserve the density of finsets |
| Interval.lean | Subset relationships for pointwise multiplication/addition on intervals (`Icc`, `Ico`, `Ioc`, etc.) with monotonicity assumptions |
| Scalar.lean | Scalar addition (`+ᵥ`), scalar multiplication (`•`), and scalar subtraction (`-ᵥ`) operations on finsets with associated lemmas and instances |

## Subdirectories

No subdirectories.

## Search Tags

finset pointwise-operations pointwise-multiplication pointwise-addition finset-operations singleton-finset negation-finset inversion-finset addition-finset multiplication-finset subtraction-finset division-finset scalar-multiplication scalar-addition big-operators density interval-arithmetic monotonicity locally-finite-order
