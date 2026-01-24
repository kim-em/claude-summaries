---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/Meta
generated: 2026-01-25T05:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 6
subdirs_count: 2
---

# Meta

## Overview

The `Mathlib/Lean/Meta/` directory provides advanced metaprogramming utilities for working with Lean's `MetaM` monad and meta-level operations. It contains extensions to core Lean functionality for congruence lemma generation, discrimination trees (both standard and refined), simplification support, subexpression matching, and rewriting. These tools support Mathlib's automation tactics and enable sophisticated expression indexing, unification, and transformation capabilities.

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

- [x] `RefinedDiscrTree/` - Implementation details for refined discrimination tree (Basic, Encode, Initialize, Lookup)
- [x] `Tactic/` - Tactic-level utilities for expression rewriting

## Search Tags

lean4 metaprogramming metamonad metam congruence-lemmas discrimination-tree refined-discr-tree simplifier simp-context unification pattern-matching subexpression-matching rewriting kabstract type-checking coercion expression-indexing library-search tactic-support
