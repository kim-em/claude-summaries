---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/TwoSidedIdeal
generated: 2026-02-01T22:50:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 6
subdirs_count: 0
---

# TwoSidedIdeal

## Overview

The `TwoSidedIdeal/` directory formalizes two-sided ideals in non-commutative rings as equivalence classes under ring congruences. Unlike one-sided ideals (which absorb multiplication on only one side), two-sided ideals absorb multiplication from both left and right, making them the natural generalization of ideals from commutative algebra. The directory establishes the complete lattice structure on two-sided ideals, operations like span/map/comap, and the relationship between two-sided ideals and ordinary left ideals in commutative rings.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `TwoSidedIdeal R` as a wrapper around `RingCon R`; SetLike instance interpreting membership as `I.ringCon x 0`; order embedding to sets; AddCommGroup structure; operations (add/neg/mul absorption); opposite ideal constructions (op/unop); set-theoretic constructor `mk'` |
| Lattice.lean | Complete lattice structure on two-sided ideals with sup (ideal sum), inf (ideal intersection), sSup/sInf (arbitrary joins/meets), top (whole ring), bot (zero ideal); membership characterizations for lattice operations; `one_mem_iff` relating unit membership to maximality |
| Operations.lean | Span construction (smallest two-sided ideal containing a set); map (pushforward under ring homomorphism) and comap (pullback); characterizations of span membership via additive subgroup closure; Galois connection between left ideals and two-sided ideals (`fromIdeal` ⊣ `asIdeal`); order isomorphism with left ideals in commutative rings; module structures over R and Rᵐᵒᵖ |
| Kernel.lean | Kernel of a ring homomorphism as a two-sided ideal; `ker f = ⊥ ↔ injective f`; proof that `ker (ringCon.mk')` recovers the original ideal |
| BigOperators.lean | Interaction with sums and products: list/multiset/finset sum membership (if all summands in ideal, sum is in ideal); product membership (if any factor in ideal, product is in ideal for rings/commutative rings) |
| Instances.lean | NonUnitalSubringClass instance showing two-sided ideals are non-unital subrings |

## Subdirectories

(none)

## Search Tags

two-sided-ideal non-commutative-ring ring-congruence ideal lattice span map comap kernel Galois-connection left-ideal right-ideal opposite-ring module additive-subgroup absorption non-unital commutative-vs-noncommutative bigoperators
