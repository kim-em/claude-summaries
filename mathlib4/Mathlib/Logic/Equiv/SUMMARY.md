---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic/Equiv
generated: 2026-01-25T23:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: nightly-testing
status: complete
files_count: 17
subdirs_count: 1
---

# Equiv

## Overview

The `Equiv/` directory contains the comprehensive theory of type equivalences (bijections) in mathlib4. At its core are `Equiv α β` (notation `α ≃ β`), representing bundled bijections with explicit inverses, and `PartialEquiv`, representing bijections between subsets (used primarily for manifold charts). The directory provides foundational definitions (`Defs.lean`), extensive lemmas and constructions (`Basic.lean`), and specialized equivalences for standard type constructors: products, sums, options, lists, multisets, finsets, arrays, and finite types. Key functionality includes equivalence composition/inversion, transferring instances along equivalences, permutations (`Equiv.Perm`), and connections to embeddings and functors. The `Fin/` subdirectory provides critical building blocks for working with finite indexed types, including canonical conversions between `Fin n` and option/sum types, product/sum decomposition equivalences, and cyclic rotation operations that are fundamental to finite permutation theory.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Equiv α β` structure (bundled bijection with `toFun`, `invFun`, `left_inv`, `right_inv` proofs); `Equiv.Perm α` permutation abbreviation; `EquivLike` typeclass; basic operations (refl, symm, trans); instance transfer functions (inhabited, unique, decidableEq); imports tactics (simps, substs) and foundational types (FunLike, Quot, Subtype, Unique); 913 lines |
| Basic.lean | Extensive library of equivalence constructions and lemmas building on `Defs.lean`; includes pi/option/sigma equivalences, subtype operations (`subtypeCongr`, `Perm.subtypeCongr`), quotient type equivalences, ulift/plift handling, and many specialized bijections; imports Option, Sum, Function.Conjugate, Lift, Int.Notation; 1075 lines of advanced equivalence theory |
| PartialEquiv.lean | Partial equivalences between subsets of types; `PartialEquiv α β` has `toFun`/`invFun` inverse on `source`/`target` subsets only; designed for manifold charts where functions are only locally bijective; includes composition (`trans`), symmetry, reflection, `ofSet` identity on subset, `EqOnSource` equivalence relation; implements `mfld_set_tac` tactic for domain manipulation; 991 lines |
| Set.lean | Equivalences involving sets; `Equiv.ofInjective` (injective function noncomputably equivalent to range), `Equiv.setCongr` (equal sets equivalent as types), `Equiv.Set.union` (disjoint union equivalent to `Sum`); lemmas for image/preimage under equivalences, subset relations, range properties; separated from Basic to avoid requiring full lattice structure on sets early; 653 lines |
| Prod.lean | Product type equivalences; `Equiv.prodCongr` combines two equivalences using `Prod.map` (`ea : α₁ ≃ α₂` and `eb : β₁ ≃ β₂` yields `α₁ × β₁ ≃ α₂ × β₂`); `pprodEquivProd` (`PProd α β ≃ α × β`); `pprodCongr` for PProd; 529 lines |
| Sum.lean | Sum type equivalences; `Equiv.sumEquivSigmaBool` (canonical equivalence `α ⊕ β ≃ Σ b, bif b then β else α`); `Equiv.prodSumDistrib` (distributive law `α × (β ⊕ γ) ≃ (α × β) ⊕ (α × γ)`); sum congruence and various canonical isomorphisms for sums; 364 lines |
| Option.lean | Option type equivalences; `Equiv.optionCongr` (universe-polymorphic version of `EquivFunctor.mapEquiv Option e`); `Equiv.removeNone` (construct `α ≃ β` from `Option α ≃ Option β` by removing none); option-specific lemmas and transformations; 286 lines |
| List.lean | List equivalences using encodability; `Equiv.listEquivOfEquiv` (lift `α ≃ β` to `List α ≃ List β` via mapping); `Encodable.encodeList`/`decodeList` for constructive encoding/decoding of lists; uses pairing function on ℕ for encodability proofs; 190 lines |
| Multiset.lean | Multiset equivalences; lifts equivalences from underlying types to multisets; connections to encodable multisets; 116 lines |
| Finset.lean | Finset equivalences; lifts equivalences to finite sets; connections between finsets and their underlying types; 123 lines |
| Fintype.lean | Equivalences involving finite types; `Function.Embedding.toEquivRange` (computably turn fintype embedding into equiv to its range, using exhaustive search); `Equiv.Perm.viaFintypeEmbedding` (extend permutation domain via embedding, fixing outside range); note: computable but poor performance; 137 lines |
| Array.lean | Array equivalences; lifts equivalences from element types to arrays; 55 lines |
| Bool.lean | Bool-specific equivalences; canonical bijections involving boolean types; 37 lines |
| Nat.lean | Nat-specific equivalences; canonical bijections involving natural numbers; 61 lines |
| Embedding.lean | Equivalences on embedding types; `Equiv.sumEmbeddingEquivProdEmbeddingDisjoint` (embeddings from sum type equivalent to pairs of embeddings with disjoint ranges); constructs larger embeddings from smaller ones; 96 lines |
| Functor.lean | Equivalences for functors; lifts equivalences through functor applications; `EquivFunctor` machinery; 89 lines |
| Pairwise.lean | Equivalences preserving pairwise relations; connections between equivalences and pairwise properties; 25 lines |

## Subdirectories

- [x] `Fin/` - Equivalences involving `Fin n` (finite types with n elements)

## Search Tags

equivalence bijection type-equivalence equiv permutation partial-equiv manifold-charts isomorphism inverse product-equiv sum-equiv option-equiv list-equiv fintype embedding functor subtype quotient-type lean4 mathlib
