---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/Expr
generated: 2026-01-24T09:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 4
subdirs_count: 0
---

# Expr

## Overview

The `Mathlib/Lean/Expr/` directory contains fundamental utilities for working with Lean expressions (`Expr`). It provides recognizers, constructors, transformations, and specialized operations on expressions, including support for working with numeric literals (naturals, integers, rationals), set coercions, and recursive expression replacement with memoization. This is a core metaprogramming module used throughout Mathlib for expression analysis and manipulation.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Comprehensive expression utilities: binder info helpers, name operations (`mapPrefix`, `fromComponents`, `isPrefixOf?`), constant info manipulation, expression recognizers (`numeral?`, `le?`, `lt?`, `ne?`, `sides?`), expression modifiers (`modifyArg`, `setArg`, `renameBVar`), numeric construction (`ofNat`, `ofInt`), proof erasure (`eraseProofs`), projection creation (`mkProjection`), and structure reduction (`reduceProjStruct?`) |
| ExtraRecognizers.lean | Expression recognizers requiring theory imports: `coeTypeSet?` recognizes set-to-type coercions in the form `Set.Elem s` or `{x // x ∈ s}` |
| Rat.lean | Rational number support for expressions: `ToExpr Rat` instance, `rat?` recognizer for rational literals in normal form (including division normalization checks), `isExplicitNumber` predicate for numeric literals (naturals, integers, rationals) |
| ReplaceRec.lean | Recursive expression replacement with memoization: `replaceRec` provides a flexible alternative to `Expr.replace` where the replacement function has access to recursive calls, enabling transformations that can conditionally recurse into subexpressions |

## Subdirectories

*(No subdirectories)*

## Search Tags

lean4 metaprogramming expressions expr recognizers numeric-literals rational-numbers natural-numbers integers expression-manipulation binder-info name-operations constant-info projection structure-fields expression-transformation memoization set-coercions type-coercions proof-erasure
