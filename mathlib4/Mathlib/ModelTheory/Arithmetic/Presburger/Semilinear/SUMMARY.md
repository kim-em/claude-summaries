---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/ModelTheory/Arithmetic/Presburger/Semilinear
generated: 2026-01-25T20:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Semilinear

## Overview

The `Semilinear/` directory contains a comprehensive formalization of linear and semilinear sets in additive commutative monoids. Linear sets are cosets of finitely generated additive submonoids, and semilinear sets are finite unions of linear sets. The files prove that semilinear sets form a Boolean algebra (closed under union, intersection, complement, and set difference) and establish the proper decomposition theorem showing every semilinear set can be expressed as a finite union of proper linear sets with linearly independent generators.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines linear sets (cosets of finitely generated submonoids), semilinear sets (finite unions of linear sets), proper linear sets (with linearly independent periods), and proper semilinear sets; proves closure under union, projection, set addition, and additive closure; establishes the proper decomposition theorem |
| Basic.lean | Proves semilinear sets are closed under intersection, set difference, and complement (in finitely generated monoids); establishes semilinearity of linear equation solutions; includes technical results about slice properties, preimages, and matrix representations |

## Subdirectories

(none)

## Search Tags

semilinear-sets linear-sets additive-monoid proper-decomposition linear-independence presburger-arithmetic boolean-algebra closure-properties ginsburg-spanier eilenberg finite-union coset finitely-generated slice-property linear-equations
