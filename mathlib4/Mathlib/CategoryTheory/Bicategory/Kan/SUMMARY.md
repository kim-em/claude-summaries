---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Bicategory/Kan
generated: 2025-12-07T16:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# Kan

## Overview

The `Kan/` directory provides the formalization of Kan extensions and Kan lifts in bicategories. It establishes the universal property characterization (Kan extensions as initial objects in categories of extensions), existence typeclasses, and the relationship between adjunctions and Kan extensions. The directory includes constructors for left Kan extensions/lifts with notation `f⁺ g` and `f₊ g`, absolute Kan extensions that commute with all morphisms, and proves that adjunctions are precisely Kan extensions of the identity.

## Key Files

| File | Purpose |
|------|---------|
| IsKan.lean | Defines `LeftExtension.IsKan` as initial objects in extension categories with universal property (desc, fac, hom_ext) and absolute Kan extensions/lifts that commute with all 1-morphisms |
| HasKan.lean | Existence typeclasses `HasLeftKanExtension` and `HasLeftKanLift` with constructors `lan f g` (notation `f⁺ g`) and `lanLift f g` (notation `f₊ g`), plus commutativity conditions for when extensions commute with morphisms |
| Adjunction.lean | Proves adjunctions are Kan extensions: right adjoints are absolute left Kan extensions of identity, left adjoints are absolute left Kan lifts of identity, with TFAE characterizations of adjoint functors via Kan extensions |

## Subdirectories

None.

## Search Tags

kan-extension kan-lift left-kan-extension right-kan-extension adjunction-as-kan universal-property initial-object absolute-kan commutativity structured-arrow bicategory-limits lan-functor
