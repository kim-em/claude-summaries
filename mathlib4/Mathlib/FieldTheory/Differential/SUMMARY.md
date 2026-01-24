---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/Differential
generated: 2026-01-24T23:55:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Differential

## Overview

The `Differential/` directory formalizes differential field theory, focusing on differential field extensions and Liouville's theorem on integration in finite terms. It provides an algebraic treatment of logarithmic derivatives, defines Liouville field extensions (a concept introduced for the formalization), and proves that all finite-dimensional field extensions in characteristic zero are Liouville extensions. The implementation follows Rosenlicht's 1972 work on integration in finite terms.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines logarithmic derivative `logDeriv` algebraically (a′/a); proves properties (multiplication, division, powers, products); constructs differential algebra instances for `AdjoinRoot` and finite-dimensional extensions; proves uniqueness of derivations on finite extensions |
| Liouville.lean | Formalizes Liouville's theorem; defines `IsLiouville` class for field extensions where elements expressible as `v + ∑ cᵢ * logDeriv uᵢ` in the extension can also be expressed in the base field; proves all finite-dimensional extensions in characteristic zero are Liouville using Galois theory and normal closures |

## Subdirectories

(No subdirectories)

## Search Tags

differential-fields liouville-theorem logarithmic-derivative field-extensions differential-algebra derivations integration-in-finite-terms finite-dimensional-extensions galois-theory algebraic-extensions characteristic-zero rosenlicht primitive-element adjoin-root
