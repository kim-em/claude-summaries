---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Filter/AtTopBot
generated: 2026-01-26T21:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 19
subdirs_count: 0
---

# AtTopBot

## Overview

The `AtTopBot/` directory provides comprehensive theory for the `atTop` and `atBot` filters, which represent limits as values approach positive and negative infinity respectively in ordered types. The directory includes core definitions of these filters as infima over principal filters, fundamental properties (basis characterizations, membership criteria, NeBot conditions), interaction with Tendsto for convergence, and extensive algebraic infrastructure showing how these filters behave under arithmetic operations in monoids, groups, rings, and fields. Special attention is given to archimedean structures where natural number/integer/rational casts preserve the atTop property, and completeness properties in lattices.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions of atTop and atBot filters as infima of principal filters; membership lemmas (Ici_mem_atTop, Ioi_mem_atTop, etc.); eventually/frequently characterizations; top/bot element special cases; piecewise function convergence for monotone/antitone sequences |
| Basic.lean | Filter basis characterizations (hasAntitoneBasis_atTop, atTop_basis, atTop_basis_Ioi); NeBot instances and characterizations; simp lemmas for membership (mem_atTop_sets, eventually_atTop); frequently_atTop characterizations; map_atTop_eq formula; dual results for atBot |
| Tendsto.lean | Interaction of Tendsto with atTop/atBot: not_tendsto_const theorems; eventually_gt/ge/ne propagation through Tendsto; OrderTop/OrderBot special cases (pure filters); tendsto_atTop/atBot characterizations via Eventually |
| Group.lean | Convergence to ±infinity in ordered commutative groups: tendsto_atTop_mul_left/right theorems showing f*g → ∞ when f bounded and g → ∞; tendsto_atTop/atBot_inv showing g⁻¹ → 0 when g → ∞; versions with/without eventual bounds |
| Monoid.lean | Convergence in ordered monoids: tendsto_atTop/atBot_mul theorems; atTop/atBot_of_mul_isBoundedUnder_le showing bounded*unbounded → unbounded; pow_unbounded_of_one_lt; tendsto_pow_atTop_atTop for bases > 1 |
| Ring.lean | Linear ordered ring theory: const_mul_atTop lemmas for positive constants; add_atTop showing f+g → ∞ when either tends to infinity and other bounded below; sub_atTop/atBot lemmas; specialized results for ℤ and ℕ |
| Field.lean | Linear ordered semifield theory: tendsto_const_mul_atTop_of_pos iff lemmas (r*f → ∞ iff f → ∞ for r > 0); tendsto_inv_atTop_zero (f → ∞ implies f⁻¹ → 0); zpow and rpow convergence; div_atTop lemmas; field-specific arithmetic |
| Archimedean.lean | Archimedean structures: Nat.comap_cast_atTop (cast preserves atTop); tendsto_natCast_atTop_iff (Nat.cast ∘ f → ∞ iff f → ∞); analogous results for Int and Rat casts; tendsto_PNat_val_atTop_atTop; atTop countably generated in archimedean types |
| CompleteLattice.lean | Supremum/infimum interaction with atTop/atBot in complete/conditionally complete lattices: Monotone.ciSup_comp_tendsto_atTop (⨆ a, f(g a) = ⨆ b, f b when g → ∞); dual results for infima and atBot; subsingleton special cases |
| CountablyGenerated.lean | Proves atTop and atBot are countably generated filters in specific settings; basis characterizations using countable index sets; implications for sequential convergence |
| Disjoint.lean | Disjointness results: disjoint_pure_atTop (pure x and atTop are disjoint in types without top); disjoint_atBot_atTop (in types without top or bot); used for non-convergence proofs |
| Prod.lean | Product filter interactions: atTop (α × β) characterized via component-wise atTop; tendsto_fst/snd_atTop lemmas; prod_atTop theorems relating product to individual atTop filters |
| Map.lean | Map and comap operations: map_atTop_eq formulae; comap behavior; image and preimage interaction with atTop/atBot; used for function composition convergence |
| Interval.lean | Interval-specific results for atTop/atBot: membership criteria for interval sets; Icc/Ico/Ioc variants; eventually statements in interval contexts |
| Finite.lean | Finite type behavior: atTop/atBot in finite ordered types reduce to principal filters (pure max/min); characterizations of when these filters are NeBot or trivial |
| Finset.lean | Finset-specific lemmas for atTop/atBot: set membership for finset-related constructions; interaction with finite suprema/infima |
| BigOperators.lean | Big operator interaction: convergence of sums (∑ᶠ), products (∏ᶠ), and other finset operations as index tends to atTop; eventually constant sequences |
| ModEq.lean | Modular arithmetic: atTop preservation under modular equivalence; eventually_modEq results for convergent sequences |
| Floor.lean | Floor/ceiling function interaction with atTop/atBot: tendsto_floor_atTop, tendsto_ceil_atTop showing floor/ceil preserve atTop convergence in archimedean contexts |

## Subdirectories

None.

## Search Tags

atTop atBot filter infinity convergence limit tendsto eventually frequently ordered preorder monotone archimedean group ring field monoid lattice supremum infimum basis NeBot disjoint countably-generated product map comap interval finite modular-arithmetic floor-ceiling big-operators
