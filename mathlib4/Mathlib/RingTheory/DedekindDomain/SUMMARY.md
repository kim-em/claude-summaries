---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/DedekindDomain
generated: 2026-01-26T20:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 14
subdirs_count: 1
---

# DedekindDomain

## Overview

The `DedekindDomain/` directory contains the formalization of Dedekind domains and Dedekind rings, which are Noetherian integrally closed domains (or rings) of Krull dimension at most one. This theory is fundamental to algebraic number theory, providing the framework for studying rings of integers in number fields and their generalizations. The directory includes multiple equivalent characterizations (dimension ≤ 1, DVR localizations, UFD structure), extensive factorization theory for ideals and fractional ideals, adic valuations and completions, the different ideal for ring extensions, and specialized structures like S-integers, S-units, Selmer groups, and the finite adèle ring.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `IsDedekindRing` (Noetherian, integrally closed, dimension ≤ 1) and `IsDedekindDomain` (additionally an integral domain); proves PIDs are Dedekind domains |
| Dvr.lean | Equivalent characterization: Dedekind domains as Noetherian domains where localization at every nonzero prime is a DVR (discrete valuation ring); shows `IsDedekindDomain` ⟺ `IsDedekindDomainDvr` |
| PID.lean | Criteria for when a Dedekind domain is a PID: finite maximal ideals, finite primes, or UFD structure implies PID; includes localization over prime results |
| Factorization.lean | Factorization of nonzero ideals and fractional ideals as products ∏ v^(nᵥ) over maximal ideals; defines `FractionalIdeal.count` (multiplicity), proves finite support and finprod factorizations |
| AdicValuation.lean | v-adic valuations on Dedekind domains and fraction fields; defines `intValuation` and `valuation`, proves uniformizer existence, constructs `adicCompletion` and `adicCompletionIntegers` |
| Different.lean | Different ideal 𝔇 for ring extensions; defines `Submodule.traceDual` and `FractionalIdeal.dual` under trace form; proves conductor-different formula f'(x) ∈ 𝔇 and ramification criterion |
| IntegralClosure.lean | Proves integral closure of a Dedekind domain in a finite separable extension is again a Dedekind domain; shows integral closure is localization at nonzero divisors |
| Instances.lean | Infrastructure for working with localizations of ring extensions; provides compatible algebra instances for towers R ⊆ S with localizations Rₚ ⊆ Sₚ and fraction fields K ⊆ L |
| GaussLemma.lean | Gauss's Lemma for Dedekind domains: content ideal equals ⊤ iff all v-adic Gauss norms equal 1; PID version with primitive polynomials |
| SInteger.lean | S-integers (v-adic valuation ≤ 1 for v ∉ S) and S-units (v-adic valuation = 1 for v ∉ S); defines `Set.integer` subalgebra and `Set.unit` subgroup |
| SelmerGroup.lean | Selmer groups K(S,n) as subgroup of Kˣ/(Kˣ)ⁿ with v-adic valuations divisible by n for v ∉ S; framework for fundamental exact sequence with class groups and unit groups |
| LinearDisjoint.lean | Results on extensions with coprime different ideals; if Frac(R₁) ⊔ Frac(R₂) = Frac(B) are linearly disjoint and differents are coprime, then 𝔇(B/A) = 𝔇(R₁/A)·𝔇(R₂/A) |
| FiniteAdeleRing.lean | Finite adèle ring of R as restricted product ∏ʳ_v K_v over maximal ideals v with respect to rings of integers; defines topology and commutative ring structure |

## Subdirectories

- [x] `Ideal/` - Specialized ideal theory for Dedekind domains

## Search Tags

Dedekind-domain Dedekind-ring Noetherian integrally-closed Krull-dimension discrete-valuation-ring DVR principal-ideal-domain PID unique-factorization-domain UFD fractional-ideal factorization multiplicity count adic-valuation valuation uniformizer completion different-ideal conductor ramification unramified trace-dual S-integer S-unit Selmer-group adele finite-adele restricted-product localization height-one-spectrum maximal-ideal algebraic-number-theory number-field ring-of-integers Gauss-lemma content-ideal primitive-polynomial linear-disjoint coprime-different
