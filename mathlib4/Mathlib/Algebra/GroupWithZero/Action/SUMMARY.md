---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/GroupWithZero/Action
generated: 2025-12-01T06:09:53Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 12
subdirs_count: 1
---

# Action

## Overview

The `Action/` directory develops the complete theory of group and monoid actions in the presence of zero elements, bridging the gap between pure group actions and module structures. It establishes the fundamental action typeclasses (`SMulZeroClass`, `SMulWithZero`, `MulActionWithZero`, `DistribSMul`, `DistribMulAction`, `MulDistribMulAction`) that preserve zero, addition, and multiplication; provides instances for all standard constructions (products, Pi types, opposites, units, homomorphism types); and develops the theory of homomorphisms, equivalences, and faithful actions that respect these zero-preserving structures. The `Pointwise/` subdirectory extends this theory to set and finset collections, characterizing how scalar multiplication interacts with set operations and when zero appears in scaled collections. Together, these components form the essential foundation for module theory, representation theory, linear algebra, and functional analysis.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core action typeclass definitions: `SMulZeroClass` (preserves right zero), `SMulWithZero` (preserves both zeros), `MulActionWithZero` (monoid action with zero), `DistribSMul` (distributes over addition), `DistribMulAction` (monoid action on additive monoid), `MulDistribMulAction` (multiplicative action on monoid), with pullback/pushforward constructions |
| Basic.lean | Basic theory: bijectivity/injectivity/surjectivity lemmas for group actions with zero, additive equivalences and automorphisms (`DistribMulAction.toAddEquiv`, `DistribMulAction.toAddAut`), `smulMonoidWithZeroHom`, and power laws (`smul_zpow₀'`) |
| Hom.lean | Scalar multiplication instances on morphism types: `SMulZeroClass`, `SMulWithZero`, `MulActionWithZero` on `ZeroHom A B`, and `DistribSMul`, `DistribMulAction` on `AddMonoidHom A B`, with compatibility for `SMulCommClass`, `IsScalarTower`, `IsCentralScalar` |
| Pi.lean | Product type instances: `SMulZeroClass`, `DistribSMul`, `DistribMulAction`, `SMulWithZero`, `MulActionWithZero`, `MulDistribMulAction` for Pi types `∀ i : I, f i`, with both dependent and non-dependent versions, plus `Pi.single_smul` lemmas |
| Prod.lean | Binary product instances: `SMulZeroClass`, `DistribSMul`, `DistribMulAction`, `MulDistribMulAction`, `SMulWithZero`, `MulActionWithZero` for `α × β`, with `DistribMulAction.prodOfSMulCommClass` construction and equivalence `DistribMulAction.prodEquiv` |
| Units.lean | Actions on and by units: `SMulZeroClass`, `DistribSMul`, `DistribMulAction`, `MulDistribMulAction` instances for `Mˣ`, inverse smul lemmas (`inv_smul_smul₀`, `smul_inv_smul₀`), `Equiv.smulRight` as order isomorphism, and `Units.mulDistribMulAction'` for actions of groups on units |
| Opposite.lean | Opposite type instances: `SMulZeroClass`, `SMulWithZero`, `MulActionWithZero`, `DistribMulAction`, `MulDistribMulAction` for actions on and by `Mᵐᵒᵖ`, with faithful action instance `CancelMonoidWithZero.toFaithfulSMul_opposite` |
| End.lean | Endomorphism and composition: `Function.Surjective.distribMulActionLeft`, `DistribMulAction.compHom`, `MulDistribMulAction.compHom`, `AddMonoid.End.applyDistribMulAction` instance, and `DistribMulAction.toAddEquiv₀` for group-with-zero actions |
| Center.lean | Center of groups with zero: `Subgroup.centerUnitsEquivUnitsCenter` establishing equivalence between the center of units and the units of the center in a group with zero |
| ConjAct.lean | Conjugation action: `ConjAct G₀` instance for `GroupWithZero`, with `mulAction₀` and `smulCommClass₀` instances for conjugation as a multiplicative action preserving zero |
| Faithful.lean | Faithful actions: `CancelMonoidWithZero.faithfulSMul` instance showing that nontrivial cancellative monoids with zero act faithfully on themselves |
| TransferInstance.lean | Instance transfer across equivalences: methods to transfer `SMulZeroClass`, `SMulWithZero`, `MulActionWithZero`, `DistribSMul`, `DistribMulAction` structures across `Equiv` preserving definitional equalities |

## Subdirectories

- [x] `Pointwise/` - Pointwise scalar multiplication on sets and finite sets in the context of groups with zero: typeclass instances for set/finset collections, zero behavior and membership characterizations, and nonzero scalar injectivity properties for set operations

## Search Tags

group-action scalar-multiplication zero-preservation distrib-mul-action mul-action-with-zero smul-zero-class smul-with-zero additive-action product-action pi-action opposite-action units-action faithful-action conjugation-action homomorphism-action pointwise-operations sets finite-sets module-foundations representation-theory linear-algebra functional-analysis
