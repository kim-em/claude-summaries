---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/ODE
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# ODE

## Overview

The `ODE/` directory contains formalization of ordinary differential equations, providing both fundamental inequalities for bounding ODE solutions and existence theorems for solutions to initial value problems. It implements Grönwall's inequality for controlling the growth of solutions and the Picard-Lindelöf (Cauchy-Lipschitz) theorem establishing local existence of integral curves and flows to time-dependent vector fields via the contraction mapping principle.

## Key Files

| File | Purpose |
|------|---------|
| Gronwall.lean | Grönwall-like inequalities bounding norm growth of functions satisfying derivative bounds; includes corollaries for distance between approximate/exact ODE solutions, uniqueness theorems for ODEs with Lipschitz right-hand sides |
| PicardLindelof.lean | Picard-Lindelöf (Cauchy-Lipschitz) theorem proving local existence of solutions to time-dependent ODEs; constructs solutions via contraction mapping on space of Lipschitz functions, shows solutions are C^n when vector field is C^n, proves Lipschitz continuity in initial conditions |

## Subdirectories

*(No subdirectories)*

## Search Tags

ode ordinary-differential-equations gronwall-inequality picard-lindelof cauchy-lipschitz existence-uniqueness initial-value-problem lipschitz vector-fields contraction-mapping integral-curves flows derivative-bounds solution-estimates
