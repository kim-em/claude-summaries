---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Matroid/Minor
generated: 2025-12-08T20:15:32Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 4
subdirs_count: 0
---

# Minor

## Overview

The `Minor/` directory implements the theory of matroid minors, which are matroids obtained through deletion and contraction operations. These operations generalize the graph-theoretic notions of edge deletion and edge contraction to the abstract matroid setting. Deletion `M ＼ D` restricts a matroid to its ground set minus `D`, while contraction `M ／ C` is the dual operation (defined as `(M✶ ＼ C)✶`). Together they form the foundation of the minor partial order on matroids, central to structural matroid theory and analogous to the minor relation for graphs.

## Key Files

| File | Purpose |
|------|---------|
| Restrict.lean | Matroid restriction `M ↾ R` (independent sets of `M` contained in `R`); defines restriction partial order `≤r`; proves `(M ↾ X).IsBase I ↔ M.IsBasis I X`; establishes `Matroidᵣ α` type synonym with `PartialOrder`; includes `IsBasis` transfer lemmas and augmentation theorems |
| Delete.lean | Matroid deletion `M ＼ D` as restriction to `M.E \ D`; dual to contraction; deletion commutes with itself; preserves finiteness/finitary properties; relates loops/circuits/closure under deletion; satisfies `M ＼ D ≤r M` unconditionally |
| Contract.lean | Matroid contraction `M ／ C` defined as `(M✶ ＼ C)✶`; duality: `(M ／ C)✶ = M✶ ＼ C`; proves `IsBasis.contract_indep_iff`: `(M ／ I).Indep J ↔ Disjoint J I ∧ M.Indep (J ∪ I)` for basis `I`; contraction-deletion commutativity `M ／ C ＼ D = M ＼ D ／ C` for disjoint `C, D`; fundamental circuit lifting; contraction of circuits; preserves rank-finiteness and finitary property |
| Order.lean | Minor partial order `N ≤m M` (exists `C, D` with `N = M ／ C ＼ D`); strict minors `N <m M`; proves reflexivity, transitivity, antisymmetry; establishes `PartialOrder (Matroid α)` instance; shows `C, D` can be chosen disjoint via `IsMinor.exists_eq_contract_delete_disjoint`; minors preserve independence/dependence with subset restrictions |

## Subdirectories

*(No subdirectories)*

## Search Tags

matroid-minor deletion contraction restriction partial-order duality dual-operation ground-set independent-set basis circuit fundamental-circuit matroid-theory structural-combinatorics isomorphism reflexive transitive antisymmetric finitary rank-finite minor-closed graph-minor representability
