---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/Semigrp
generated: 2025-12-04T06:00:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Semigrp

## Overview

The `Semigrp/` directory defines bundled category instances for magmas (types with multiplication) and semigroups (types with associative multiplication), providing both multiplicative and additive variants. It establishes the categories `MagmaCat`, `AddMagmaCat`, `Semigrp`, and `AddSemigrp` with their morphisms (as `MulHom`/`AddHom`), forgetful functors, and isomorphism infrastructure. The implementation closely parallels `Mathlib/Algebra/Category/MonCat/Basic.lean` but for structures without identity elements.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines bundled categories for magmas and semigroups; establishes `MagmaCat` (types with `Mul`), `AddMagmaCat` (types with `Add`), `Semigrp` (types with `Semigroup`), and `AddSemigrp` (types with `AddSemigroup`) with concrete category instances, morphisms as homomorphisms, forgetful functor from `Semigrp` to `MagmaCat`, and bidirectional conversions between `MulEquiv` and categorical isomorphisms |

## Subdirectories

None.

## Search Tags

category-theory semigroups magmas bundled-categories concrete-categories forgetful-functors morphisms homomorphisms multiplicative-equivalences additive-structures to-additive
