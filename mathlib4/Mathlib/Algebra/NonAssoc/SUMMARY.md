---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/NonAssoc
generated: 2025-12-04T09:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 0
subdirs_count: 2
---

# NonAssoc

## Overview

The `NonAssoc/` directory provides foundational theory for non-associative algebraic structures, specifically pre-Lie algebras and Lie-admissible algebras. These structures generalize associative algebras by imposing weaker conditions on the associator `(x * y) * z - x * (y * z)`. The directory establishes the hierarchy: pre-Lie structures (which have symmetric associators) are instances of Lie-admissible structures (which satisfy associator identities ensuring their commutator brackets form Lie algebras). This formalization includes both ring and algebra (module) versions, with equivalences between left and right variants via opposite multiplication, providing the algebraic foundations for applications in control theory, numerical analysis, and deformation theory.

## Key Files

*(No files directly in this directory)*

## Subdirectories

- [x] `LieAdmissible/` - Lie-admissible rings and algebras where the associator satisfies an identity ensuring the commutator bracket forms a Lie ring/algebra, with instances showing pre-Lie structures are Lie-admissible (complete)
- [x] `PreLie/` - Pre-Lie rings and algebras defined by left or right symmetry of the associator, with equivalence between left and right versions via opposite multiplication (complete)

## Search Tags

non-associative pre-lie lie-admissible associator commutator-bracket nonunital-ring
