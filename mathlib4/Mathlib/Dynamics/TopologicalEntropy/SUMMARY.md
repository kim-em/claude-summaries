---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Dynamics/TopologicalEntropy
generated: 2025-01-24T21:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# TopologicalEntropy

## Overview

This folder formalizes topological entropy for dynamical systems using Bowen-Dinaburg's definitions in the setting of uniform spaces. Topological entropy measures the complexity of a dynamical system by tracking the exponential growth rate of distinguishable orbits. The implementation provides two equivalent approaches: one using dynamical covers (minimal sets whose dynamical balls cover a subset) and one using dynamical nets (maximal sets of pairwise distinguishable orbits). The theory is developed for subsets rather than just invariant sets, avoiding frequent subtype manipulations, with a key theorem (`coverEntropy_restrict`) showing equivalence with the standard restriction-based definition.

## Key Files

| File | Purpose |
|------|---------|
| DynamicalEntourage.lean | Defines `dynEntourage T U n`, the dynamical entourage where points are U-close if their first n iterates under T are U-close; provides basic lemmas about membership, monotonicity, symmetry, and interaction with semiconjugacies |
| CoverEntropy.lean | Implements topological entropy via covers; defines `IsDynCoverOf`, `coverMincard` (minimal cover cardinality), `coverEntropyEntourage`/`coverEntropyInfEntourage` (exponential growth rates), and `coverEntropy`/`coverEntropyInf` (supremum over entourages); proves liminf equals limsup for invariant sets |
| NetEntropy.lean | Implements topological entropy via nets; defines `IsDynNetIn`, `netMaxcard` (maximal net cardinality), `netEntropyEntourage`/`netEntropyInfEntourage`; proves equivalence with cover-based entropy (`coverEntropy_eq_iSup_netEntropyEntourage`) |
| Semiconj.lean | Studies entropy under semiconjugacies; proves `coverEntropy_image_le_of_uniformContinuous` (entropy decreases under uniformly continuous semiconjugacies) and `coverEntropy_restrict` (entropy of restriction to invariant set equals `coverEntropy T F`) |
| Subset.lean | Proves properties of entropy as a function of subsets: monotonicity (`coverEntropy_monotone`), equality with closure (`coverEntropy_closure`), and behavior under unions (`coverEntropy_union` gives max of entropies, extends to finite unions) |

## Subdirectories

(none)

## Search Tags

topological-entropy dynamical-systems bowen-dinaburg uniform-spaces covers nets dynamical-entourage dynamical-balls exponential-growth entropy semiconjugacy invariant-sets closure monotonicity union ergodic-theory complexity
