---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean
generated: 2026-01-24T22:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 14
subdirs_count: 4
---

# Lean

## Overview

The `Mathlib/Lean/` directory provides low-level metaprogramming utilities and extensions to Lean 4's core libraries. It contains helper functions and additional APIs for working with Lean's internal types and monads (Expr, Name, Environment, CoreM, MetaM, etc.), plus specialized utilities for tactic elaboration, pretty printing, and linting. These are foundational tools that support Mathlib's metaprogramming infrastructure, including tactics, automation, and code analysis.

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

- [x] `Elab/` - Elaboration utilities for tactics and terms
- [x] `Expr/` - Expression manipulation tools
- [ ] `Meta/` - MetaM-level utilities
- [ ] `PrettyPrinter/` - Pretty printing customizations

## Search Tags

lean4 metaprogramming utilities expressions names environment linter tactic-elaboration infotree context monad-extensions core-extensions mathlib-infrastructure json serialization exceptions thunks local-context
