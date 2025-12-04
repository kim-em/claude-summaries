---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/NonAssoc
generated: 2025-12-04T08:35:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: preliminary
files_count: 0
subdirs_count: 2
---

# NonAssoc

## Overview

The `NonAssoc/` directory contains theory for non-associative algebraic structures, focusing on pre-Lie algebras and Lie-admissible algebras. These are generalizations of associative algebras where the associator `(x * y) * z - x * (y * z)` satisfies weaker symmetry conditions rather than being zero. Pre-Lie algebras have associators symmetric in either the first two or last two variables, while Lie-admissible algebras satisfy a specific associator identity that ensures the commutator bracket `[x,y] = x*y - y*x` forms a Lie algebra.

## Key Files

*(No files directly in this directory)*

## Subdirectories

- [x] `LieAdmissible/` - Lie-admissible rings and algebras where the associator satisfies an identity ensuring the commutator bracket forms a Lie ring/algebra, with instances showing pre-Lie structures are Lie-admissible (complete)
- [x] `PreLie/` - Pre-Lie rings and algebras defined by left or right symmetry of the associator, with equivalence between left and right versions via opposite multiplication (complete)

## Search Tags

non-associative pre-lie lie-admissible associator commutator-bracket nonunital-ring
