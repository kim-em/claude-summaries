---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/SimpleGraph/Regularity
generated: 2025-12-08T23:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 7
subdirs_count: 0
---

# Regularity

## Overview

The `Regularity/` directory contains a complete formalization of Szemerédi's Regularity Lemma (SRL), a landmark result in extremal combinatorics stating that any sufficiently large graph behaves approximately like a random graph. The implementation proves the equipartition version: for any ε > 0 and integer l, there exists a bound M such that any graph on at least l vertices can be partitioned into at least l and at most M parts, with the resulting equipartition being ε-uniform. The proof uses an energy increment method, repeatedly refining non-uniform partitions until energy stabilization forces uniformity.

## Key Files

| File | Purpose |
|------|---------|
| Lemma.lean | Main result: proves Szemerédi's Regularity Lemma via energy induction, iteratively applying increment construction until partition is ε-uniform or energy exceeds 1 |
| Uniform.lean | Defines ε-uniformity for pairs of vertex sets (edge density close across large subsets) and partitions (≥(1-ε) proportion of pairs are ε-uniform); includes witness construction for non-uniformity |
| Energy.lean | Defines partition energy (normalized sum of squared edge densities) as auxiliary quantity driving induction; proves energy bounded in [0,1] |
| Chunk.lean | Constructs partition refinement of a single part by atomizing along non-uniformity witnesses; proves local energy increase for non-uniform pairs and bounded decrease for uniform pairs |
| Increment.lean | Assembles chunk partitions into global increment partition; proves overall energy increase by at least ε^5/4 when partition is not uniform |
| Equitabilise.lean | Constructs equipartitions with prescribed part sizes (a parts of size m, b parts of size m+1) that almost refine given partitions; enables arbitrary-size equipartitions |
| Bound.lean | Provides numerical bounds for algorithm: stepBound (blowup factor 4^n per iteration), initialBound (starting partition size), bound (final maximum size); includes tower-type bound arithmetic |

## Subdirectories

*(No subdirectories)*

## Search Tags

szemeredi-regularity-lemma graph-uniformity epsilon-regular equipartition energy-increment extremal-combinatorics edge-density random-graph partition-refinement szrl combinatorics graph-theory
