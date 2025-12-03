---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Algebra/Hom
generated: 2025-12-01T19:50:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# Hom

## Overview

The `Hom/` directory provides specialized theory for algebra homomorphisms in specific contexts. Currently it contains the equivalence between ring homomorphisms and ℚ-algebra homomorphisms, establishing that for rings with ℚ-algebra structure, every ring homomorphism automatically commutes with the rational scalar action and can be reinterpreted as a ℚ-algebra homomorphism.

## Key Files

| File | Purpose |
|------|---------|
| Rat.lean | Equivalence `RingHom.equivRatAlgHom` showing that for ℚ-algebras, ring homomorphisms and ℚ-algebra homomorphisms are equivalent structures, with conversion functions `toRatAlgHom` and `toRingHom` |

## Subdirectories

None.

## Search Tags

algebra-homomorphism rational-algebra ring-homomorphism equivalence rat-alg-hom algebraMap commutes
