---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/RootSystem/GeckConstruction
generated: 2026-01-25T17:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 4
subdirs_count: 0
---

# GeckConstruction

## Overview

The `GeckConstruction/` directory implements Geck's construction of a semisimple Lie algebra from a reduced crystallographic root system with distinguished base. This construction defines the Lie algebra directly on matrices indexed by the base support and root indices, building `sl₂` triples (h, e, f) for each simple root that satisfy Cartan matrix relations. The implementation includes proofs that the construction yields trace-free matrices, has irreducible defining representation, and produces semisimple Lie algebras with trivial radical. This provides one of three standard approaches to constructing Lie algebras from root systems, avoiding the sign ambiguities present in direct bracket constructions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core construction: `sl₂` triples (h, e, f) as matrices on `(b.support ⊕ ι) × (b.support ⊕ ι)`, lieAlgebra and cartanSubalgebra definitions, involution ω for transferring results between e and f, basic properties including Abelian Cartan subalgebra and triangularizability |
| Lemmas.lean | Supporting lemmas for the construction: root membership results (Lemma 2.5 from Geck), chainBotCoeff and chainTopCoeff multiplication formula (Lemma 2.6), IsNotG2 proof for reduced irreducible systems with specific root configurations, detailed case analysis for root chain relationships |
| Relations.lean | `sl₂` triple relations: isSl2Triple instance proving (h, e, f) satisfy standard relations, interaction lemmas between different triples (lie_h_e, lie_h_f for Cartan matrix scaling, lie_e_f_ne proving commutativity for distinct simple roots), follows Lemmas 3.3-3.5 from Geck |
| Semisimple.lean | Proof that Geck construction yields semisimple Lie algebras: nilpotency of e and f matrices, trace_toEnd_eq_zero for trace-free representation (Lemma 4.1), instIsIrreducible for irreducibility of defining representation (Lemma 4.2), instHasTrivialRadical proving semisimplicity (Lemma 4.3) |

## Subdirectories

*(No subdirectories)*

## Search Tags

lie-algebras geck-construction semisimple root-systems sl2-triples cartan-subalgebra matrix-algebras crystallographic reduced-root-systems irreducible nilpotent trace-free representations weight-spaces chain-coefficients root-pairings
