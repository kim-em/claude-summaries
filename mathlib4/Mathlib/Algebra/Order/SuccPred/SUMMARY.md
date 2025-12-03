---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/SuccPred
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# SuccPred

## Overview

The `SuccPred/` subdirectory provides specialized results for successor and predecessor functions in ordered algebraic structures. It covers successor/predecessor behavior in `SuccAddOrder` structures (where successor relates to addition by one), type tags (`Multiplicative` and `Additive` wrappers preserving successor/predecessor structures), and `WithBot` types (adding a bottom element with algebraic successor properties). These files extend the core successor/predecessor theory from `Order/SuccPred` with algebraic compatibility.

## Key Files

| File | Purpose |
|------|---------|
| PartialSups.lean | Partial suprema in `SuccAddOrder`: lemmas for `partialSups f (i + 1)` and `partialSups f (Order.succ i)` decompositions in linearly ordered types with successor structure |
| TypeTags.lean | Successor/predecessor instances for type tags: proves `Multiplicative` and `Additive` inherit `SuccOrder`, `PredOrder`, `IsSuccArchimedean`, and `IsPredArchimedean` from underlying type |
| WithBot.lean | Algebraic successor properties for `WithBot`: natural number coercions (`succ (n : WithBot α) = n + 1`), special cases for 0/1, and characterization `1 ≤ a ↔ 0 < a` |

## Subdirectories

*(none)*

## Search Tags

successor-order predecessor-order succ-add-order partial-sups type-tags multiplicative additive with-bot algebraic-successor
