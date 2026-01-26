---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Fin
generated: 2026-01-26T20:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Fin

## Overview

The `Fin/` directory contains order-theoretic structures and properties for finite types `Fin n`, where `Fin n` represents the type of natural numbers less than `n`. The directory establishes `Fin n` as a bounded linear order, provides numerous order embeddings and isomorphisms (cast, succ, rev, succAbove), proves monotonicity results for various `Fin` operations, and includes specialized order isomorphisms between `Fin n` and finsets with strict ordering constraints. This is foundational infrastructure for reasoning about finite ordinals and indexed families throughout Mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Linear order instance for `Fin n`, bounded order structure (with top/bottom), order embeddings (valOrderEmb, succOrderEmb, castLEOrderEmb, castAddOrderEmb, castSuccOrderEmb, addNatOrderEmb, natAddOrderEmb, succAboveOrderEmb), order isomorphisms (orderIsoSubtype, castOrderIso, revOrderIso), monotonicity proofs for cast/succ/addNat/natAdd/predAbove, strictMono characterizations for functions on Fin, uniqueness theorem for order isomorphisms between Fin types |
| Finset.lean | Order isomorphisms from `Fin n` to finsets with ordering constraints: orderIsoSingleton (`Fin 1 ≃o {a}`), orderIsoPair (`Fin 2 ≃o {a, b}` when `a < b`), orderIsoTriple (`Fin 3 ≃o {a, b, c}` when `a < b < c`) |
| SuccAboveOrderIso.lean | Order isomorphism `Fin.succAboveOrderIso` between `Fin (n + 1)` and the complement `{i}ᶜ` as a finset, utilizing the `succAboveOrderEmb` embedding |
| Tuple.lean | Order properties on tuples (functions `Fin n → α`): pi_lex ordering for cons, insertNth operations preserving intervals (insertNth_mem_Icc), monotonicity characterizations for vecCons (strictMono_vecCons, monotone_vecCons), order isomorphisms for tuple decomposition (piFinTwoIso, finTwoArrowIso, consOrderIso, snocOrderIso, insertNthOrderIso), finSuccAboveOrderIso between `Fin n` and `{x : Fin (n+1) // x ≠ p}`, castLEOrderIso for promoting into larger Fin types |

## Subdirectories

*(No subdirectories)*

## Search Tags

Fin finite-type bounded-order linear-order order-embedding order-isomorphism monotone strict-monotone cast succ pred rev succAbove predAbove tuple vector finset complement
