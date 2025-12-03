---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/ContinuousCohomology
generated: 2025-12-02T10:30:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# ContinuousCohomology

## Overview

The `ContinuousCohomology/` directory implements continuous cohomology theory for topological groups acting on topological modules. It defines continuous cohomology as the homology of homogeneous cochains, using a categorical framework with functors from `Action (TopModuleCat R) G` to cochain complexes. The implementation uses an inductive definition of homogeneous cochains as G-invariant continuous functions in `C(G, C(G,...,C(G, M)))` rather than the traditional `C(Gⁿ, M)`, allowing for more general topological groups beyond locally compact ones.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions for continuous cohomology: defines the functor `I` taking representations to `C(G, rep)`, the complex of homogeneous cochains (`MultiInd.complex`), the invariants functor extracting G-invariant submodules, and the continuous cohomology functor `continuousCohomology R G n`; proves `H⁰_cont(G, X) ≅ Xᴳ` via `continuousCohomologyZeroIso` |

## Subdirectories

None.

## Search Tags

continuous-cohomology topological-groups group-cohomology homogeneous-cochains categorical-cohomology action-categories topological-modules invariants cochain-complex homology-functor group-representations
