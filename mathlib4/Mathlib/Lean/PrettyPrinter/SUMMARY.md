---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/PrettyPrinter
generated: 2026-01-25T07:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# PrettyPrinter

## Overview

This folder contains extensions to Lean 4's delaborator, which converts internal expressions back into user-facing syntax for display. The single file provides additional DelabM utilities for working with binders, options, and go-to-definition annotations during delaboration.

## Key Files

| File | Purpose |
|------|---------|
| Delaborator.lean | Delaborator extensions: `withBindingBodyUnusedName'` (descend into lambda/pi body with fresh name and fvar), `OptionsPerPos.setBool` (update options at subexpression position), `annotateGoToDef` (add go-to-def info to syntax with module and range), `annotateGoToSyntaxDef` (add go-to-def for notation kind) |

## Subdirectories

None

## Search Tags

lean4 delaborator pretty-printer syntax-annotation go-to-definition binder-handling options-per-position term-info metaprogramming
