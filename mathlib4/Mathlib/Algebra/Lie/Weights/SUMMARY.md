---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Lie/Weights
generated: 2025-12-02T19:45:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 7
subdirs_count: 0
---

# Weights

## Overview

The `Weights/` directory contains the complete theory of weight spaces and root systems for Lie algebras. Weight spaces are simultaneous generalized eigenspaces that decompose Lie modules, analogous to how eigenspaces decompose vector spaces under linear operators. For nilpotent Lie algebras, the binomial theorem ensures weight spaces are Lie submodules. The directory establishes foundational weight space decompositions, proves that weights are linear maps in characteristic zero or for Abelian algebras, develops chain techniques for studying families of roots, provides the complete theory of roots for Lie algebras with non-degenerate Killing forms (including Cartan subalgebra properties, coroots, and root space dimension results), constructs root systems from splitting semisimple Lie algebras, and proves irreducibility of root systems for simple Lie algebras. This is authored primarily by Oliver Nash with significant contributions from Andrew Yang and Janos Wolosz.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core weight space theory: `weightSpace M χ` as intersection of `χ x`-eigenspaces, `genWeightSpaceOf M χ x` as maximal generalized eigenspace, `Weight R L M` typeclass for non-trivial weight spaces, Fitting decomposition via `posFittingCompOf`/`posFittingComp`, fundamental results `iSupIndep_genWeightSpace` (independence), `iSup_genWeightSpace_eq_top` (completeness), `weight_vector_multiplication` for tensor products |
| Cartan.lean | Root spaces relative to Cartan subalgebras: `rootSpace H χ` as weight space of adjoint representation restricted to nilpotent subalgebra `H`, `corootSpace` dual notion, product operations `rootSpaceWeightSpaceProduct` and `rootSpaceProduct`, characterization `zeroRootSubalgebra_eq_iff_is_cartan` relating zero root spaces to Cartan subalgebras |
| Chain.lean | Root/weight chain theory: `α`-chains (families `k • α + β`) for studying root strings, `exists₂_genWeightSpace_smul_add_eq_bot` (existence of trivial chain endpoints), `genWeightSpaceChain` (sum of weight spaces in chain), `trace_toEnd_genWeightSpaceChain_eq_zero` (trace-zero action on chains), `exists_forall_mem_corootSpace_smul_add_eq_zero` (integral linear relations via coroot spaces) |
| Linear.lean | Linearity of weights: `LinearWeights` typeclass encoding that weights are `R`-linear and vanish on derived ideal, `Weight.toLinear` bundles weights as linear maps, instances `instLinearWeightsOfIsLieAbelian` (Abelian case) and `instLinearWeightsOfCharZero` (characteristic zero), `exists_forall_lie_eq_smul` (simultaneous eigenvectors from generalized eigenvectors) |
| Killing.lean | Roots for Lie algebras with non-degenerate Killing forms: `ker_restrict_eq_bot_of_isCartanSubalgebra` (Killing form non-singular on Cartan subalgebras), `instIsLieAbelianOfIsCartanSubalgebra` (Cartan subalgebras are Abelian), `isSemisimple_ad_of_mem_isCartanSubalgebra` (Cartan elements are semisimple over perfect fields), `span_weight_eq_top` (roots span dual space), `coroot` construction, `isCompl_ker_weight_span_coroot` (kernel-coroot decomposition), `finrank_rootSpace_eq_one` (root spaces one-dimensional) |
| RootSystem.lean | Root systems from Lie algebras: chain length theory via `chainLength`, integrality result `apply_coroot_eq_cast` (`β(coroot α) = q - r` for `α`-chain `β - qα ... β + rα`), characterization `rootSpace_zsmul_add_ne_bot_iff` (only chain members are roots of form `β + kα`), multiplicity result `eq_neg_or_eq_of_eq_smul` (`±α` only scalar multiples that are roots), construction `rootSystem` (root system of splitting semisimple Lie algebra with non-degenerate Killing form in characteristic zero) |
| IsSimple.lean | Simple Lie algebras and irreducible root systems: `invtSubmoduleToLieIdeal` (constructs Lie ideal from invariant submodule of dual space), main theorem `instIsIrreducible` (root system of simple Lie algebra with non-degenerate Killing form is irreducible), authored by Janos Wolosz |

## Subdirectories

None.

## Search Tags

weight-space root-space generalized-eigenspace cartan-subalgebra nilpotent-lie-algebra killing-form root-system coroot chain-technique fitting-decomposition linear-weights characteristic-zero abelian semisimple-lie-algebra simple-lie-algebra irreducible-root-system finite-dimensional representation-theory eigenvalue weight-vector root-vector sl2-triple
