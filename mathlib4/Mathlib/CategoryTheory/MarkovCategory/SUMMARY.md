---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/MarkovCategory
generated: 2025-12-07T12:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# MarkovCategory

## Overview

The `MarkovCategory/` directory formalizes Markov categories, a categorical framework for probabilistic reasoning. A Markov category is a copy-discard category where the discard operation is natural with respect to all morphisms, meaning that composing any morphism with discard is equivalent to discarding directly. This naturality condition enforces a probabilistic interpretation where morphisms preserve normalization, and it leads to the key structural result that the monoidal unit is a terminal object.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `MarkovCategory` typeclass extending `CopyDiscardCategory` with natural discard, proves the monoidal unit is terminal |

## Subdirectories

None

## Search Tags

markov-category categorical-probability probability copy-discard-category natural-discard terminal-object monoidal-category normalization bayesian-inference string-diagrams
