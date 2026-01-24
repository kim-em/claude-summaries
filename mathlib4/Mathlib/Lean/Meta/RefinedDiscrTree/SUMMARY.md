---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Lean/Meta/RefinedDiscrTree
generated: 2026-01-25T09:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# RefinedDiscrTree

## Overview

Implementation of the lazy refined discrimination tree, an advanced expression indexing data structure for Lean metaprogramming. This directory provides the complete implementation including core data types (`Key`, `Trie`, `LazyEntry`), expression encoding with lazy evaluation and η-reduction support, tree initialization with parallel processing of imported modules, and matching/lookup operations with unification. The refined version improves on standard discrimination trees by supporting lambda/forall indexing, numbered metavariable keys for pattern matching, and lazy evaluation for efficient incremental computation.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core data structures: `Key` (discrimination tree keys including star/labelledStar metavariables, const/fvar/bvar with arity, literals, sort, lambda, forall, projection), `LazyEntry` (lazy computation state with stack, previous expression, metavariable context, and computed keys), `Trie` (tree node with values, star/labelledStar/children maps, and pending lazy entries), `RefinedDiscrTree` (root key map and array of tries). Provides formatting, hashing, and `keysAsPattern` for user-friendly display |
| Encode.lean | Expression encoding to key sequences: `encodingStep`/`encodingStepWithEta` (convert expressions to keys one at a time with lazy evaluation), `initializeLazyEntry`/`initializeLazyEntryWithEta` (compute first key and create lazy entry), `evalLazyEntry` (evaluate one step of lazy computation), `processPrevious` (expand application arguments onto stack), `getStackEntries` (determine which arguments to index vs ignore based on type info and implicit/instance status), `lambdaTelescopeReduce` (strip lambda binders with variable introduction), `etaPossibilities` (generate all possible η-reduced forms), `encodeExpr`/`encodeExprWithEta` (complete encoding functions) |
| Initialize.lean | Tree construction and population: `insert` (add key/lazy-entry pair to tree), `PreDiscrTree` (preliminary structure for fast concurrent initialization with root key map and pending entry arrays), `createImportedDiscrTree` (parallel construction from all imported constants using tasks allocated by `constantsPerTask`), `createModuleDiscrTree` (construction from current module declarations), `ModuleDiscrTreeRef` (reference wrapper for incremental updates), `addConstToPreDiscrTree` (helper for adding constants with error handling), `blacklistInsertion` (filter for unsuitable declarations like internal details, deprecated items, and auto-generated names), `ImportFailure`/`ImportErrorData` (error tracking during initialization) |
| Lookup.lean | Tree matching and lookup operations: `getMatch` (find values matching expression with optional unification and root star matching), `MatchResult` (scored results in TreeMap with `toArray`/`flatten` for ordered retrieval), `getMatchLoop` (main non-deterministic matching loop maintaining stack of `PartialMatch`es), `evalNode` (evaluate pending lazy entries in trie node, expanding keys and inserting into star/labelledStars/children maps), `matchQueryStar` (handle star metavariables in query expression), `matchTreeStars` (handle star/labelledStar patterns in discrimination tree with assignment checking), `matchKey` (exact key matching), `matchTreeRootStar` (handle root-level metavariable patterns), `TreeM` monad (state for tries array during matching) |

## Subdirectories

(none)

## Search Tags

lean4 metaprogramming refined-discrimination-tree discrimination-tree expression-indexing lazy-evaluation lazy-computation pattern-matching unification metavariables eta-reduction lambda-indexing forall-indexing library-search parallel-initialization trie-structure key-encoding scoring concurrent-processing
