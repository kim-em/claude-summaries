---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Fin
generated: 2025-12-09T10:37:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: preliminary
files_count: 10
subdirs_count: 1
---

# Fin

## Overview

The `Fin/` directory provides comprehensive theory for the finite type `Fin n`, representing natural numbers strictly less than `n`. It includes basic operations and properties (coercions, casting, ordering), successor/predecessor operations (`succ`, `pred`, `succAbove`, `predAbove`), embeddings into natural numbers and larger `Fin` types, the reverse/reflection operation, parity properties, pigeonhole principles, vector/matrix notation (`![a, b, c]`), an inductive variant `Fin2`, flag/chain constructions, and specialized tuple operations in a subdirectory.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and lemmas for `Fin n`; includes eliminators (`finZeroElim`), equivalence to subtypes, coercion properties, value injectivity, and fundamental ordering operations |
| SuccPred.lean | Successor and predecessor operations; defines `finCongr` (cast as equivalence), `Fin.succAbove` (embed skipping a point), `Fin.predAbove` (partial inverse), casting operations (`castLE`, `castAdd`, `castSucc`) and their injectivity |
| Embedding.lean | Embeddings of `Fin n`; includes `valEmbedding` (coercion to ℕ), `succEmb`, `castLEEmb`, `castAddEmb`, `castSuccEmb`, `addNatEmb`, `natAddEmb` |
| VecNotation.lean | Matrix and vector notation `![a, b, c]` for `Fin n → α`; defines `vecEmpty` and `vecCons` with macro rules for convenient vector construction syntax |
| Parity.lean | Parity properties in `Fin n`; proves element `k` is even in `Fin n` iff `n` is odd or `Fin.val k` is even; includes `even_succAbove_add_predAbove` used for de Rham cohomology |
| Rev.lean | Reverse operation `Fin.rev : Fin n → Fin n` mapping `i ↦ n - 1 - i`; defines `revPerm` as the antitone involution permutation |
| Pigeonhole.lean | Pigeonhole-like results adapted for `Fin m → Fin n`; includes `le_of_injective`, `le_of_embedding`, `lt_of_injective_of_notMem`, `le_of_surjective` |
| SuccPredOrder.lean | `SuccOrder` and `PredOrder` instances for `Fin n`; makes `Fin n` compatible with successor/predecessor order structures |
| FlagRange.lean | Range of `f : Fin (n + 1) → α` as a maximal chain (flag) when `f₀ = ⊥`, `fₙ = ⊤`, and consecutive elements weakly cover each other |
| Fin2.lean | Inductive type variant of `Fin n` defined inductively rather than as a subtype of ℕ; useful for induction principle and different definitional equalities; includes conversions, addition, embedding, permutations |

## Subdirectories

- [x] `Tuple/` - Tuple operations and theory for `Fin n → α` (vectors with statically-known length)

## Search Tags

fin finite-type bounded-naturals successor predecessor casting embedding vector-notation matrix-notation pigeonhole parity reverse inductive-fin tuple
