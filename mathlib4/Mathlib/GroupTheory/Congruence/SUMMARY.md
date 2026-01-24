---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Congruence
generated: 2026-01-24T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Congruence

## Overview

The `Congruence/` directory formalizes congruence relations on algebraic structures (monoids and groups). A congruence relation is an equivalence relation that preserves the binary operation (multiplication or addition). The directory provides the core definitions, basic properties, homomorphism interactions, quotient constructions, and the isomorphism theorems for monoids and groups. Key functionality includes defining congruence relations as structures extending setoids, constructing quotient structures that inherit algebraic properties, lifting homomorphisms through quotients, and establishing correspondences between congruence relations and kernels of homomorphisms.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of Con and AddCon structures, inductive definition of smallest congruence (conGen/addConGen), basic properties (refl/symm/trans/mul), quotient construction, complete lattice structure, coercion to Quotient type, and basic group/monoid instances on quotients |
| Hom.lean | Homomorphism interactions: kernel as congruence (Con.ker), natural quotient map (Con.mk'), universal property (Con.lift), homomorphism lifting and uniqueness, congruence mapping (Con.map), and order-preserving correspondence between congruences containing c and congruences on c.Quotient |
| Basic.lean | Advanced quotient properties: product congruences, pi-type congruences, quotient isomorphisms (Con.congr), comap properties for equivalences, submonoid perspective, isomorphism theorems (quotientKerEquivRange, quotientKerEquivOfSurjective, comapQuotientEquiv, quotientQuotientEquivQuotient), scalar multiplication actions on quotients |
| BigOperators.lean | Preservation of big operators: proves that congruence relations preserve list products (list_prod), multiset products (multiset_prod), and finset products (finset_prod), along with their additive variants |
| Opposite.lean | Opposite group/monoid congruences: defines Con.op (congruence on Mᵐᵒᵖ from congruence on M), Con.unop (reverse direction), and orderIsoOp establishing order isomorphism between Con M and Con Mᵐᵒᵖ |

## Subdirectories

(None)

## Search Tags

congruence-relation equivalence-relation quotient monoid group kernel homomorphism lift universal-property isomorphism-theorem quotient-map setoid multiplicative additive big-operators opposite
