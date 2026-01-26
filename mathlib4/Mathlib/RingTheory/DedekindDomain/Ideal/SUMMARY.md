---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/DedekindDomain/Ideal
generated: 2026-01-26T20:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 2
subdirs_count: 0
---

# Ideal

## Overview

The `Ideal/` subdirectory contains specialized ideal theory for Dedekind domains, focusing on invertibility of fractional ideals and the unique factorization structure of ideals. It establishes the equivalence between the `IsDedekindDomain` and `IsDedekindDomainInv` definitions (where every nonzero fractional ideal is invertible), provides the `Semifield` and `UniqueFactorizationMonoid` instances for ideals, and develops extensive lemmas for working with prime factorizations, Chinese remainder theorem, and ideal arithmetic in Dedekind domains.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core invertibility theory: defines `IsDedekindDomainInv` (all nonzero fractional ideals invertible), proves equivalence with `IsDedekindDomain`, establishes `Semifield` instance for fractional ideals, and `UniqueFactorizationMonoid` instance for ideals |
| Lemmas.lean | Extensive lemmas on ideal factorization: defines `HeightOneSpectrum` (nonzero prime ideals), proves ideal arithmetic properties (gcd=sup, lcm=inf), Chinese remainder theorem for Dedekind domains, prime power intersections, and bijections between prime factors under ring isomorphisms |

## Subdirectories

*(none)*

## Search Tags

Dedekind-domain invertible-fractional-ideal IsDedekindDomainInv Semifield UniqueFactorizationMonoid ideal-factorization HeightOneSpectrum height-one-spectrum prime-ideal maximal-ideal Chinese-remainder-theorem CRT quotient-equiv prime-factorization normalized-factors multiplicity gcd lcm sup-mul-inf inf-prime-pow ideal-arithmetic PID principal-ideal-domain discrete-valuation-ring DVR primesOver primesOverFinset ring-isomorphism ideal-bijection coprime codisjoint
