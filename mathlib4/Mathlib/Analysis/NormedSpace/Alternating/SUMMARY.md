---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/NormedSpace/Alternating
generated: 2025-12-05T07:40:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 1
---

# Alternating

## Overview

The `Alternating/` directory is a deprecated import layer providing backward compatibility for alternating multilinear maps in normed spaces. All content was deprecated on 2025-11-21 during a module reorganization that moved alternating map functionality to `Mathlib.Analysis.Normed.Module.Alternating.*`. The directory contains two top-level import forwarders for basic alternating map theory and curry operations, plus a subdirectory for uncurry operations. The `Uncurry/` subdirectory specifically handles uncurry operations for Fin-indexed alternating maps, maintaining compatibility with code that referenced the old `Mathlib.Analysis.NormedSpace.Alternating.Uncurry.*` namespace.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Alternating.Basic` (deprecated 2025-11-21) |
| Curry.lean | Deprecated import forwarding to `Mathlib.Analysis.Normed.Module.Alternating.Curry` (deprecated 2025-11-21) |

## Subdirectories

- [x] `Uncurry/` - Uncurry operations for alternating maps (complete)

## Search Tags

alternating-maps multilinear-maps normed-spaces deprecated-imports backward-compatibility curry uncurry fin-indexed module-reorganization
