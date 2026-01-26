---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/SuccPred
generated: 2026-01-26T09:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 11
subdirs_count: 0
---

# SuccPred

## Overview

The `SuccPred/` directory formalizes successor and predecessor operations on ordered types. It defines `SuccOrder` (orders with a sensible successor function `succ a` giving the least element greater than `a`) and `PredOrder` (orders with a predecessor function `pred a` giving the greatest element less than `a`). The directory includes archimedean variants where iterating `succ`/`pred` reaches all comparable elements, limit theory distinguishing elements that don't cover others (successor/predecessor limits), connections to linear locally finite orders showing they are countable and order-isomorphic to subsets of ℤ, relations with suprema/infima in complete linear orders, interval decompositions, closure properties for relations, compatibility with initial segment embeddings, rooted tree applications, and extensions to `WithBot`/`WithTop` types.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `SuccOrder` (with `succ : α → α`, `le_succ`, `max_of_succ_le`, `succ_le_of_lt`) and `PredOrder` (with `pred : α → α`, `pred_le`, `min_of_le_pred`, `le_pred_of_lt`); constructors for no-max/no-min cases; OrderDual instances; covering relation `a ⋖ succ a`; extensive API for successor/predecessor arithmetic |
| Archimedean.lean | Archimedean successor/predecessor orders: `IsSuccArchimedean` (can reach any `b ≥ a` by iterating `succ` from `a`), `IsPredArchimedean` (dual for `pred`); induction principles for succ-archimedean orders; density results |
| Limit.lean | Successor and predecessor limits: `IsSuccPrelimit a` (no element covers `a`, so `a` can't be anyone's successor), `IsPredPrelimit` (dual), `IsSuccLimit` (non-minimal successor prelimit), `IsPredLimit` (non-maximal predecessor prelimit); characterizations in various order contexts |
| LinearLocallyFinite.lean | Linear locally finite orders have successor/predecessor structure: proves `LinearLocallyFiniteOrder` implies `SuccOrder`, `PredOrder`, `IsSuccArchimedean`, `IsPredArchimedean`, and `Countable`; defines `toZ i0 i` assigning integers to elements while respecting order; proves `orderIsoRangeToZOfLinearSuccPredArch`, `orderIsoNatOfLinearSuccPredArch`, `orderIsoIntOfLinearSuccPredArch` establishing order isomorphisms with ℤ, ℕ, or finite ranges depending on boundedness |
| CompleteLinearOrder.lean | Relations between successor/predecessor limits and suprema/infima in conditionally complete linear orders: `csSup_mem_of_not_isSuccPrelimit` (if supremum is not a successor prelimit, it's in the set), `csInf_mem_of_not_isPredPrelimit` (dual), variants for indexed suprema `ciSup`/infima `ciInf`, and for `IsLUB`/`IsGLB` |
| IntervalSucc.lean | Interval decompositions using successor: `Monotone.biUnion_Ico_Ioc_map_succ` (union of `Ioc (f i) (f (succ i))` equals `Ioc (f m) (f n)` for monotone `f` in archimedean succ orders), `Monotone.pairwise_disjoint_on_Ioc_succ` (intervals `Ioc (f n) (f (succ n))` are pairwise disjoint), dual versions for predecessor |
| Relation.lean | Properties of relations on types with `SuccOrder`/`PredOrder`: `reflTransGen_of_succ_of_le` (if `r i (succ i)` for all `i` in `[n,m)`, then `(n,m)` in reflexive-transitive closure of `r`), `transGen_of_succ_of_lt` (transitive closure version), duals for predecessor, versions for linear orders with bidirectional conditions |
| InitialSeg.lean | Initial segment embeddings preserve successor/predecessor structure: `InitialSeg.map_succ` (initial segment maps preserve `succ`), `InitialSeg.map_pred` (preserve `pred`), `apply_covBy_apply_iff` (preserve covering relation), `isSuccLimit_apply_iff` (preserve successor limit property), analogous results for `PrincipalSeg` |
| Tree.lean | Rooted tree theory using predecessor structure: assumes `PartialOrder`, `PredOrder`, `IsPredArchimedean`, `OrderBot` (root); defines `findAtom r` (unique atom below element `r` in tree), proves `isAtom_findAtom`, `pred_findAtom`, characterizes when `findAtom r = ⊥` |
| WithBot.lean | Successor on `WithBot α`: defines `WithBot.succ` mapping `⊥ ↦ ⊥` and `(a : α) ↦ Order.succ a`, proves monotonicity `succ_mono`, strict monotonicity under `NoMaxOrder`, `lt_succ`, characterizes `succ_eq_bot`; dual results for `WithTop.pred` |

## Subdirectories

(none)

## Search Tags

successor predecessor succ-order pred-order archimedean covering-relation limit successor-limit predecessor-limit linear-locally-finite countable order-isomorphism toZ initial-segment principal-segment reflexive-transitive-closure interval-decomposition rooted-tree WithBot WithTop
