---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/NonAssoc/LieAdmissible
generated: 2025-12-04T09:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# LieAdmissible

## Overview

This directory contains the definition and theory of Lie-admissible rings and algebras, which are non-associative structures whose commutator bracket `[x,y] = x*y - y*x` forms a Lie ring/algebra. The key property is an associator identity that ensures the Jacobi identity holds for the commutator. The implementation shows that both left and right pre-Lie structures are instances of Lie-admissible structures, establishing the connection between these non-associative algebra types.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `LieAdmissibleRing` and `LieAdmissibleAlgebra` classes with an associator identity, proves they yield Lie rings/algebras via commutator bracket, and shows that both left and right pre-Lie structures are Lie-admissible |

## Subdirectories

*(No subdirectories)*

## Search Tags

lie-admissible associator commutator-bracket lie-ring lie-algebra pre-lie nonassociative jacobi-identity
