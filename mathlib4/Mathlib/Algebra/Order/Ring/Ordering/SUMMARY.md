---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Ring/Ordering
generated: 2025-12-01T19:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Ordering

## Overview

The `Ordering/` directory develops the theory of ring orderings and preorderings in the classical sense of real algebra (following Lam 1984). A **preordering** on a commutative ring is a subsemiring containing all squares but not `-1`, intuitively capturing "non-negative" elements. An **ordering** is a preordering that is total (contains either `x` or `-x` for all `x`) and whose support (elements with both `x` and `-x` in the preordering) forms a prime ideal. This algebraic structure underlies the connection between ordered rings and quotient constructions: an ordering with support `p` induces a linear order on `R⧸p` making it an ordered ring.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `RingPreordering` structure (subsemiring with squares and without `-1`), `supportAddSubgroup` (elements with both `x` and `-x` in preordering), `HasIdealSupport` typeclass (support closed under multiplication), `support` ideal, and `IsOrdering` class (preordering that is total with prime support) |
| Basic.lean | Fundamental properties: subsemiring ordering lemmas (`toSubsemiring_le_toSubsemiring`), closure under unit inverses (`unitsInv_mem`, `inv_mem` for fields), sums of squares membership (`mem_of_isSumSq`), minimal constructor `mk'`, support non-triviality (`support_ne_top`, `one_notMem_support`), field support characterization (`support_eq_bot`), characteristic 2 support ideal (`hasIdealSupport_of_isUnit_two`), and ordering characterization via negated products (`isOrdering_iff`) |

## Subdirectories

*(none)*

## Search Tags

ring-ordering preordering ring-preordering support-ideal prime-ideal ordered-ring-quotient sums-of-squares field-ordering total-ordering lam-real-algebra subsemiring non-negative-elements characteristic-two
