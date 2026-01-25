---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/RamificationInertia
generated: 2026-01-25T19:00:00Z
git_sha: 64c76eabb64d58848cd5a272f58dfa31f3d1e3ea
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# RamificationInertia

## Overview

The `RamificationInertia/` directory contains theory relating to ramification index and inertia degree in field extensions, particularly in the context of Dedekind domains and algebraic number fields. For a prime ideal P in a ring extension S over R lying over a prime p, the ramification index measures the multiplicity of P in the factorization of p, while the inertia degree measures the degree of the residue field extension. This theory is fundamental to understanding how prime ideals decompose in ring extensions, with special treatment of Galois extensions where all primes lying over a given prime behave uniformly.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and theorems for ramification index (multiplicity of prime factorization) and inertia degree (residue field degree), including the fundamental identity `Σ e·f = [Frac(S):Frac(R)]` |
| Galois.lean | Hilbert's ramification theory for Galois extensions: proves uniformity of ramification/inertia across all primes lying over a fixed prime, defines `ramificationIdxIn` and `inertiaDegIn`, establishes `r·e·f = [L:K]` formula |
| Unramified.lean | Connects ramification index to the algebraic predicate `IsUnramifiedAt`, proving equivalence between `e(p) = 1` and unramified extensions for Dedekind domains over characteristic 0 bases |

## Subdirectories

(No subdirectories)

## Search Tags

ramification-index inertia-degree dedekind-domain prime-factorization galois-extension residue-field algebraic-number-theory unramified hilbert-ramification field-extension lie-over prime-ideal
