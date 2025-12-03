---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Group
generated: 2025-12-01T20:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 30
subdirs_count: 4
---

# Group

## Overview

The `Group/` directory provides comprehensive theory for ordered groups, covering both bundled definitions (where order is part of the group structure) and unbundled typeclasses (where monotonicity properties are separate). The directory spans fundamental operations (absolute value, Jordan decomposition, integer powers), structural tools (positive cone constructions, order isomorphisms), specialized results (densely ordered groups are not cyclic, sharp bounds for integer sums), and pointwise operations on sets. It includes both the abstract algebraic framework and concrete instances for working with ordered groups in lattice contexts, group actions preserving order, and interval arithmetic. The theory applies to both general ordered groups and specialized cases like integers and linearly ordered groups.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Bundled ordered group definitions, conversion between `IsOrderedMonoid` and `IsOrderedCancelMonoid` for commutative groups, linear ordered group lemmas |
| Basic.lean | Integer power (`zpow`) operations in ordered groups: monotonicity, strict monotonicity, injectivity, and the proof that nontrivial densely ordered groups are not cyclic |
| Abs.lean | Absolute value theory in ordered groups: `\|a\|ₘ = max a a⁻¹`, properties of `\|a / b\|ₘ`, triangle inequalities, and absolute value equations |
| PosPart.lean | Positive and negative parts in lattice ordered groups: Jordan decomposition `a = a⁺ - a⁻`, coprimes property `a⁺ ⊓ a⁻ = 0` |
| Cone.lean | Construct ordered groups from positive cones: `GroupCone` structure encoding axioms in terms of nonnegative elements, conversion between cones and ordered groups |
| Indicator.lean | Support of functions in ordered contexts: `mulSupport` interaction with lattice operations (sup, inf, max, min) |
| DenselyOrdered.lean | Lemmas about densely linearly ordered groups: characterization via multiplicative epsilon arguments |
| OrderIso.lean | Inverse and multiplication as order isomorphisms: `x ↦ x⁻¹` as order-reversing equivalence, multiplication as order isomorphism |
| Synonym.lean | Group structures on order type synonyms: transfer algebraic instances to `αᵒᵈ`, `Lex α`, `Colex α` |
| Bounds.lean | Bounds in ordered groups |
| CompleteLattice.lean | Complete lattice structures on ordered groups |
| Cyclic.lean | Cyclic ordered groups |
| End.lean | Endomorphisms of ordered groups |
| Equiv.lean | Equivalences preserving ordered group structure |
| Finset.lean | Finset operations in ordered groups |
| Ideal.lean | Ideals in ordered groups |
| InjSurj.lean | Injective and surjective functions in ordered groups |
| Instances.lean | Type class instances for ordered groups |
| Lattice.lean | Lattice operations in ordered groups |
| MinMax.lean | Min/max operations in ordered groups |
| Multiset.lean | Multiset operations in ordered groups |
| Nat.lean | Natural number operations in ordered groups |
| Opposite.lean | Opposite groups with order |
| PartialSups.lean | Partial suprema in ordered groups |
| PiLex.lean | Lexicographic order on Pi types with group structure |
| Prod.lean | Product groups with order |
| TypeTags.lean | Type tags for ordered groups |
| Units.lean | Units in ordered groups |
| Action.lean | Group actions preserving order (entry point) |
| Int.lean | Integer-specific ordered group theory (entry point) |

## Subdirectories

- [x] `Action/` - Group actions preserving order: tautological actions by relation isomorphisms, order isomorphism actions on flags (maximal chains), and transfer of actions to order type synonyms (`αᵒᵈ`, `Lex α`)
- [x] `Int/` - Sharp bounds for sums of bounded finsets of integers: exploit distinctness to get tighter bounds than naive cardinality multiplication (e.g., `sum_le_sum_Ioc`, `sum_Ico_le_sum`)
- [x] `Pointwise/` - Pointwise operations on sets in ordered monoids/groups: bounds preservation under multiplication, suprema/infima of products (`sSup (s * t) = sSup s * sSup t`), and comprehensive interval preimage/image lemmas
- [x] `Unbundled/` - Unbundled (typeclass-based) ordered group theory with fine-grained monotonicity control: `MulLeftMono`, `MulRightMono`, absolute value as `a ⊔ a⁻¹`, Birkhoff inequalities, integer-specific results

## Search Tags

ordered-groups ordered-commutative-groups linear-ordered-groups absolute-value mabs jordan-decomposition positive-part negative-part positive-cone group-cone zpow-monotonicity densely-ordered cyclic-groups order-isomorphism group-actions lattice-ordered-groups multiset-operations finset-operations unbundled-ordered-groups mul-left-mono mul-right-mono triangle-inequality solid-sets birkhoff-inequalities pointwise-operations bounded-sets supremum infimum interval-arithmetic preimage-image affine-transformations integer-sums sharp-bounds distinct-integers flags maximal-chains order-dual lexicographic-order faithful-action tautological-action relation-isomorphism typeclass-based-order covariance contravariance
