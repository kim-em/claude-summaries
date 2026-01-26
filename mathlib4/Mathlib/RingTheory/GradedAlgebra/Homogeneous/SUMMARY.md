---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/GradedAlgebra/Homogeneous
generated: 2026-01-26T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Homogeneous

## Overview

The `Homogeneous/` directory provides the theory of homogeneous elements and structures within graded algebras. It defines homogeneous ideals, submodules, and subsemirings—algebraic structures that are closed under projection to graded components. Core results include characterizations of homogeneity, lattice operations preserving homogeneity, Galois connections between homogeneous cores and hulls, and the irrelevant ideal (elements with zero degree-zero component).

## Key Files

| File | Purpose |
|------|---------|
| Ideal.lean | Homogeneous ideals in graded rings; `Ideal.IsHomogeneous` definition and lattice structure for `HomogeneousIdeal`; homogeneous core (largest homogeneous ideal contained in `I`) and hull (smallest containing `I`) with Galois insertion/coinsertion; irrelevant ideal `⨁_{i>0} 𝒜ᵢ = {a \| a₀ = 0}` |
| Submodule.lean | Homogeneous submodules `HomogeneousSubmodule 𝒜 ℳ` for graded modules; closure under projection to components; extensionality lemmas and membership characterizations |
| Subsemiring.lean | Homogeneous subsemirings in graded semirings; closure of homogeneous elements forms homogeneous subsemiring; homogeneous core construction for arbitrary subsemirings |

## Subdirectories

(No subdirectories)

## Search Tags

homogeneous-element homogeneous-ideal homogeneous-submodule homogeneous-subsemiring graded-algebra graded-ring graded-module projection decompose IsHomogeneous HomogeneousIdeal HomogeneousSubmodule HomogeneousSubsemiring homogeneous-core homogeneous-hull Galois-insertion Galois-coinsertion irrelevant-ideal complete-lattice lattice-operations degree-zero-component
