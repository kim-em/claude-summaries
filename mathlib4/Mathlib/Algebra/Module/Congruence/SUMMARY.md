---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Module/Congruence
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# Congruence

## Overview

This directory defines congruence relations that respect scalar multiplication and additive structure on modules. It provides three levels of structure: `SMulCon` for relations preserving scalar multiplication, `VAddCon` for additive actions, and `ModuleCon` for relations preserving both addition and scalar multiplication. The quotient types by these congruences inherit appropriate algebraic instances (including `Module` for `ModuleCon`), and the directory establishes the first isomorphism theorem for modules via the kernel construction.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `SMulCon`, `VAddCon`, and `ModuleCon` structures; quotient constructions with inherited instances (`MulAction`, `DistribMulAction`, `Module`); kernel congruences for homomorphisms; first isomorphism theorem `quotientKerEquivOfSurjective` |

## Subdirectories

None.

## Search Tags

congruence-relation module-congruence scalar-multiplication equivalence-relation quotient-module kernel isomorphism-theorem smul-con module-con vadd-con first-isomorphism-theorem setoid
