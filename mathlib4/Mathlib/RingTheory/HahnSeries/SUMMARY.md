---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/HahnSeries
generated: 2026-01-26T08:25:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 11
subdirs_count: 0
---

# HahnSeries

## Overview

The `HahnSeries/` directory contains a comprehensive formalization of Hahn series, which generalize Laurent series by allowing arbitrary well-ordered index sets. If `Γ` is ordered and `R` has zero, then `R⟦Γ⟧` consists of formal series over `Γ` with coefficients in `R`, whose supports are partially well-ordered. This includes the fundamental structure definition, addition and multiplication operations, summable families, power series connections, valuations, lexicographic ordering, binomial expansions, cardinality theory, and the Hahn embedding theorem for ordered abelian groups. These generalize Laurent series (which use `Γ = ℤ`) and provide a powerful framework for working with valued fields and ordered algebraic structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `HahnSeries Γ R` structure as functions with partially well-ordered support; defines support, single series, order, orderTop, map, and embDomain operations |
| Addition.lean | Additive structure on Hahn series: addition by coefficient-wise addition, scalar multiplication, additive monoid/group instances, and module structure |
| Multiplication.lean | Multiplicative structure: semiring and ring instances via convolution product, `HahnModule` type alias for avoiding instance diamonds, constant term homomorphism `C : R →+* R⟦Γ⟧`, embedding ring homomorphisms, and invertible series close to 1 |
| Summable.lean | Theory of formally summable families of Hahn series with well-ordered union of supports and finite co-support at each coefficient; formal sum operations `hsum` and `lsum`, pointwise scalar multiplication and product, power series, unit characterization theorem |
| PowerSeries.lean | Isomorphism `toPowerSeries : R⟦ℕ⟧ ≃+* PowerSeries R` showing Hahn series with `Γ = ℕ` are equivalent to formal power series; includes no-zero-divisors instances from multivariate power series |
| Lex.lean | Lexicographical ordering on Hahn series `Lex R⟦Γ⟧`; shows this is a linear order when `Γ` and `R` are linearly ordered; proves ordered group and ring instances, and finite Archimedean class decomposition |
| Valuation.lean | Additive valuation `addVal Γ R : AddValuation R⟦Γ⟧ (WithTop Γ)` on Hahn series over domains, mapping series to their minimal nonzero coefficient index (or ⊤ for zero) |
| Binomial.lean | Binomial expansions of powers of Hahn series using `embDomain`; defines `binomialFamily` for formal expansion of `x^r` as `(1 + (x-1))^r` when `x` is close to 1 |
| Cardinal.lean | Cardinality theory: defines `cardSupp` as the cardinality of support, establishes bounds for operations (addition, multiplication, scalar action), constructs bounded subgroups/subrings/subfields |
| HEval.lean | Power series evaluation in Hahn series: ring homomorphism `PowerSeries.heval` substituting the generating variable with a positive-order Hahn series, extending to formal infinite sums via summable families |
| HahnEmbedding.lean | Hahn embedding theorem: every linearly ordered abelian group embeds as ordered subgroup of `Lex ℝ⟦FiniteArchimedeanClass M⟧`, proven via divisible hull and rational module structure |

## Subdirectories

(No subdirectories)

## Search Tags

Hahn-series generalized-power-series Laurent-series valued-field well-ordered partial-well-ordered support orderTop valuation additive-valuation summable-family formal-sum convolution-product HahnModule power-series-isomorphism lexicographic-order Archimedean-class Hahn-embedding binomial-expansion cardinality-support embedding ring-homomorphism linear-order ordered-group
