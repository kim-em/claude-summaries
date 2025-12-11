---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Stream
generated: 2025-12-11T10:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 2
subdirs_count: 0
---

# Stream

## Overview

The `Stream/` directory defines `Stream' α`, an infinite sequence of elements of type `α` (essentially `ℕ → α`). This is named `Stream'` to avoid conflict with Lean's built-in `Stream` type. The implementation provides a rich API for working with infinite sequences, including construction (cons, iterate, corec), access (head, tail, get, drop), transformations (map, zip, interleave), and proofs via bisimulation and coinduction.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions for `Stream' α` including `cons`, `head`, `tail`, `drop`, `map`, `zip`, `iterate`, `corec`, `interleave`, `even`, `odd`, `cycle`, `tails`, `inits`, `take`, `appendStream'`, and the natural numbers stream `nats` |
| Init.lean | Theorems and properties about streams: extensionality, bisimulation proofs, coinduction principles, lemmas for all the operations defined in Defs.lean, and applicative functor laws (`pure`, `apply`) |

## Subdirectories

(none)

## Search Tags

stream infinite-sequence corecursion bisimulation coinduction iterate corec interleave even odd cycle tails inits take drop append-stream nats applicative
