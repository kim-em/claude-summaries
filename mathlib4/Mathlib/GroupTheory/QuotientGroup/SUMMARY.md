---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/QuotientGroup
generated: 2026-01-24T08:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# QuotientGroup

## Overview

The `QuotientGroup/` directory provides the foundational theory of quotient groups by normal subgroups. It defines the quotient group structure `G/N` for a normal subgroup `N`, establishes the canonical quotient homomorphism, and proves the fundamental isomorphism theorems (Noether's first, second, third, and fourth/correspondence theorems). The directory includes tools for lifting and mapping homomorphisms through quotients, finiteness deduction for groups via kernel-range conditions, and equivalences between modular congruence relations and quotient group equality.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: quotient group structure, congruence relation construction, canonical homomorphism `mk'`, lift/map operations, kernel characterization, normal subgroup-congruence relation correspondence |
| Basic.lean | Isomorphism theorems and advanced quotient theory: Noether's first isomorphism theorem (`quotientKerEquivRange`), second isomorphism theorem (`quotientInfEquivProdNormalQuotient`), third isomorphism theorem (`quotientQuotientEquivQuotient`), correspondence theorem (`comapMk'OrderIso`), quotient maps for subgroups, equivalences by integer powers |
| Finite.lean | Finiteness deduction: constructive finiteness proofs for groups given finite domain/codomain and kernel-range relationships (`fintypeOfKerLeRange`, `fintypeOfKerOfCodom`, `fintypeOfDomOfCoker`), equivalence between group finiteness and subgroup-quotient finiteness |
| ModEq.lean | Modular congruence equivalence: proves that additive congruence modulo `p` (`a ≡ b [PMOD p]`) is equivalent to equality of cosets in the quotient by `AddSubgroup.zmultiples p` |

## Subdirectories

(none)

## Search Tags

quotient-group normal-subgroup isomorphism-theorem noether first-isomorphism second-isomorphism third-isomorphism correspondence-theorem lattice-theorem kernel-range lift map finiteness congruence modular-arithmetic coset canonical-homomorphism
