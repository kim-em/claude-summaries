---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monoidal/OfChosenFiniteProducts
generated: 2025-12-07T11:10:45Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# OfChosenFiniteProducts

## Overview

This directory contains deprecated module redirects that previously provided monoidal structures constructed from explicitly chosen finite products. Both files were deprecated on 2025-05-08 and now simply re-export `Mathlib.CategoryTheory.Monoidal.Cartesian.Basic`, indicating that this functionality has been consolidated into the Cartesian monoidal category framework. This is a legacy compatibility layer for code that previously imported from this location.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Deprecated module redirecting to Cartesian.Basic for basic monoidal structure from chosen products |
| Symmetric.lean | Deprecated module redirecting to Cartesian.Basic for symmetric monoidal structure from chosen products |

## Subdirectories

None

## Search Tags

deprecated monoidal-categories chosen-finite-products cartesian-monoidal legacy-compatibility module-redirect
