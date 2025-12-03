---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/WithTop
generated: 2025-12-01T19:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# WithTop

## Overview

The `WithTop/` directory provides conversion functionality from `WithTop α` (types with a top element) back to the base type `α`. The key contribution is `untop₀`, which maps elements to the base type by sending `⊤` to zero, similar to how `ENat.toNat` works. This includes comprehensive simplifier lemmas for algebraic operations (addition, negation, multiplication), order relations, and max/min operations when the base type has appropriate structure.

## Key Files

| File | Purpose |
|------|---------|
| Untop0.lean | Defines `WithTop.untop₀` conversion mapping `⊤` to zero, with simplification lemmas for zero classes, additive groups, multiplication, and ordered structures including comparison and max/min operations |

## Subdirectories

*(none)*

## Search Tags

with-top untop conversion top-element zero-mapping ordered-additive-groups linear-order simplification-lemmas gcongr
