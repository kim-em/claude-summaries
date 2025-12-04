---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/CStarAlgebra/Unitary
generated: 2025-12-04T14:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Unitary

## Overview

The `Unitary/` directory contains theory about unitary elements in C⋆-algebras, focusing on two major themes: the topological structure of the unitary group and the algebraic spanning property. It establishes that the unitary group is locally path connected via logarithmic maps on balls of radius 2, and proves that unitary elements span the entire C⋆-algebra as a complex vector space.

## Key Files

| File | Purpose |
|------|---------|
| Connected.lean | Proves the unitary group in a C⋆-algebra is locally path connected; establishes a partial homeomorphism between `ball (1 : unitary A) 2` and `ball (0 : selfAdjoint A) π` via `argSelfAdjoint` and `expUnitary`; characterizes the path component of identity as finite products of exponential unitaries |
| Span.lean | Proves that unitary elements span the entire C⋆-algebra; shows every element is a linear combination of four unitaries with coefficients bounded by `‖x‖ / 2`; constructs specific unitaries from selfadjoint elements using `a + I • √(1 - a²)` |

## Subdirectories

(none)

## Search Tags

unitary-group locally-path-connected exponential-map logarithm argSelfAdjoint selfadjoint-elements continuous-functional-calculus path-components homeomorphism spanning-sets linear-combinations spectral-theory slit-plane principal-branch unitary-elements cstar-algebras
