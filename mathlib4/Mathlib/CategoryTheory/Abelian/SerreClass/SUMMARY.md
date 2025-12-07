---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Abelian/SerreClass
generated: 2025-12-07T07:39:30Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 0
---

# SerreClass

## Overview

The `SerreClass/` directory provides a formalization of Serre subcategories (also known as Serre classes) in abelian categories. A Serre class is a property of objects that contains the zero object and is closed under subobjects, quotients, and extensions. The directory defines Serre classes, the associated morphism properties (monomorphisms, epimorphisms, and isomorphisms modulo the Serre class), and establishes their relationship to Bousfield localizations. These constructions are fundamental for working with localization and quotient categories in homological algebra.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `IsSerreClass` type class as property containing zero and closed under subobjects, quotients, extensions; proves closure under isomorphisms and characterizes the property via short exact sequences |
| MorphismProperty.lean | Defines `monoModSerre`, `epiModSerre`, and `isoModSerre` morphism properties where f satisfies isoModSerre if kernel(f) and cokernel(f) are in the Serre class; proves multiplicativity, two-out-of-three property, and stability under retracts |
| Bousfield.lean | Connects Serre classes to Bousfield localizations: shows that an exact functor G with fully faithful right adjoint identifies the codomain as the localization with respect to G.kernel.isoModSerre |

## Subdirectories

(none)

## Search Tags

serre-subcategories serre-classes quotient-categories localization bousfield-localization morphism-properties kernel-cokernel-properties two-out-of-three multiplicative short-exact-sequences homological-algebra
