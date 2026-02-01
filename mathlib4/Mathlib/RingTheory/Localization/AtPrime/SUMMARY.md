---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Localization/AtPrime
generated: 2026-02-01T12:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 2
subdirs_count: 0
---

# AtPrime

## Overview

This directory contains the theory of localization at prime ideals in commutative algebra. It extends the general localization theory to the specific case where `S` is the localization of a ring `R` at the complement of a prime ideal `P` (denoted `P.primeCompl`). The key result is that such localizations are always local rings, with maximal ideal corresponding to the image of `P`. The development includes bijections between prime ideals of the localization and primes contained in `P`, residue field isomorphisms, and for Dedekind domains, preservation of ramification indices and inertia degrees under localization.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory: `IsLocalization.AtPrime` typeclass abbreviation, `Localization.AtPrime` type abbreviation, proof that localization at prime complement is a local ring (`AtPrime.isLocalRing`), `orderIsoOfPrime` bijection between primes of localization and primes contained in P, `comap_maximalIdeal`, `localRingHom` for induced maps, `equivQuotMaximalIdeal` isomorphism showing localization preserves residue field, `equivQuotientMapMaximalIdeal` for extensions |
| Extension.lean | Primes in extensions of localizations at primes: for Dedekind domain extensions R to S with prime p, establishes bijection `primesOverEquivPrimesOver` between primes of S over p and primes of localized Sp over maximal ideal, proves inertia degree and ramification index are preserved by this bijection |

## Subdirectories

(none)

## Search Tags

localization AtPrime prime-ideal local-ring IsLocalization Localization primeCompl maximalIdeal isLocalRing orderIsoOfPrime comap localRingHom residue-field equivQuotMaximalIdeal Dedekind-domain ramification-index inertia-degree primesOver primesOverEquivPrimesOver extension algebra LiesOver
