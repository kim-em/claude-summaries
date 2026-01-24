---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/Meta
generated: 2026-01-25T10:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 2
---

# Meta

## Overview

The `Mathlib/Lean/Meta/` directory provides advanced metaprogramming utilities for working with Lean's `MetaM` monad and meta-level operations. It extends core Lean functionality with sophisticated tools for congruence lemma generation, expression indexing via discrimination trees, simplification support, subexpression matching, and rewriting. The directory includes a comprehensive implementation of the refined discrimination tree (a lazy expression indexing data structure with parallel initialization and unification-based matching) and high-level tactic utilities for expression rewriting. These tools form critical infrastructure for Mathlib's automation tactics, enabling efficient library search, pattern matching, and expression transformation.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | MetaM utilities: `preservingMCtx` (restore mvar context after execution), `forallMetaTelescopeReducingUntilDefEq` (create metavars for forall binders until type matches target), `pureIsDefEq` (check definitional equality without assigning mvars), `mkRel` (optimized relation construction for Eq/Iff), `withEnsuringLocalInstance` (synthesize or assume typeclass instance), `ensureHasType`/`ensureIsFunction`/`ensureIsSort` (type checking with coercion support) |
| CongrTheorems.lean | Advanced congruence lemma generation: `mkHCongrWithArity'` (generates congruence lemmas with automatic subsingleton proof discovery), `mkRichHCongr` (creates congruence lemmas with dependency-aware hypotheses for each argument equality), `FastSubsingleton`/`FastIsEmpty` (fast-failing typeclass variants for congruence proof automation), `withSubsingletonAsFast` (context transformation for efficient subsingleton checking) |
| DiscrTree.lean | Discrimination tree extensions: `getSubexpressionMatches` (find all keys matching expression or subexpressions, returns results in priority order), `keysSpecific` (check if key array is specific vs wildcard pattern like `[*]` or `[=, *, *, *]`) |
| KAbstractPositions.lean | Subexpression position utilities for rewriting: `kabstractPositions` (find all positions that unify with a pattern), `viewKAbstractSubExpr` (get subexpression at position with occurrence number for `kabstract`), `kabstractIsTypeCorrect` (verify that abstracting a subexpression produces well-typed result, critical for `rw` tactic safety) |
| RefinedDiscrTree.lean | Public imports for refined discrimination tree: combines `Lookup` and `Initialize` modules, provides `findImportMatches`/`findModuleMatches`/`findMatches` functions for expression-based library search with scoring. Features lambda/forall indexing, numbered metavariable keys (`*0`, `*1` for pattern matching), η-reduction support, and lazy evaluation for efficient lookup |
| Simp.lean | Simplifier helper functions: `Result.ofTrue` (construct proof from simp result that reduces to True), `getPropHyps` (collect all propositional hypotheses), `simpTheoremsOfNames`/`Context.ofNames`/`Context.ofArgs` (construct simp contexts from lemma names or syntax), `simpOnlyNames` (simplify with specific lemmas only), `simpType` (simplify expression type and convert using type hints/casts), `simpEq` (independently simplify both sides of equality), `SimpTheorems.contains`/`isInSimpSet`/`getAllSimpDecls`/`getAllSimpAttrs` (query simp attribute membership) |

## Subdirectories

- [x] `RefinedDiscrTree/` - Complete lazy refined discrimination tree implementation with expression encoding, parallel tree initialization, and unification-based matching. Supports lambda/forall indexing, numbered metavariables, η-reduction, and scored results for library search
- [x] `Tactic/` - High-level tactic utilities for expression rewriting in MetaM contexts, providing convenience wrappers around core Lean rewrite functionality

## Search Tags

lean4 metaprogramming metamonad metam congruence-lemmas discrimination-tree refined-discr-tree simplifier simp-context unification pattern-matching subexpression-matching rewriting kabstract type-checking coercion expression-indexing library-search tactic-support
