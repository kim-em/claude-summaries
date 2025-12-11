---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/ZMod
generated: 2025-12-11T12:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 10
subdirs_count: 0
---

# ZMod

## Overview

The `ZMod/` directory implements the integers modulo n (written as `ZMod n` or mathematically as Z/nZ). The type `ZMod n` is defined to be `Fin n` for positive n, and `Z` for n=0 (representing all integers with no modular reduction). This directory provides the fundamental ring structure, coercion operations, field instance for prime moduli, the `val` and `valMinAbs` functions for extracting representative integers, connections to quotient groups and quotient rings, unit group operations, and specialized results about factorials and automorphisms in modular arithmetic.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `ZMod n` as `Fin n` (for n > 0) or `Z` (for n = 0); establishes `CommRing` instance; defines ring structure on `Fin n` |
| Basic.lean | Main API for `ZMod`: `val` function returning natural number representative; coercions to/from integers; `CharP n` instance; field structure for prime moduli; Chinese Remainder Theorem (for two moduli); `cast` ring homomorphism |
| Units.lean | Unit group `(ZMod n)^x`: `unitsMap` homomorphism between unit groups; `unitOfCoprime` constructor; surjectivity of unit maps; `eq_unit_mul_divisor` decomposition |
| QuotientGroup.lean | Equivalences between `ZMod n` and quotient groups: `Z / nZ` as additive group quotient; connections to minimal periods and orbit structures; applications to zpowers and zmultiples |
| QuotientRing.lean | Equivalences between `ZMod n` and quotient rings: `Z / (n)` as ideal quotient; Chinese Remainder Theorem for arbitrary finite products; `ZMod.equivPi` decomposition by prime factorization |
| ValMinAbs.lean | The `valMinAbs` function returning integer representative closest to 0 (in interval `(-n/2, n/2]`); comparison with `val`; properties of absolute values and negation |
| Coprime.lean | Connections between coprimality and unit/zero properties: `coe_int_isUnit_iff_isCoprime`; `eq_zero_iff_gcd_ne_one` for prime moduli |
| IntUnitsPower.lean | Power operation on `Z^x` (integer units {1, -1}) by `ZMod 2`, `N`, and `Z`; module structure on `Additive Z^x`; related to `negOnePow` |
| Factorial.lean | Descending factorials in modular arithmetic: `cast_descFactorial` relating `(p-1)!_n` to `(-1)^n * n!` in `ZMod p` |
| Aut.lean | Automorphism group of `ZMod n`: `AddAutEquivUnits` showing `AddAut (ZMod n)` is isomorphic to `(ZMod n)^x` |

## Subdirectories

None.

## Search Tags

zmod integers-modulo-n modular-arithmetic finite-field quotient-ring quotient-group chinese-remainder-theorem units coprime valminabs characteristic-p ring-homomorphism fin
