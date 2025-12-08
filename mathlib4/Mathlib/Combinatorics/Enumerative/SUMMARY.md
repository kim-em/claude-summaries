---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Enumerative
generated: 2025-12-08T19:15:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 9
subdirs_count: 1
---

# Enumerative

## Overview

The `Enumerative/` directory contains formalized enumerative combinatorics: the branch of mathematics concerned with counting objects with specific properties. Core topics include Bell numbers (counting set partitions with various refinements), Catalan numbers (counting binary trees, Dyck paths, and balanced brackets with explicit formulas and bijections), compositions (ordered partitions contrasting with unordered integer partitions), double counting arguments for bipartite graphs, Dyck words (balanced parentheses sequences), incidence algebras (multiplicative structures on posets with Möbius inversion and Euler characteristic), inclusion-exclusion principles (alternating sum formulas for unions and intersections), and Stirling numbers (counting permutations with k cycles and set partitions into k subsets). The `Partition/` subdirectory provides a comprehensive theory of integer partitions including the fundamental `Partition n` structure as multisets, conversions between partitions and other structures (compositions, symmetric functions), special partition types (odd parts, distinct parts), and a complete generating function theory with infinite product formulas including `genFun f = ∏' i, (1 + ∑' j, f(i+1)(j+1) • X^((i+1)*(j+1)))` with convergence proofs.

## Key Files

| File | Purpose |
|------|---------|
| Bell.lean | Bell numbers for multisets: refined Bell numbers `Multiset.bell m` counting partitions of sets with parts of given cardinalities, uniform Bell numbers `Nat.uniformBell m n` for dividing `m * n` elements into `m` groups of `n`, and standard Bell numbers `Nat.bell n` counting all partitions of `n` elements; includes recurrence relations and factorial formulas |
| Catalan.lean | Catalan numbers: recursive definition `catalan (n+1) = ∑ i, catalan i * catalan (n-i)`, explicit formula `catalan n = centralBinom n / (n+1)`, and bijection with binary trees proving `treesOfNumNodesEq_card_eq_catalan` that `n` internal nodes yield `catalan n` trees |
| Composition.lean | Compositions of natural numbers as ordered partitions: `Composition n` structure with list of positive integers summing to `n`, representing decompositions of `{0,...,n-1}` into consecutive blocks; includes `blocksFun`, `sizeUpTo`, `embedding`, `index`, splitting/joining lists along compositions, and bijection with `CompositionAsSet` proving `composition_card n = 2^(n-1)` |
| DoubleCounting.lean | Double counting arguments for bipartite graphs: bounds number of edges via `card_mul_le_card_mul` relating minimum/maximum edges per vertex to set sizes, with `bipartiteBelow`/`bipartiteAbove` functions counting edges and variants for strict inequalities |
| DyckWord.lean | Dyck words (balanced bracket sequences): structure with equal `U`s and `D`s where all prefixes have at least as many `U`s as `D`s, semilength (half the length), `firstReturn` index for matching brackets, bijection `equivTree` with binary trees, and proof that `catalan n` Dyck words exist of semilength `n` |
| IncidenceAlgebra.lean | Incidence algebras on locally finite orders: multiplicative structure on functions over intervals with convolution product, zeta function (constant 1 on intervals), inductively-defined Möbius function as left inverse of zeta, Möbius inversion formulas for sums over intervals, and Euler characteristic for bounded orders |
| InclusionExclusion.lean | Inclusion-exclusion principle: alternating sum formulas for unions/intersections via `inclusion_exclusion_sum_biUnion` (sum over union equals alternating sum over intersections) and `inclusion_exclusion_card_biUnion` (cardinality version), plus dual formulas for intersections of complements |
| Partition.lean | Re-export module for `Partition.Basic` (deprecated since 2025-11-15) |
| Stirling.lean | Stirling numbers: `stirlingFirst n k` (unsigned, counting permutations of `n` elements with `k` cycles) and `stirlingSecond n k` (counting partitions of `n` elements into `k` non-empty subsets), both with recurrence relations, diagonal formulas `stirlingFirst n n = stirlingSecond n n = 1`, and edge formulas involving factorials and binomial coefficients |

## Subdirectories

- [x] `Partition/` - Integer partitions and generating functions

## Search Tags

enumerative-combinatorics bell-numbers catalan-numbers compositions double-counting dyck-words dyck-paths incidence-algebra moebius-inversion inclusion-exclusion integer-partitions stirling-numbers set-partitions permutation-cycles binary-trees balanced-parentheses zeta-function euler-characteristic bipartite-graphs
