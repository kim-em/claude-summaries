---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/MonoidLocalization
generated: 2026-01-24T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# MonoidLocalization

## Overview

The `MonoidLocalization/` directory provides a comprehensive formalization of localization for commutative monoids, generalizing the classical construction from ring theory by removing dependence on addition. The core theory characterizes localizations up to isomorphism via a universal property (elements of submonoid become units, surjectivity, and equality conditions), defines the localization as a quotient type via congruence relations, and provides the fundamental `mk'` construction and `lift` universal homomorphism. Specialized topics include localization away from a single element (Away maps), the Grothendieck group construction (localization at the top submonoid making all elements invertible), ordered structures on localizations, monoids with zero (handling triviality when zero is inverted), cardinality bounds, finiteness preservation, and submonoid characterizations via division pairs.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core localization theory: characteristic predicate (IsLocalizationMap), LocalizationMap structure, quotient construction via congruence relations, universal properties (mk', lift, map), equivalence of congruence and standard localization relations |
| Away.lean | Localization away from a single element: AwayMap type abbreviation for localization at powers of x, invSelf construction (inverse of x), lift for away maps, awayToAwayRight composition |
| GrothendieckGroup.lean | Grothendieck group construction as localization at top submonoid: inclusion map (of), inverse operation, group structure, lift equivalence between monoid homs M → G and group homs GrothendieckGroup M → G |
| Order.lean | Ordered structures on localizations: LE/LT instances for ordered cancel monoids, PartialOrder and LinearOrder instances, IsOrderedCancelMonoid instance, mkOrderEmbedding order embedding |
| MonoidWithZero.lean | Localization of monoids with zero: triviality when 0 ∈ S, CommMonoidWithZero instance, lift₀ for MonoidWithZero homomorphisms, zero-specific properties |
| Cardinality.lean | Cardinality bounds: #(Localization S) ≤ #M via delegation to Ore localization |
| Finite.lean | Finiteness preservation: localization of finitely generated monoid at finitely generated submonoid is finitely generated, Grothendieck group of FG monoid is FG |
| Lemmas.lean | Additional lemmas requiring extra imports: surj_pi_of_finite for product types, pi instance for localization of products |
| DivPairs.lean | Submonoid of pairs with quotient in a submonoid: divPairs construction for pairs (a,b) where f(a)/f(b) ∈ s, used in Grothendieck group theory |

## Subdirectories

*(none)*

## Search Tags

monoid-localization commutative-monoid localization quotient-monoid congruence-relation characteristic-predicate universal-property grothendieck-group away-map ordered-monoid monoid-with-zero cardinality finiteness div-pairs localization-map mk lift
