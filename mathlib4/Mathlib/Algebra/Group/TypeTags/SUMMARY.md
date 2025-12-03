---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/TypeTags
generated: 2025-12-01T22:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# TypeTags

## Overview

The `TypeTags/` directory provides type tags for converting between additive and multiplicative algebraic structures. It defines two main type wrappers—`Additive α` (turns multiplicative structures into additive ones) and `Multiplicative α` (turns additive structures into multiplicative ones)—along with comprehensive infrastructure for transferring instances, homomorphisms, and equivalences between these dual presentations. This facility is essential for reusing theorems and constructions across the additive/multiplicative divide without code duplication, leveraging the `@[to_additive]` automation framework.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core type tag definitions (`Additive`, `Multiplicative`) with conversion functions (`ofMul`/`toMul`, `ofAdd`/`toAdd`); comprehensive instances automatically transferring all group-like structures (semigroups, monoids, groups, and their commutative/cancellative variants) between additive and multiplicative presentations; includes operation transfer (`+` ↔ `*`, `-` ↔ `/`, negation ↔ inversion, scalar multiplication ↔ powers) |
| Finite.lean | Finiteness preservation across type tags; proves `Finite`, `Infinite`, and `Fintype` instances are preserved by both `Additive` and `Multiplicative` wrappers, with cardinality-preserving proofs |
| Hom.lean | Homomorphism transport between additive and multiplicative types; provides equivalences like `AddMonoidHom.toMultiplicative : (α →+ β) ≃ (Multiplicative α →* Multiplicative β)` and variants (`toMultiplicativeLeft`, `toMultiplicativeRight`) for mixed situations, with corresponding additive equivalences and extensionality lemmas |

## Subdirectories

(none)

## Search Tags

type-tags additive multiplicative conversion structure-transport homomorphism-transport to-additive dual-structures instance-transfer monoid-hom add-monoid-hom equivalence fintype finite
