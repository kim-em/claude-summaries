---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Control/Monad
generated: 2025-12-08T15:45:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 3
subdirs_count: 0
---

# Monad

## Overview

The `Monad/` directory provides specialized monad constructs and infrastructure for advanced functional programming patterns. It contains core utilities for monad normalization (Basic), the continuation monad transformer (ContT/Cont) with call-with-current-continuation support, and writer monads (WriterT/Writer) for accumulating appendable state. These modules extend basic monad functionality with powerful control flow mechanisms and state management patterns.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core monad rewrite rules and normalization attributes (functor_norm, monad_norm); ext attributes for transformer equality; StateT.eval for discarding final state; equivalence functions reducing StateT/ReaderT equality to function space equality |
| Cont.lean | Continuation monad (ContT/Cont) with MonadCont typeclass for callCC (call-with-current-continuation); LawfulMonadCont laws; MonadCont instances for ExceptT, OptionT, WriterT, StateT, ReaderT with proper label lifting and goto operations; ContT.equiv for equivalence reduction |
| Writer.lean | Writer monad (WriterT/Writer) for accumulating output; MonadWriter typeclass with tell/listen/pass operations; instances for ReaderT, StateT composition; supports both [EmptyCollection ω] [Append ω] and [Monoid ω] contexts; MonadWriterAdapter for adapting writer output type; WriterT.equiv for equivalence reduction |

## Subdirectories

None.

## Search Tags

monad continuation-monad writer-monad monad-transformers callcc control-flow state-accumulation logging monadic-normalization functor-norm monad-norm lawful-monad continuation-passing-style cps tell-listen-pass monad-writer state-transformer reader-transformer except-transformer option-transformer equivalence-functors
