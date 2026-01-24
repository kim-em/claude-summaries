---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Function/LpSpace/DomAct
generated: 2026-01-25T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# DomAct

## Overview

The `DomAct/` directory defines and analyzes the action of the domain multiplication group `Mᵈᵐᵃ` on Lp spaces. This action works by precomposing functions with measure-preserving transformations: if `c : Mᵈᵐᵃ` and `f` represents an element of `Lᵖ(α, E)`, then `c • f` is represented by `a ↦ f(c • a)`. The directory establishes that this action preserves all the algebraic and metric structure of Lp spaces (distributivity, isometric property, compatibility with scalar multiplication), and proves continuity of the action in both variables under appropriate topological conditions (R₁ spaces with inner regular measures).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines the SMul action of Mᵈᵐᵃ on Lp spaces via compMeasurePreserving, proves algebraic properties (distributivity over addition, compatibility with subtraction and negation, SMulCommClass instances), establishes isometric properties (norm/distance preservation), and constructs MulAction and DistribMulAction instances |
| Continuous.lean | Proves continuity of the Mᵈᵐᵃ action on Lp spaces: shows the action is continuous in both the group element and the Lp function for 1 ≤ p < ∞ on locally finite inner regular measures over R₁ spaces with continuous group actions |

## Subdirectories

(none)

## Search Tags

domain-action domact lp-space group-action measure-preserving isometric-action smul-invariant continuous-action distribmul-action inner-regular haar-measure topological-group
