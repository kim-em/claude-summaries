---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Equiv
generated: 2025-12-01T22:10:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# Equiv

## Overview

The `Equiv/` directory defines multiplicative and additive equivalences (`MulEquiv` and `AddEquiv`), which are the group-theoretic notion of isomorphism - type equivalences that preserve the algebraic structure. These bundled equivalences extend base type equivalences (`Equiv`) with multiplication/addition preservation axioms, forming the foundation for group, monoid, and semigroup isomorphisms throughout mathlib4. The directory provides the core typeclass definitions, comprehensive API for working with these isomorphisms (including composition, inversion, and lifting), and specialized constructions for opposite groups, type tags (Multiplicative/Additive), and finite types.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of `MulEquiv` (notation `≃*`) and `AddEquiv` (notation `≃+`); defines bundled equivalences as structure combining `Equiv` with homomorphism, `MulEquivClass`/`AddEquivClass` typeclasses; includes basic operations (identity `refl`, inverse `symm`, composition `trans`), coercions to functions and homomorphisms, and fundamental lemmas about bijectivity, identity/inverse preservation, and extensionality |
| Basic.lean | Extended API for multiplicative/additive equivalences requiring more imports; provides `ofUnique` for types with unique elements, `arrowCongr` for function type equivalences, `monoidHomCongrLeft`/`monoidHomCongrRight` for induced equivalences on homomorphism spaces, `piCongrRight` for dependent products, `piUnique` for singleton-indexed families, and `Equiv.inv` establishing that inversion is a permutation on types with involutive inversion |
| TypeTags.lean | Conversions between multiplicative and additive equivalences via type tags `Multiplicative` and `Additive`; provides `AddEquiv.toMultiplicative`/`MulEquiv.toAdditive` translating between `≃+` and `≃*`, specialized versions for partially-tagged types (`toMultiplicativeLeft`, `toMultiplicativeRight`), and canonical isomorphisms like `Multiplicative (Additive G) ≃* G`; includes endomorphism conversions (`monoidEndToAdditive`) and product/pi type conversions (`prodMultiplicative`, `piMultiplicative`, `funMultiplicative`) |
| Opposite.lean | Equivalences and homomorphisms for opposite groups (multiplication order reversal); defines `MulOpposite.opAddEquiv` and `AddOpposite.opMulEquiv` as equivalences to opposite types, `MulEquiv.inv'` establishing `G ≃* Gᵐᵒᵖ` via inversion, homomorphism transport to/from opposite (`toOpposite`, `fromOpposite`), and the `op`/`unop` functorial action on homomorphisms (`MulHom.op`, `MonoidHom.op`, `MulEquiv.op`) showing that opposite is a fully faithful functor |
| Finite.lean | Decidability instances for equivalences on finite types; provides `decidableEqMulEquivFintype` and `decidableEqAddEquivFintype` showing that equality of multiplicative/additive equivalences is decidable when the codomain has decidable equality and domain is finite (by reduction to function equality via `DFunLike.coe_injective`) |

## Subdirectories

*No subdirectories*

## Search Tags

mul-equiv add-equiv group-isomorphism monoid-isomorphism equivalence ≃* ≃+ group-theory isomorphism bijection automorphism opposite mul-opposite add-opposite multiplicative additive type-tags fintype decidable-eq arrow-congr pi-congr homomorphism-space monoid-hom-congr to-additive
