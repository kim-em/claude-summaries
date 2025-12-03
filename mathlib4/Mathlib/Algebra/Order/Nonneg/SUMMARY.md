---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Nonneg
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 6
subdirs_count: 0
---

# Nonneg

## Overview

The `Nonneg/` directory provides a comprehensive theory for the nonnegative subtype `{x : α // 0 ≤ x}` of ordered algebraic structures. This subtype construction lifts algebraic instances (zero, one, addition, multiplication, powers, etc.) and order structures from the base type while preserving their properties through coercion. The directory builds up from basic arithmetic operations through complete algebraic structures (semirings, fields) and includes specialized support for lattice operations, modules, and floor functions. This infrastructure is foundational for working with concrete types like `ℝ≥0` and `ℚ≥0`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core nonnegative subtype infrastructure: Zero, One, Add, Mul, Pow instances with simp/norm_cast lemmas; builds up AddMonoid, AddCommMonoid, Semiring, CommSemiring instances; includes `toNonneg` function (`max a 0`) and truncated subtraction for lattices |
| Ring.lean | Bundled ordered ring instances: IsOrderedAddMonoid, IsOrderedCancelAddMonoid, IsOrderedRing, IsStrictOrderedRing; includes ExistsAddOfLE, Nontrivial, NoZeroDivisors, CanonicallyOrderedAdd, OrderedSub, and LinearOrderedCommMonoidWithZero |
| Field.lean | Semifield structure on nonnegative elements: Inv, Div, Zpow instances, NNRat casting and scalar multiplication, complete Semifield instance, equivalence between units and positive elements (`unitsEquivPos`), LinearOrderedCommGroupWithZero for fields |
| Module.lean | Module structure for nonnegative scalars: proves any R-module M is also an R≥0-module with SMul, SMulWithZero, IsOrderedModule, IsStrictOrderedModule, and full Module instances |
| Lattice.lean | Lattice structures on nonnegative subtypes: OrderBot, NoMaxOrder, SemilatticeSup/Inf, DistribLattice, DenselyOrdered, ConditionallyCompleteLinearOrder, ConditionallyCompleteLinearOrderBot instances |
| Floor.lean | FloorSemiring instance for nonnegative elements: natural-valued floor and ceiling functions inherited from base type with norm_cast lemmas |

## Subdirectories

None

## Search Tags

nonnegative subtype ordered-algebra semiring-instances field-instances module-instances lattice-structures floor-ceiling coercion-lemmas canonical-order truncated-subtraction nnrat-scalar ℝ≥0 ℚ≥0
