---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Countable
generated: 2025-12-09T02:00:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 3
subdirs_count: 0
---

# Countable

## Overview

The `Countable/` directory defines typeclasses for countable and uncountable types in Lean. `Countable α` means there exists an injective map from `α` to `ℕ`, while `Uncountable α` means the type is not countable. These are weaker than `Encodable` (which requires a specific encoding) and serve as a general framework for reasoning about cardinality. The files provide basic instances for built-in types (Bool, Nat, Int, products, sums, options, etc.) and establish the connection to the `Small` typeclass.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of `Countable` and `Uncountable` typeclasses with basic instances (Nat, Bool, Fin, subsingletons, finite types, PLift, ULift, quotients) and fundamental lemmas about injectivity/surjectivity preservation |
| Basic.lean | Extended instances for type operations: sums, products, options, sigma types, dependent functions over finite domains; establishes equivalence with `Function.Embedding` characterization |
| Small.lean | Proves that all countable types are small (equivalent to a type in any universe); connects countability to universe-level size |

## Subdirectories

*(none)*

## Search Tags

countable uncountable cardinality injective-to-nat typeclass small-types finite-types encodable embedding
