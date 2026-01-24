---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics/Circle
generated: 2026-01-24T00:00:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 0
subdirs_count: 1
---

# Circle

## Overview

The `Circle/` directory formalizes the dynamics of circle maps in Mathlib, specifically focusing on rotation number theory for orientation-preserving circle homeomorphisms. The key concept is the translation number (also called rotation number), which measures the average asymptotic displacement of points under iteration of a monotone map that commutes with integer translation.

## Key Files

| File | Purpose |
|------|---------|
| *(no files directly in this folder)* | |

## Subdirectories

- [x] `RotationNumber/` - Translation/rotation number theory for lifts of circle homeomorphisms; defines `CircleDeg1Lift` as monotone maps `f : ℝ → ℝ` satisfying `f(x+1) = f(x)+1`, with the translation number τ(f) = lim (f^n(x) - x)/n

## Search Tags

circle-dynamics rotation-number translation-number circle-homeomorphisms degree-one-lift monotone-maps semiconjugacy Poincare orbit-equivalence circle-maps
