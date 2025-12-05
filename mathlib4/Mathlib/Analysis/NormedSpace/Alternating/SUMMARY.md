---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/NormedSpace/Alternating
generated: 2025-12-05T07:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 2
subdirs_count: 1
---

# Alternating

## Overview

The `Alternating/` directory contains deprecated import forwarding modules for alternating multilinear maps in normed spaces. All files were deprecated on 2025-11-21 and redirect to the reorganized `Mathlib.Analysis.Normed.Module.Alternating.*` hierarchy. The directory provides backward compatibility for code referencing the old `Mathlib.Analysis.NormedSpace.Alternating.*` paths, covering basic alternating map theory, curry operations, and uncurry operations specialized to Fin-indexed maps.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Alternating.Basic` (deprecated 2025-11-21) |
| Curry.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Alternating.Curry` (deprecated 2025-11-21) |

## Subdirectories

- [x] `Uncurry/` - Uncurry operations for alternating maps (complete)

## Search Tags

alternating-maps multilinear-maps normed-spaces deprecated-imports backward-compatibility curry uncurry fin-indexed module-reorganization
