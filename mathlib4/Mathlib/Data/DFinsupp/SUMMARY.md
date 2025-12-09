---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/DFinsupp
generated: 2025-12-09T04:30:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 16
subdirs_count: 0
---

# DFinsupp

## Overview

This directory implements dependent functions with finite support, denoted `Π₀ i, β i`, which are the dependent-typed version of `Finsupp`. Unlike `Finsupp α β` (functions `α →₀ β`), `DFinsupp` allows the codomain type to vary based on the input (`β : ι → Type v`). The core structure pairs a function with a proof-irrelevant multiset representing a superset of the support, enabling computationally efficient operations (particularly addition) without requiring decidability of zero equality. The directory provides algebraic instances (additive structures, modules, scalar multiplication), order structures (pointwise and lexicographic), and numerous utility functions including big operators (sum/prod), well-foundedness results, and equivalences with related types (multisets, sigma types).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `DFinsupp` structure with notation `Π₀ i, β i`; basic operations including `mapRange`, `zipWith`, `single`, `update`, `erase`; additive group instances; computational support via `support'` (multiset superset) and `support` (actual finset requiring decidability) |
| BigOperators.lean | Big operator support for `DFinsupp`: defines `prod` and `sum` operations over the support; provides `sumAddHom` (sum using additive homomorphisms without recomputing support) and `finset_sum` compatibility lemmas |
| Module.lean | Scalar multiplication and module structure on `DFinsupp`: `SMulZeroClass`, `DistribMulAction`, and `Module` instances via pointwise operations; includes `coeFnLinearMap` for coercion to pi types as linear maps |
| Order.lean | Pointwise order structures: `LE`, `LT`, `Preorder`, `PartialOrder` instances via pointwise comparison; `orderEmbeddingToFun` embedding `DFinsupp` into function space |
| Lex.lean | Lexicographic order on `DFinsupp`: defines `DFinsupp.Lex r s` for ordering by first differing coordinate; provides `Lex (Π₀ i, α i)` and `Colex (Π₀ i, α i)` type synonyms with appropriate order instances |
| WellFounded.lean | Well-foundedness of lexicographic and product orders on `DFinsupp`: proves `DFinsupp.Lex.wellFounded` (lexicographic order well-founded when index order is well-order and coordinate orders are well-founded with bottom elements); derives product order well-foundedness by choosing appropriate well-orders |
| Notation.lean | Extends `fun₀ \| 3 => a \| 7 => b` notation to work for `DFinsupp` (desugars to `DFinsupp.update` and `DFinsupp.single`); provides custom `Repr` instance displaying functions using `fun₀` syntax |
| NeLocus.lean | Defines `neLocus f g : Finset α` as the finite set where two `DFinsupp`s differ; generalizes support of difference to situations without subtraction; includes membership characterizations and relationship to equality |
| Interval.lean | Finite intervals for `LocallyFiniteOrder` instance on `DFinsupp`: defines `Finset.dfinsupp` for finitely supported products of finsets; proves cardinality formulas and provides `Icc`, `Ico`, `Ioc`, `Ioo` interval constructions |
| Ext.lean | Extensionality principles for additive homomorphisms from `DFinsupp`: proves `addHom_ext` (two additive homomorphisms equal if they agree on all `single i x` elements); shows `⋃ i, range (single i)` generates `DFinsupp` under addition |
| Sigma.lean | Conversions between `Π₀ (i : Σ j, α j), δ i.1 i.2` and `Π₀ i (j : α i), δ i j`: defines `sigmaCurry` and `sigmaUncurry` with `sigmaCurryEquiv` bundling them as a bijection; includes additive and linear equivalence versions |
| Multiset.lean | Equivalence between `Π₀ _ : α, ℕ` and `Multiset α`: defines `toMultiset` (sum using `Multiset.replicate`) and `toDFinsupp` (using `Multiset.count`); proves these are inverse additive homomorphisms |
| Encodable.lean | Provides `Encodable (Π₀ i, α i)` instance (when `ι` and all `α i` are encodable and have decidable non-zero) via `sigmaFinsetFunEquiv`; provides `Countable` instance for countable index and codomain types |
| FiniteInfinite.lean | Finiteness properties: `fintype` instance when domain and all codomains are finite (via equivalence with pi types); `infinite_of_left` when domain is infinite; `infinite_of_exists_right` when any codomain is infinite |
| Small.lean | Universe level smallness: provides `Small.{w}` instance on `DFinsupp π` when `ι` and all `π i` are `w`-small; application to `Finsupp` via `finsuppEquivDFinsupp` |
| Submonoid.lean | Interaction with submonoids: proves `dfinsuppProd_mem` and `dfinsuppSumAddHom_mem` for membership preservation; characterizes `iSup` of additive submonoids as range of `sumAddHom` (`mem_iSup_iff_exists_dfinsupp`) |

## Subdirectories

*None*

## Search Tags

dfinsupp dependent-functions finite-support dependent-types notation big-operators module-structure order lexicographic-order well-founded multiset encodable countable sigma-types submonoids algebraic-structures
