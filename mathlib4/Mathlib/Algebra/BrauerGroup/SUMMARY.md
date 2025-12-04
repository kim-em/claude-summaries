---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/BrauerGroup
generated: 2025-12-04T05:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# BrauerGroup

## Overview

The `BrauerGroup/` directory contains the foundational definitions for the Brauer group of a field K, a fundamental construction in algebraic number theory and noncommutative algebra. The Brauer group classifies finite-dimensional central simple algebras up to Brauer equivalence (the relation where two algebras are equivalent if their matrix rings are isomorphic). This single-file module defines the central simple algebra structure (`CSA`), the Brauer equivalence relation (algebras are equivalent if `Mₙ(A) ≃ₐ[K] Mₘ(B)` for some n, m), proves it is an equivalence relation, and defines the Brauer group as the quotient by this relation.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of Brauer group theory: `CSA K` structure for finite-dimensional central simple algebras over a field K (wrapping central, simple, and finite-dimensional properties), `IsBrauerEquivalent` relation stating two algebras are equivalent if their matrix algebras are isomorphic (with proof of reflexivity, symmetry, and transitivity), `Brauer.CSA_Setoid` constructing the setoid structure, and `BrauerGroup K` as the quotient type. Includes TODOs for proving the group structure via tensor products and functoriality from fields to groups. |

## Subdirectories

(none)

## Search Tags

brauer-group central-simple-algebra azumaya morita-equivalence galois-cohomology algebraic-number-theory matrix-algebras tensor-product field-theory quotient-setoid equivalence-relation
