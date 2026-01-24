---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Coset
generated: 2026-01-24T23:10:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Coset

## Overview

The `Coset/` directory formalizes the foundational theory of left and right cosets in group theory. It provides core definitions of coset equivalence relations, the quotient type construction `α ⧸ s` for quotients by subgroups, canonical maps between cosets and subgroups, and cardinality results including Lagrange's theorem. The files progress from basic definitions and quotient constructions through computational lemmas about coset membership and equivalence, to finiteness conditions and the fundamental divisibility result that subgroup order divides group order.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core quotient type definitions: `leftRel`/`rightRel` equivalence relations, `QuotientGroup.mk` canonical map, basic `QuotientGroup.eq` characterization, bijection between left and right coset quotients |
| Basic.lean | Coset theory infrastructure: membership characterizations (`mem_leftCoset_iff`), coset equivalence predicates, associativity lemmas, bijections between cosets and subgroups (`leftCosetEquivSubgroup`), quotient embedding/mapping functions, product decompositions (`groupEquivQuotientProdSubgroup`), fiber equivalences for homomorphisms |
| Card.lean | Lagrange's theorem and cardinality: finiteness instances for quotients, proof that `Nat.card α = Nat.card (α ⧸ s) * Nat.card s`, divisibility results (`card_subgroup_dvd_card`, `card_quotient_dvd_card`) |

## Subdirectories

None.

## Search Tags

coset left-coset right-coset quotient-group lagrange-theorem subgroup-index cardinality fiber-equivalence coset-equivalence quotient-type setoid
