---
source_path: /Users/kim/projects/lean/lean4-2/downstream_releases/mathlib4/Mathlib/Data/Finsupp/MonomialOrder
generated: 2025-12-09T08:45:00Z
git_sha: 8630639169c28647dbae9f5b0132c77dcbfe2281
git_branch: bump_to_v4.26.0-rc2
status: complete
files_count: 1
subdirs_count: 0
---

# MonomialOrder

## Overview

The `MonomialOrder/` subdirectory contains implementations of specific monomial orderings for Gröbner basis theory. While the parent `MonomialOrder.lean` defines the general framework for monomial orders (well-founded orderings on `σ →₀ ℕ` compatible with addition) and provides a basic lexicographic example, this subdirectory provides the degree-lexicographic (graded lexicographic) ordering, which first compares total degrees and then uses lexicographic ordering as a tiebreaker.

## Key Files

| File | Purpose |
|------|---------|
| DegLex.lean | Homogeneous lexicographic monomial ordering: defines `DegLex (σ →₀ ℕ)` type synonym and `MonomialOrder.degLex`, which compares by total degree first, then lexicographically; includes well-foundedness proofs and examples showing `X₁ < X₀` and `X₀·X₁ < X₀²` |

## Subdirectories

None

## Search Tags

monomial-order deg-lex degree-lexicographic graded-lexicographic grobner-basis polynomial-ordering finsupp well-founded type-synonym linear-order
