---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/NormedSpace/HahnBanach
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# HahnBanach

## Overview

The `HahnBanach/` directory contains deprecated import modules that forward to reorganized locations for Hahn-Banach theorem related functionality. All three files are deprecated modules (deprecated 2025-11-06) that provide backward compatibility for code referencing the old `Mathlib.Analysis.NormedSpace.HahnBanach.*` module paths. The content has been reorganized into the `Mathlib.Analysis.Normed.Module.HahnBanach` module for the extension theorem and `Mathlib.Analysis.LocallyConvex.*` modules for separation and separating dual theorems.

## Key Files

| File | Purpose |
|------|---------|
| Extension.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.HahnBanach` for the Hahn-Banach extension theorem (deprecated 2025-11-06) |
| SeparatingDual.lean | Deprecated import forwarding to `Mathlib.Analysis.LocallyConvex.SeparatingDual` and `Mathlib.Analysis.Normed.Operator.CompleteCodomain` for separating dual space theory (deprecated 2025-11-06) |
| Separation.lean | Deprecated import forwarding to `Mathlib.Analysis.LocallyConvex.Separation` for separation theorems in locally convex spaces (deprecated 2025-11-06) |

## Subdirectories

(none)

## Search Tags

hahn-banach deprecated-imports backward-compatibility extension-theorem separating-dual separation-theorems locally-convex functional-analysis normed-spaces module-reorganization
