---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Sym
generated: 2025-12-11T20:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 3
subdirs_count: 1
---

# Sym

## Overview

This directory defines symmetric powers of a type, which are fundamental constructions in combinatorics and algebra. The nth symmetric power `Sym α n` consists of homogeneous n-tuples modulo permutations by the symmetric group, implemented as multisets of fixed cardinality. The symmetric square `Sym2 α` (unordered pairs) receives extensive treatment as a special case, implemented as a quotient of `α × α` by swap. Key functionality includes membership operations, diagonal elements, conversions between symmetric relations and `Sym2` values, and the "stars and bars" combinatorial technique for counting multisets. The subdirectory extends `Sym2` with Aesop automation, finitely-supported function lifting, and order-theoretic operations including a canonical sorting equivalence with ordered pairs.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions for nth symmetric power `Sym α n` as `{s : Multiset α // card s = n}`; includes `cons`, `erase`, `replicate`, `map`, `attach`, `append`, `fill`, `filterNe`, and equivalence with vectors modulo permutations (`Sym'`) |
| Card.lean | Stars and bars combinatorics: proves `card (Sym α k) = multichoose (card α) k` and `card (Sym α k) = choose (card α + k - 1) k`; cardinality results for diagonal/off-diagonal elements of `Sym2` |
| Sym2.lean | Comprehensive treatment of symmetric square (unordered pairs): defines `Sym2 α` as quotient of `α × α` by swap; includes `Sym2.mk` notation `s(x, y)`, membership, `IsDiag` predicate, `fromRel`/`ToRel` for symmetric relations, `map`, `pmap`, `attachWith`, `toMultiset`, `toFinset`, `equivSym`, and integration with `Set.sym2` |

## Subdirectories

- [x] `Sym2/` - Additional symmetric square functionality (Aesop rule set, Finsupp lifting, ordering/sorting)

## Search Tags

symmetric-powers symmetric-square unordered-pairs multisets quotients permutations stars-and-bars combinatorics multichoose binomial-coefficients diagonal relations aesop finsupp sorting linear-order lattice
