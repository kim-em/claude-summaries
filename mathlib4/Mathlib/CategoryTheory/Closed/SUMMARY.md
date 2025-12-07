---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Closed
generated: 2025-12-07T10:45:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 9
subdirs_count: 1
---

# Closed

## Overview

The `Closed/` directory contains deprecated redirect modules that forward to the new location at `Mathlib.CategoryTheory.Monoidal.Closed`. All files in this directory are deprecated as of 2025-11-28 and simply re-export the corresponding modules from the monoidal subcategory structure. This directory exists for backward compatibility, allowing existing code to continue importing from the old location while the library transitions to the new organizational structure where closed categories are properly categorized under monoidal categories.

## Key Files

| File | Purpose |
|------|---------|
| Cartesian.lean | Deprecated redirect to Monoidal.Closed.Cartesian (cartesian closed categories) |
| Enrichment.lean | Deprecated redirect to Monoidal.Closed.Enrichment (enriched closed categories) |
| Functor.lean | Deprecated redirect to Monoidal.Closed.Functor (functors between closed categories) |
| FunctorToTypes.lean | Deprecated redirect to Monoidal.Closed.FunctorToTypes (closed structure on functors to types) |
| Ideal.lean | Deprecated redirect to Monoidal.Closed.Ideal (closed ideals) |
| Monoidal.lean | Deprecated redirect to Monoidal.Closed.Basic (basic monoidal closed category structure) |
| Types.lean | Deprecated redirect to Monoidal.Closed.Types (closed structure on Type category) |
| Zero.lean | Deprecated redirect to Monoidal.Closed.Zero (closed categories with zero objects) |

## Subdirectories

- [ ] `FunctorCategory/` - Deprecated redirects for closed structure on functor categories (pending)

## Search Tags

deprecated-modules backward-compatibility closed-categories monoidal-closed-categories cartesian-closed redirects module-reorganization
