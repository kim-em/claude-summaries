---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Group/Pointwise
generated: 2025-12-01T12:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Pointwise

## Overview

The `Pointwise/` directory provides theory for pointwise operations on sets in ordered monoids and groups. This includes bounds preservation under multiplication/addition, suprema and infima of products/sums of sets (both conditional and complete lattice settings), and comprehensive lemmas about preimages and images of intervals under affine transformations and group operations. The interval file is particularly extensive, covering all standard interval types (Icc, Ico, Ioc, Ioo, Ici, Iic, Ioi, Iio) under various operations.

## Key Files

| File | Purpose |
|------|---------|
| Bounds.lean | Upper/lower bounds preservation under pointwise multiplication: bounded sets multiply to bounded sets, inverse preserves bounds with reversal, range operations |
| CompleteLattice.lean | Suprema and infima of pointwise products/inverses: `sSup (s * t) = sSup s * sSup t`, `sSup s⁻¹ = (sInf s)⁻¹`, both conditional and complete lattice versions |
| Interval.lean | Preimages and images of intervals under group operations: comprehensive coverage of addition/subtraction/multiplication/division/negation/inversion transformations on all interval types, including affine maps in ordered fields |

## Subdirectories

*(No subdirectories)*

## Search Tags

pointwise-operations ordered-sets bounded-sets supremum infimum interval-arithmetic preimage-image group-operations affine-transformations ordered-monoids ordered-groups ordered-fields lattice-operations
