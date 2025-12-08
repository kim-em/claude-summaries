---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/WithTerminal
generated: 2025-12-08T15:38:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 4
subdirs_count: 0
---

# WithTerminal

## Overview

The `WithTerminal/` directory formalizes constructions for freely adjoining terminal and initial objects to categories. It provides `WithTerminal C` and `WithInitial C`, which are categories built from `C` by formally adding a terminal or initial object respectively, along with universal properties, functoriality, equivalences with comma categories, and additional structural results including connections to cones/cocones and finite category instances.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `WithTerminal C` and `WithInitial C` as inductive types, category structures, inclusion functors, lift operations with universal properties, functoriality (`map`), pseudofunctors on Cat, equivalences with comma categories, and opposite equivalences |
| Cone.lean | Relations between cone categories and WithTerminal/WithInitial constructions, including `liftFromOver` and `liftFromUnder` functors, equivalences between `Cone K` and `Cone (liftFromOver K)` (and dual for cocones), and limit/colimit preservation results for Over/Under categories |
| FinCategory.lean | Finiteness results showing `WithTerminal C` and `WithInitial C` are finite categories when `C` is, including `Fintype` instances via equivalence with `Option C` and `FinCategory` instances |
| Lemmas.lean | Additional lemmas requiring more imports, primarily cofiltered and filtered category instances: `WithTerminal C` is cofiltered when `C` is cofiltered-or-empty, `WithInitial C` is filtered when `C` is filtered-or-empty |

## Subdirectories

(none)

## Search Tags

category-theory with-terminal with-initial freely-adjoining terminal-objects initial-objects universal-properties lift comma-categories pseudofunctors cones cocones limits colimits over-categories under-categories finite-categories cofiltered filtered
