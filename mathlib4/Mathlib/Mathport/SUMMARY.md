---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Mathport
generated: 2026-01-25T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Mathport

## Overview

The `Mathlib/Mathport/` directory is a vestigial compatibility layer that historically contained instructions for `mathport`, the automated tool that translated Lean 3's `mathlib` to Lean 4's `mathlib4`. The directory has been emptied of its original content, with only a README remaining to guide users who still need mathport support back to the `v3-eol` tag, which contains the final mathport infrastructure including syntax translation mappings and an implicit TODO list of unported Lean 3 tactics. This directory serves as a historical marker of the completed Lean 3 to Lean 4 migration.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Explains that mathport infrastructure has been removed and directs users needing mathport to the `v3-eol` tag, which contains the final form of mathport support including `Syntax.lean` with unported tactics list |

## Subdirectories

(none)

## Search Tags

mathport lean3-lean4-migration compatibility porting-tool v3-eol historical syntax-translation deprecated
