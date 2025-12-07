---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Preserves/Creates
generated: 2025-12-07T00:00:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# Creates

## Overview

The `Creates/` directory extends the theory of limit creation by functors with classes for finite (co)limits and specific shapes. It defines typeclasses `CreatesFiniteLimits`, `CreatesFiniteColimits`, `CreatesFiniteProducts`, and `CreatesFiniteCoproducts` for functors that create all limits/colimits over finite categories or finite discrete categories, establishes that composition of creating functors creates limits and that creation can be transferred along natural isomorphisms, and proves that functors creating finite limits automatically preserve them. A separate file provides utility lemmas showing that pullbacks and pushouts can be lifted from the target category to the source category when the functor creates those specific limit shapes.

## Key Files

| File | Purpose |
|------|---------|
| Finite.lean | Defines `CreatesFiniteLimits`, `CreatesFiniteColimits`, `CreatesFiniteProducts`, `CreatesFiniteCoproducts` typeclasses with composition, natural isomorphism transfer, and automatic preservation instances |
| Pullbacks.lean | Lemmas `HasPullback.of_createsLimit` and `HasPushout.of_createsColimit` showing that creation of cospan/span limits lifts pullback/pushout existence from target to source |

## Subdirectories

None.

## Search Tags

creates-limits creates-colimits creates-finite-limits creates-finite-colimits creates-finite-products creates-finite-coproducts lift-limits pullback-creation pushout-creation functor-composition natural-isomorphism universe-polymorphism
