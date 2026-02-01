---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Valuation/ValuativeRel
generated: 2026-02-01T23:00:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: preliminary
files_count: 2
subdirs_count: 0
---

# ValuativeRel

## Overview

The `ValuativeRel/` subdirectory develops the theory of valuative relations, which provide an alternative approach to valuation theory by encoding the preorder on a ring arising from an equivalence class of valuations. The `ValuativeRel R` class bundles a relation `x ≤ᵥ y` that mimics the preorder induced by a valuation, completely characterizing the equivalence class of valuations. This includes the canonical valuation taking values in a constructed `ValueGroupWithZero R`, compatibility with existing valuations, rank-one valuations with embeddings into ℝ≥0, discrete valuations with maximal elements, nontriviality conditions, and valuative extensions for algebra maps.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `ValuativeRel R` class defining the relation `x ≤ᵥ y` with axioms ensuring a well-behaved valuation; constructs the canonical `ValueGroupWithZero R` as a quotient; defines `valuation R : Valuation R (ValueGroupWithZero R)` and proves it is compatible; introduces `ValuativeRel.ofValuation` to construct a valuative relation from any valuation; defines rank-one (`IsRankLeOne`), nontrivial (`IsNontrivial`), and discrete (`IsDiscrete`) properties; introduces `ValuativeExtension A B` for algebras with compatible valuative relations |
| Trivial.lean | Defines `trivialRel` valuative relation on domains where all non-zero elements are related (equivalent to the trivial valuation sending all non-zero elements to 1); proves that valuative relations compatible with the trivial valuation equal `trivialRel`; shows that trivial valuative relations have subsingleton units in the value group, are not nontrivial, and are discrete |

## Subdirectories

(No subdirectories)

## Search Tags

valuative-relation preorder valuation equivalence-class value-group-with-zero canonical-valuation compatible rank-one discrete-valuation nontrivial uniformizer trivial-valuation valuative-extension algebra-extension positive-submonoid quotient-construction ordered-monoid linear-order archimedean support-ideal prime-ideal
