---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Young
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Young

## Overview

The `Young/` directory formalizes Young diagrams and semistandard Young tableaux (SSYTs), fundamental objects in algebraic combinatorics and representation theory. Young diagrams are finite collections of cells arranged in up-left justified rows (represented as lower sets in ℕ × ℕ), with a complete API including lattice structure, transpose operation, row/column access, and equivalence to weakly decreasing lists of positive natural numbers. Semistandard Young tableaux are fillings of Young diagrams where entries are weakly increasing along rows and strictly increasing down columns.

## Key Files

| File | Purpose |
|------|---------|
| YoungDiagram.lean | Defines Young diagrams as finite lower sets in ℕ × ℕ grid with up-left justification; provides distributive lattice structure (sup/inf/bot), transpose as order isomorphism, row/column accessors with monotonicity properties, and equivalence between diagrams and sorted lists of row lengths |
| SemistandardTableau.lean | Defines semistandard Young tableaux as functions ℕ → ℕ → ℕ filling Young diagrams with weakly increasing rows and strictly increasing columns; includes the "highest weight" tableau where row i contains all i's, serving as canonical example |

## Subdirectories

*(No subdirectories)*

## Search Tags

young-diagram young-tableau semistandard-tableau ssyt algebraic-combinatorics representation-theory partition lower-set lattice transpose row-length column-length
