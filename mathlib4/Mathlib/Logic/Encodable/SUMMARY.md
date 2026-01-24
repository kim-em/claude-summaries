---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic/Encodable
generated: 2026-01-25T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Encodable

## Overview

The `Encodable/` directory implements encodable (constructively countable) types as a typeclass framework. Encodable types have explicit encode/decode functions to and from natural numbers, with the key property that `decode (encode a) = some a`. Unlike `Denumerable`, `Encodable` includes finite types, though for infinite types the two concepts coincide. The directory provides the core typeclass definition, numerous instances (for products, sums, sigma types, subtypes, quotients, and more), the `ULower` construction for universe lowering, constructive choice functions, and extensions for lattice operations and Pi types over finite domains.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core `Encodable` typeclass definition with encode/decode functions and the `encodek` invariant; includes `decode₂` (failsafe variant ensuring range membership), `ULower` type for universe lowering, constructive choice functions (`choose`, `chooseX`) for decidable predicates, `axiom_of_choice` and `skolem` for encodable types; provides instances for Nat, PUnit, Option, Sum, Bool, Prop, Sigma, Prod, Subtype, Fin, Int, PNat, ULift, PLift; defines `ofEquiv`, `ofLeftInjection`, `ofInj` for deriving encodability; includes `Directed.sequence` for noncomputable monotone/antitone sequences and `encodableQuotient` for quotients by decidable equivalence relations |
| Lattice.lean | Lattice and set operations on encodable types: `iSup_decode₂` and `iUnion_decode₂` relating suprema/unions over decoded naturals to suprema/unions over the encodable type; `iUnion_decode₂_cases` elimination principle; `iUnion_decode₂_disjoint_on` proving pairwise disjointness is preserved through encoding; separated from Basic.lean to minimize imports in foundational files |
| Pi.lean | Encodability for vectors and (dependent) function types: `List.Vector.encodable` for vectors of fixed length n, `finArrow` for `Fin n → α`, `finPi` for dependent functions over `Fin n`, `fintypeArrow` and `fintypePi` for functions with finite domain (wrapped in `Trunc` as encoding is non-unique), and `fintypeArrowOfEncodable` instance when domain is both encodable and finite; uses equivalences with subtypes and sigma types |

## Subdirectories

(none)

## Search Tags

encodable constructive-countability encode-decode countable finite-types denumerable choice-functions ulower universe-lowering lattice-operations pi-types finite-domain vectors sigma-types quotients setoid decidable lean4 mathlib
