---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Extremal
generated: 2025-12-08T20:30:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# Extremal

## Overview

The `Extremal/` directory contains extremal combinatorics results focusing on the Ruzsa-Szemerédi problem. This problem asks for the maximum number of edges a graph on n vertices can have if each edge belongs to exactly one triangle (locally linear graphs). The directory provides both the definition of the Ruzsa-Szemerédi number and proves asymptotic lower bounds by constructing graphs from 3-arithmetic-progression-free sets via Behrend's construction.

## Key Files

| File | Purpose |
|------|---------|
| RuzsaSzemeredi.lean | Ruzsa-Szemerédi problem: defines the Ruzsa-Szemerédi number (maximum edges in locally linear graphs), proves construction from 3AP-free sets using tripartite graphs from triangles, establishes lower bounds via Behrend's construction showing `Ω(n² * exp(-4 * √(log n)))` edges possible, and connections to additive Roth numbers |

## Subdirectories

None.

## Search Tags

extremal-combinatorics ruzsa-szemeredi locally-linear-graph triangle edge-triangle-incidence graph-theory behrend-construction 3ap-free additive-combinatorics roth-number asymptotic-bounds
