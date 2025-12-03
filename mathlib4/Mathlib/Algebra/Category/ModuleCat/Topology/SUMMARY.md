---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/ModuleCat/Topology
generated: 2025-12-03T14:25:00Z
git_sha: 5bfa1623542d7f245e45ac880c26cfe8f9ecc5ea
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Topology

## Overview

The `Topology/` directory defines the category of topological modules (`TopModuleCat R`) for topological rings R, where modules carry compatible topological structure (topological addition and continuous scalar multiplication). It establishes that TopModuleCat has all limits and colimits (constructed via induced/coinduced topologies), provides three key adjunctions (module topology, indiscrete topology, and free-forgetful), and proves that TopModuleCat is a category with homology despite not being abelian, with kernels and cokernels carrying appropriate subspace/quotient topologies.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `TopModuleCat R` as modules over topological ring R with compatible topology; constructs limits via induced topology and colimits via coinduced topology; establishes three adjunctions: `withModuleTopology` (finest topology making module operations continuous) ⊣ forget to ModuleCat, forget to ModuleCat ⊣ `indiscrete` (coarsest topology), and `free` (free topological module over topological space) ⊣ forget to TopCat |
| Homology.lean | Proves `TopModuleCat R` is a `CategoryWithHomology` despite not being abelian; defines kernels as submodules with subspace topology and cokernels as quotients with quotient topology; establishes that left and right homology definitions coincide via topological embedding and surjectivity argument using `isEmbedding_of_isOpenQuotientMap_of_isInducing` |

## Subdirectories

*(No subdirectories)*

## Search Tags

topological-modules category-theory topology continuous-linear-maps limits colimits induced-topology coinduced-topology adjunctions module-topology indiscrete-topology free-modules homology kernels cokernels non-abelian-categories
