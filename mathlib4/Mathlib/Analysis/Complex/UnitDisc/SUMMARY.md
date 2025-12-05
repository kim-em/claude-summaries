---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Complex/UnitDisc
generated: 2025-12-05T09:30:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# UnitDisc

## Overview

The `UnitDisc/` directory defines the complex unit disc (Poincaré disc) `𝔻` as the open unit ball in ℂ and establishes its basic algebraic and topological structure. It provides the type definition, coercion to ℂ, constructor functions, and proves fundamental properties like norm bounds (‖z‖ < 1 for all z ∈ 𝔻). The file also defines scalar actions by the unit circle and closed unit ball, real/imaginary part projections, and complex conjugation on the disc, establishing 𝔻 as a commutative semigroup with zero and various algebraic structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `Complex.UnitDisc` as the unit ball in ℂ; establishes coercion, norm properties (‖z‖ < 1), algebraic instances (CommSemigroup, SemigroupWithZero, HasDistribNeg); defines scalar actions by Circle and closedBall; provides re/im projections and conjugation |

## Subdirectories

None

## Search Tags

unit-disc poincare-disc complex-unit-ball open-unit-disc unit-circle-action closed-ball-action complex-conjugation norm-bounds algebraic-structures scalar-tower smul-comm-class
