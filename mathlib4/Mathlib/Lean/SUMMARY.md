---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean
generated: 2026-01-25T10:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 14
subdirs_count: 4
---

# Lean

## Overview

The `Mathlib/Lean/` directory provides comprehensive metaprogramming infrastructure extending Lean 4's core libraries across the full elaboration and meta-programming stack. At its foundation, it offers utilities for working with fundamental types (Expr, Name, Environment) and monads (CoreM, MetaM, TacticM), including expression manipulation (numeric literals, recursive replacement, pattern matching), name operations, linter APIs, and exception handling. The elaboration layer adds IDE integration (info trees, Try This suggestions), tactic execution in MetaM, and pattern elaboration. The meta layer provides sophisticated automation infrastructure: refined discrimination trees for efficient library search with lazy evaluation and scoring, advanced congruence lemma generation with subsingleton discovery, simplification support, and subexpression rewriting utilities. Finally, the pretty-printing layer extends the delaborator with binder handling and go-to-definition annotations. Together, these tools form critical infrastructure for Mathlib's metaprogramming needs, enabling the 300+ tactics, automation systems, IDE features, and code analysis tools that define Mathlib's user experience.

## Key Files

| File | Purpose |
|------|---------|
| Expr.lean | Public imports for expression utilities (Basic, ReplaceRec) |
| Meta.lean | Additional utilities for MVarId and MetaM: `let` (add hypothesis), `existsi` (refine with existential introduction), `intros!` (intro with unfolding), `getType''` (instantiate and clean metavariable types), `liftMetaTactic'` (single-goal tactic lifting), `run_for` (run TacticM from MetaM with return value) |
| Name.lean | Extended Name utilities: `allNames`/`allNamesByModule` (retrieve names from environment with filtering), `decapitalize`, `willRoundTrip` (check if name parses back to same identifier) |
| ContextInfo.lean | Execute CoreM/MetaM/TacticM actions using infotree context: `runCoreMWithMessages`, `runMetaMWithMessages`, `runTactic`, `runTacticCode` - enables running tactics in language server/editor contexts with proper message logging and context restoration |
| Linter.lean | Linter API utilities: `whenLinterOption` (conditionally run when linter enabled), `whenNotLinterOption`, `whenLinterActivated` (process `set_option ... in` and check linter status with optional error breaking) |
| Environment.lean | Additional Environment utilities: `findConstValWithKind?` (get ConstantVal with its ConstantKind), `findConstValOfKind?` (find constants matching kind predicate), `findTheoremConstVal?` (specialized for theorems only) |
| LocalContext.lean | Additional LocalContext methods: `firstDeclM`/`lastDeclM` (find first/last declaration satisfying monadic predicate) |
| Json.lean | JSON serialization instances for `PUnit`, `Fin n`, and `Subtype p` |
| CoreM.lean | CoreM state utilities: `withImportModules` (run CoreM action in fresh environment with specified imports) |
| EnvExtension.lean | Environment extension helpers: `Inhabited` instance for `ScopedEnvExtension.State` |
| Exception.lean | Exception utilities: `successIfFail` (generalized fail_if_success for MonadError), `isFailedToSynthesize` (check if exception is "failed to synthesize" error) |
| GoalsLocation.lean | SubExpr.GoalsLocation utilities: `rootExpr` (get root expression at location), `pos` (get SubExpr.Pos), `fvarId?` (get hypothesis if applicable) |
| Thunk.lean | Basic Thunk utilities and instances: simp lemmas for `get`/`pure`/`mk`, `DecidableEq`, `prod` (Cartesian product), `add` (thunk addition with Add instance) |
| Message.lean | Deprecated module (since 2025-08-18), imports Lean.Message and deprecation machinery |

## Subdirectories

- [x] `Elab/` - Elaboration infrastructure with info tree utilities (IDE support, Try This suggestions, theorem extraction), term elaboration helpers (pattern elaboration, universe levels), and tactic execution in MetaM contexts
- [x] `Expr/` - Fundamental expression utilities: recognizers and constructors for numeric literals (naturals, integers, rationals) and relations, name operations, expression modifiers, proof erasure, projection creation, set coercions, and recursive replacement with memoization
- [x] `Meta/` - Advanced MetaM infrastructure: refined discrimination tree for library search with lazy evaluation and scoring, congruence lemma generation with subsingleton discovery, simplification context construction and helpers, subexpression matching with position utilities for safe rewriting, and high-level tactic utilities for expression transformation
- [x] `PrettyPrinter/` - Delaborator extensions for converting internal expressions to user-facing syntax, with utilities for binder handling, options-per-position, and go-to-definition annotations

## Search Tags

lean4 metaprogramming utilities expressions names environment linter tactic-elaboration infotree context monad-extensions core-extensions mathlib-infrastructure json serialization exceptions thunks local-context
