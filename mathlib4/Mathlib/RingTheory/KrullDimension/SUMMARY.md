---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/KrullDimension
generated: 2026-02-01T07:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 9
subdirs_count: 0
---

# KrullDimension

## Overview

This folder formalizes the Krull dimension of commutative rings, defined as the order-theoretic Krull dimension of the prime spectrum (the supremum of lengths of chains of prime ideals). The development includes the basic definition (`ringKrullDim`), dimension bounds for special classes of rings (fields, local rings, PIDs), behavior under quotients and polynomial/power series extensions, and dimension theory for modules. Key results include that PIDs have dimension at most 1, the dimension formula `dim R[X] = dim R + 1` for Noetherian rings, and the regular sequence dimension formula for modules over local rings.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `ringKrullDim`, `Ring.KrullDimLE n`, `FiniteRingKrullDim`; dimension behavior under quotients and surjective ring homomorphisms; characterization of dimension 0 (primes are maximal) and dimension 1 rings; Jacobson equals nilradical for dimension 0 rings |
| Field.lean | Proves that fields have Krull dimension 0 (`ringKrullDim_eq_zero_of_field`) |
| LocalRing.lean | Characterizes when a local domain has dimension 1 via the maximal ideal being contained in radicals of principal ideals |
| Module.lean | Defines `Module.supportDim R M` as the Krull dimension of a module's support; relates it to `ringKrullDim (R ⧸ Ann M)` for finitely generated modules |
| NonZeroDivisors.lean | Key inequalities: `dim R/r + 1 ≤ dim R` for nonzerodivisors r; `dim R + 1 ≤ dim R[X]`; `dim R + n ≤ dim R[X₁,...,Xₙ]`; analogous results for power series |
| PID.lean | Proves PIDs satisfy `Ring.KrullDimLE 1`; non-field PIDs have dimension exactly 1; maximal ideals in PIDs have height 1 |
| Polynomial.lean | Main Noetherian results: `dim R[X] = dim R + 1` and `dim R[X₁,...,Xₙ] = dim R + n`; also upper bound `dim R[X] ≤ 2·dim R + 1` for general rings |
| Regular.lean | Regular sequence dimension formulas: `dim M/(r₁,...,rₙ)M + n = dim M` for M-sequences over Noetherian local rings; related results for ring quotients |
| Zero.lean | Detailed API for zero-dimensional rings: equivalent characterizations, behavior in local rings (unique prime ideal, nilradical = maximal ideal), Jacobson ring instance |

## Subdirectories

(none)

## Search Tags

krull-dimension ring-dimension dim prime-spectrum chain-of-primes PID principal-ideal-domain field local-ring polynomial dimension-formula noetherian regular-sequence module-support zero-dimensional jacobson nilradical maximal-ideal height
