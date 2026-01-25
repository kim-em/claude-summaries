---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/ConditionallyCompleteLattice
generated: 2026-01-26T03:28:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# ConditionallyCompleteLattice

## Overview

Conditionally complete lattices are lattices where every non-empty bounded subset has a supremum and infimum. This folder contains the core definitions and theory for conditionally complete lattices, including the main typeclasses (`ConditionallyCompleteLattice`, `ConditionallyCompleteLinearOrder`, `ConditionallyCompleteLinearOrderBot`), constructors, and properties. The theory parallels complete lattices but with additional boundedness and nonemptiness assumptions. Typical examples are `ℝ`, `ℕ`, and `ℤ` with their usual orders.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core typeclass definitions: `ConditionallyCompleteLattice` (with `le_csSup`, `csSup_le`, `csInf_le`, `le_csInf` axioms), `ConditionallyCompleteLinearOrder`, `ConditionallyCompleteLinearOrderBot`; constructors from `sSup`/`sInf` functions; well-founded linear order to conditionally complete lattice construction |
| Basic.lean | Main theory of conditionally complete lattices: extensions to `WithTop α` and `WithBot α`, fundamental lemmas about `csSup` and `csInf` with boundedness assumptions (statements prefixed with `c` to distinguish from complete lattice versions) |
| Indexed.lean | Indexed suprema and infima (`iSup`/`iInf`) for conditionally complete lattices; lemmas prefixed with `ci` (e.g., `ciSup_xxx`, `ciInf_xxx`) to distinguish from complete lattice versions; extensions to `WithTop` and `WithBot` |
| Finset.lean | Conditionally complete lattices and finite sets: connection between `csSup`/`csInf` and `Finset.max'`/`min'`, membership of suprema/infima in finite sets, bounded indexed suprema over finsets |
| Group.lean | Interaction of conditionally complete lattices with group operations: inequalities for `ciSup`/`ciInf` under multiplication with `MulLeftMono`/`MulRightMono` assumptions |

## Subdirectories

(no subdirectories)

## Search Tags

conditionally-complete-lattice csSup csInf bounded-above bounded-below supremum infimum indexed-sup indexed-inf WithTop WithBot finset linear-order well-founded lattice group-operations
