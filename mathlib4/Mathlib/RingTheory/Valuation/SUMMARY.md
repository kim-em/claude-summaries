---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Valuation
generated: 2026-02-01T22:30:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: preliminary
files_count: 19
subdirs_count: 2
---

# Valuation

## Overview

The `Valuation/` directory contains comprehensive formalization of valuation theory on rings and fields. This includes the foundational definition of valuations as monoid homomorphisms to linearly ordered monoids satisfying the ultrametric inequality; valuation rings (domains where divisibility is total); valuation subrings of fields (maximal local subrings); rings of integers under valuations (elements with valuation ≤ 1); rank one valuations with codomain embeddable in ℝ≥0; discrete valuations; extensions of valuations to algebra extensions; quotient valuations; ramification groups; and connections to integral closedness and local ring theory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `Valuation R Γ₀` as monoid homomorphism with ultrametric inequality `v(x+y) ≤ max(v x, v y)`; valuation class; support ideals; equivalence relation on valuations; additive valuations |
| ValuationRing.lean | Valuation rings (domains where for all a,b either a divides b or b divides a); proves equivalence with local Bézout domains; natural valuation on fraction field; TFAE characterization |
| ValuationSubring.lean | Valuation subrings of fields (subrings A where ∀x, x∈A or x⁻¹∈A); maximal in domination order of local subrings |
| LocalSubring.lean | Equivalence between valuation subrings and maximal local subrings; integral closedness of valuation subrings; domination order theory |
| Integers.lean | Ring of integers under a valuation (subring of elements with v(x) ≤ 1); characteristic predicates for algebras being valuation integers |
| RankOne.lean | Rank one valuations (nontrivial valuations with codomain embeddable in ℝ≥0); multiplicative archimedean property characterization |
| Extension.lean | Extension of valuations to algebra extensions; `HasExtension vR vA` typeclass for when restriction equals (is equivalent to) base valuation; flexibility for normalization choices |
| Quotient.lean | Quotient valuations: given v on R and ideal J ⊆ supp(v), construct induced valuation on R/J |
| RamificationGroup.lean | Ramification groups for valued field extensions |
| AlgebraInstances.lean | Algebra structure instances for valuation-related constructions |
| Archimedean.lean | Ring of integers under valuations in multiplicatively archimedean codomains; linear order instances on monoid ranges |
| DiscreteValuativeRel.lean | Discrete valuative relations (maximal element < 1 in value group); equivalence with ℤᵐ⁰ in rank-one case |
| ExtendToLocalization.lean | Extending valuations to localizations |
| FiniteField.lean | Valuation theory specific to finite fields |
| Integral.lean | Integral elements and integrality conditions for valuations |
| IntegrallyClosed.lean | Integral closedness properties for valuation rings |
| Minpoly.lean | Minimal polynomials in the context of valuations |
| PrimeMultiplicity.lean | Prime multiplicity theory for valuations |
| ValuativeRel.lean | Import file for valuative relation theory |

## Subdirectories

- [ ] `Discrete/` - Discrete valuation theory
- [ ] `ValuativeRel/` - Valuative relations (generalization of valuations)

## Search Tags

valuation non-archimedean-norm ultrametric valuation-ring valuation-subring local-ring domination integers rank-one discrete-valuation extension quotient-valuation ramification-group support-ideal equivalence multiplicative additive ordered-monoid linearly-ordered fraction-field Bezout-domain maximal-local-subring integrally-closed archimedean finite-field
