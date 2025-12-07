---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Enriched/Limits
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Limits

## Overview

The `Limits/` directory formalizes conical limits in enriched category theory. In enriched categories, ordinary (conical) limits are distinguished from enriched limits—this directory focuses on the former. A conical limit in an enriched category `C` is a limit that exists in the underlying ordinary category and is preserved by all enriched covariant hom-functors `eCoyoneda V X`. The directory provides type classes for expressing existence of various kinds of conical limits (general limits, products, pullbacks, terminal objects) and establishes that these imply the corresponding ordinary limit existence.

## Key Files

| File | Purpose |
|------|---------|
| HasConicalLimits.lean | Core definitions for conical limit existence: `HasConicalLimit`, `HasConicalLimitsOfShape`, `HasConicalLimitsOfSize`, and proof that conical limits are preserved by enriched Yoneda embeddings |
| HasConicalProducts.lean | Type class `HasConicalProducts` for existence of conical products (limits of discrete diagrams) and abbreviation `HasConicalProduct` for individual products |
| HasConicalPullbacks.lean | Abbreviations `HasConicalPullback` for individual pullbacks and `HasConicalPullbacks` for all pullbacks, specialized to cospan diagrams |
| HasConicalTerminal.lean | Abbreviation `HasConicalTerminal` for conical terminal objects (limit over empty diagram), derived from conical products |

## Subdirectories

*(none)*

## Search Tags

enriched-categories conical-limits enriched-limits limit-preservation enriched-yoneda enriched-hom-functors products pullbacks terminal-objects discrete-diagrams cospan-diagrams kelly-enriched-category-theory category-theory limits-of-shape
