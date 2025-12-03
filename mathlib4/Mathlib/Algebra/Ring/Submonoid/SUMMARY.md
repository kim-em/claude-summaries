---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Submonoid
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Submonoid

## Overview

The `Submonoid/` directory develops the theory of (additive) submonoids within rings and semirings, focusing on closure properties under multiplication and pointwise operations. This is complementary to the group-theoretic submonoid theory, establishing how multiplicative substructures interact with the additive closure operation and defining monoid structures on collections of additive submonoids via pointwise multiplication.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Lemmas about additive closures of multiplicative subsemigroups: closure of products under multiplication (`mul_mem_add_closure`, `mul_left_mem_add_closure`, `mul_right_mem_add_closure`) |
| Pointwise.lean | Pointwise multiplication and scalar multiplication on additive submonoids: `AddSubmonoid.mul`, `AddSubmonoid.smul`, monoid structure on `AddSubmonoid R` in the `Pointwise` locale, including `MulOneClass`, `Semigroup`, `Monoid` instances |

## Subdirectories

(none)

## Search Tags

submonoid additive-submonoid additive-closure multiplicative-subsemigroup pointwise-multiplication pointwise-operations monoid-structure distribsmul semiring closure-induction mul-mem-add-closure
