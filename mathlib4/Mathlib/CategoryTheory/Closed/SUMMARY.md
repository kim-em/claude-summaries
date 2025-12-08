---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Closed
generated: 2025-12-07T19:50:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 9
subdirs_count: 1
---

# Closed

## Overview

The `Closed/` directory is a deprecated compatibility layer that redirects to the new organizational structure at `Mathlib.CategoryTheory.Monoidal.Closed`. All nine top-level files were deprecated on 2025-11-28 and forward imports to the restructured location where closed category theory is properly categorized under monoidal categories. The directory covers the full spectrum of closed category structures: basic monoidal closed categories, cartesian closed categories, enrichment structures, functors between closed categories, closed structures on functor categories (including completeness and groupoid cases), the closed structure on the Type category, closed ideals, and closed categories with zero objects. This backward compatibility layer ensures that existing code can continue using the old import paths while the library transitions to its new organizational structure.

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

- [x] `FunctorCategory/` - Deprecated redirects for closed structure on functor categories, including basic definitions, completeness properties, and groupoid cases

## Search Tags

deprecated-modules backward-compatibility closed-categories monoidal-closed-categories cartesian-closed redirects module-reorganization functor-categories enrichment
