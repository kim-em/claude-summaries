---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/AddTorsor
generated: 2025-12-04T14:30:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# AddTorsor

## Overview

Defines additive torsors (also known as principal homogeneous spaces or affine spaces) where an additive group acts transitively and freely on a nonempty type. The typeclass `AddTorsor G P` provides two operations: `+ᵥ` (vadd) for adding group elements to points, and `-ᵥ` (vsub) for subtracting points to produce group elements. The main file establishes the fundamental torsor axioms (`vsub_vadd` and `vadd_vsub` cancellation laws) and derives the complete algebraic theory including point reflection, equivalences, and instances for products and Pi types.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `AddTorsor G P` typeclass with fundamental axioms, basic cancellation lemmas, point reflection equivalences, and subsingleton characterization |
| Basic.lean | Additional torsor theory requiring more imports: cancellation lemmas for both commutative and non-commutative groups, set-theoretic operations on torsors, product and Pi type instances, and the `constVAddHom` homomorphism |

## Subdirectories

*(No subdirectories)*

## Search Tags

additive-torsor affine-space principal-homogeneous-space vadd vsub group-action transitive-action free-action point-reflection torsor-axioms
