---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Module/Torsion
generated: 2025-12-01T07:55:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# Torsion

## Overview

The `Torsion/` directory contains the comprehensive theory of torsion submodules and torsion-free modules. It defines various notions of torsion (by single elements, by sets, by multiplicative subsets), the complementary notion of torsion-free modules (where scalar multiplication by regular elements is injective), and establishes fundamental properties including decomposition theorems for coprime torsion, quotient constructions, and closure properties under products. The directory includes both the classical torsion submodule theory and the modern torsion-free formulation, with the key result that vector spaces (modules over division rings) are torsion-free.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core torsion theory: `Ideal.torsionOf R M x` (torsion ideal of element), `Submodule.torsionBy R M a` (a-torsion submodule), `torsionBySet` (torsion by set of scalars), `torsion' R M S` (S-torsion submodule), `torsion R M` (torsion by non-zero-divisors), module predicates `IsTorsionBy`/`IsTorsionBySet`/`IsTorsion'`/`IsTorsion`, isomorphism `quotTorsionOfEquivSpanSingleton` between span and quotient by torsion ideal, decomposition theorems for coprime torsion (`torsionBy_isInternal`, `torsionBySet_isInternal`), quotient-by-torsion is torsion-free, characterization over domains via `NoZeroSMulDivisors` |
| Free.lean | Torsion-free modules: `Module.IsTorsionFree R M` typeclass (scalar multiplication by regular elements is injective), basic properties (`IsRegular.smul_right_injective`, `smul_eq_zero_iff_right`), equivalence between `IsTorsionFree ℕ M` and `IsAddTorsionFree M`, equivalence between `IsTorsionFree ℤ M` and `IsAddTorsionFree M` for char-zero domains, instances for `R` (self), opposite rings, pullback along injections |
| Field.lean | Vector spaces are torsion-free: `DivisionSemiring.to_moduleIsTorsionFree` instance showing any module over a division semiring is torsion-free (proof via scalar inverse) |
| Pi.lean | Product preservation: `Pi.instModuleIsTorsionFree` showing dependent products of torsion-free modules are torsion-free |
| Prod.lean | Binary product preservation: `Prod.moduleIsTorsionFree` showing binary products `M × N` of torsion-free modules are torsion-free |

## Subdirectories

*(No subdirectories)*

## Search Tags

torsion torsion-free torsion-submodule torsion-ideal annihilator coprime-decomposition internal-direct-sum quotient-torsion zero-divisor regular-element division-ring vector-space product-preservation galois-connection
