---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Fin/Tuple
generated: 2025-12-09T09:14:34Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 9
subdirs_count: 0
---

# Tuple

## Overview

The `Tuple/` directory provides comprehensive operations and theory for tuples represented as `Fin n → α`, treating them as vectors with statically-known length. It includes fundamental tuple manipulation operations (cons, tail, snoc, init, insertNth, removeNth, append, repeat, take), currying/uncurrying n-ary functions, embedding theory for injective tuples, finset membership for tuple products, natural number antidiagonals (tuples summing to a given value), reflection operations with proof-by-computation support, sorting tuples with monotonicity guarantees, and bubble sort induction principles for proving properties about sorted tuples.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core tuple operations on `Fin n → α`; defines cons/tail (adding/removing at start), snoc/init (adding/removing at end), insertNth/removeNth (adding/removing at arbitrary position), append (concatenating tuples), repeat (repeating tuples), and find (searching tuples); includes fundamental lemmas and induction principles |
| BubbleSortInduction.lean | Bubble sort induction principle for tuples; provides `Tuple.bubble_sort_induction` and `Tuple.bubble_sort_induction'` for proving properties preserved when swapping antitone values, using well-founded induction on lexicographic ordering of permutations |
| Curry.lean | Currying and uncurrying of n-ary functions; defines `Function.OfArity.curry/uncurry` for homogeneous n-ary functions and `Function.FromTypes.curry/uncurry` for heterogeneous functions, converting between `f a₁ a₂ ⋯ aₙ` and `f ![a₁, a₂, ⋯, aₙ]` |
| Embedding.lean | Embedding construction operations for `Fin n ↪ α`; defines `Fin.Embedding.cons`, `tail`, `snoc`, `init`, `append` for building injective tuples incrementally, plus `Function.Embedding.twoEmbeddingEquiv` relating `Fin 2 ↪ α` to pairs of distinct elements |
| Finset.lean | Finset operations for Fin-indexed tuples; proves membership lemmas for `piFinset` (Cartesian products of finsets) using cons/snoc/insertNth decompositions, and provides cardinality formulas for filtered products |
| NatAntidiagonal.lean | Collections of tuples with fixed sum; generalizes `Nat.antidiagonal` to k-tuples summing to n via `List.Nat.antidiagonalTuple`, `Multiset.Nat.antidiagonalTuple`, `Finset.Nat.antidiagonalTuple`; includes lexicographic ordering and equivalence with `Fin k → ℕ` |
| Reflection.lean | Reflection-based computational support for tuples; defines `FinVec.seq`, `map`, `sum`, `prod`, `etaExpand` with special definitional behavior on `![]` notation for proof-by-reflection; includes meta-level code for generating explicit sums/products |
| Sort.lean | Sorting tuples by values; defines `Tuple.sort f` producing a permutation that orders `Fin n` by outputs of `f : Fin n → α`, proves `Tuple.monotone_sort`, uniqueness of monotone permutations, and characterizes when tuples are sorted |
| Take.lean | Take operation restricting tuples to initial segments; defines `Fin.take m h v` extracting first m elements of n-tuple v (where h : m ≤ n), with lemmas for composition with other tuple operations (update, append, addCases) and correspondence with `List.take` |

## Subdirectories

None.

## Search Tags

tuple fin-tuple vector operations cons tail snoc init insertNth removeNth append repeat curry uncurry embedding finset antidiagonal sorting reflection take n-ary
