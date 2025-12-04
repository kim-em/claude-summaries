---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicTopology/SingularHomology
generated: 2025-12-04T00:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# SingularHomology

## Overview

This directory defines singular homology theory for topological spaces, constructing the singular chain complex and homology functors with coefficients in arbitrary preadditive categories with homology. The implementation generalizes the classical construction to work in any suitable category, recovering ordinary singular homology when taking coefficients in the abelian groups. It includes a complete calculation of the homology of totally disconnected spaces as a fundamental example.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the singular chain complex functor (via composition of the singular set functor with the alternating face map complex), the singular homology functor, and proves that totally disconnected spaces have trivial higher homology with H₀ isomorphic to the free module on the space's points |

## Subdirectories

*(No subdirectories)*

## Search Tags

singular-homology singular-chain-complex homology algebraic-topology chain-complex totally-disconnected-space homology-functor coefficients preadditive-category
