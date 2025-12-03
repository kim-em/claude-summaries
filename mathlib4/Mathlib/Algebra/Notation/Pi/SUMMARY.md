---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Notation/Pi
generated: 2025-12-01T19:47:30Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Pi

## Overview

The `Pi/` directory defines pointwise algebraic notation and operations for dependent function types (`Pi` types: `∀ i, M i`). It establishes how algebraic operators (`0`, `1`, `+`, `*`, `•`, `^`, `⁻¹`, `/`, `star`) apply componentwise to functions, forming the foundation for function-level algebra. Additionally, it introduces `mulSingle`/`single` for creating functions supported at a single index (the function analogue of basis vectors), which is fundamental for later finite support and finitely supported function constructions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines pointwise instances for `One`, `Mul`, `Inv`, `Div`, `SMul`/`Pow`, and `Star` on Pi types; includes `Pi.prod` for building product-type maps; establishes composition and constant function lemmas for all operations |
| Basic.lean | Defines `Pi.mulSingle i x` (function with value `x` at index `i` and `1` elsewhere) with comprehensive lemmas for equality, injection, application via operators, and currying/uncurrying; provides the additive variant `Pi.single` |

## Subdirectories

None.

## Search Tags

pi-type dependent-function pointwise-notation algebraic-operators mul-single single-support function-update composition-lemmas star-operation to-additive curry-uncurry
