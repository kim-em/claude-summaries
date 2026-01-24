---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/Meta/Tactic
generated: 2026-01-25T06:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Tactic

## Overview

The `Mathlib/Lean/Meta/Tactic/` directory provides additional high-level utilities for Lean's tactic-level metaprogramming, specifically focused on rewriting operations. It extends core Lean's `Lean.Meta.Tactic.Rewrite` module with convenience functions for expression rewriting in MetaM contexts without producing subgoals.

## Key Files

| File | Purpose |
|------|---------|
| Rewrite.lean | Convenience functions for rewriting in MetaM: `Expr.rewrite` (rewrites expression via equality proof, fails if subgoals produced), `Expr.rewriteType` (rewrites expression's type then transports via `Eq.mp`). Both use fresh metavariables as ambient goals and require rewrites to complete without subgoals. |

## Subdirectories

(none)

## Search Tags

lean4 metaprogramming tactic rewrite equality eq-mp type-rewriting expression-transformation metam
