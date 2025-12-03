---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/GroupWithZero/Unbundled
generated: 2025-12-01T20:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 4
subdirs_count: 0
---

# Unbundled

## Overview

The `Unbundled/` directory provides fine-grained, unbundled typeclasses for monotonicity and covariance properties of multiplication in ordered structures with zero. These typeclasses decompose the properties of ordered semirings and fields into eight granular classes (`PosMulMono`, `PosMulStrictMono`, `PosMulReflectLT`, `PosMulReflectLE`, and their right-multiplication counterparts), expressing precisely when multiplication by nonnegative or positive elements preserves or reflects order relations. The directory also constructs order isomorphisms for multiplication by positive elements in groups with zero, enabling lattice operations like `mul_inf₀` and `mul_sup₀`.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines eight core unbundled typeclasses for multiplication monotonicity: `PosMulMono` (left multiplication by nonnegative preserves ≤), `PosMulStrictMono` (left by positive preserves <), `PosMulReflectLT/LE` (left multiplication reflects order), and their right-multiplication counterparts `MulPosMono`, `MulPosStrictMono`, `MulPosReflectLT/LE`; includes conversions between classes, equivalences for commutative multiplication, and implications under linear order |
| Basic.lean | Comprehensive lemmas building on the typeclass definitions: sign preservation (`mul_pos`, `mul_nonneg`, `mul_neg_of_pos_of_neg`), reflection lemmas (`pos_of_mul_pos_right`), bi-monotonicity (`mul_lt_mul_of_nonneg`), and various multiplication inequality lemmas for structures with `MulZeroClass` |
| OrderIso.lean | Order isomorphisms for multiplication in groups with zero: `OrderIso.mulLeft₀` and `mulRight₀` express multiplication by positive elements as order-preserving equivalences, enabling lattice distribution lemmas `mul_inf₀`, `mul_sup₀`, `inf_mul₀`, `sup_mul₀` via `divRight₀` |
| Lemmas.lean | Deprecated file (since 2025-04-13) that simply redirects to `OrderIso` |

## Subdirectories

*None*

## Search Tags

unbundled-typeclasses covariance-classes contravariance-classes multiplication-monotonicity pos-mul-mono pos-mul-strict-mono mul-pos-reflect ordered-multiplication nonnegative-elements positive-elements order-isomorphism mul-left-zero mul-right-zero lattice-distribution gcongr-lemmas
