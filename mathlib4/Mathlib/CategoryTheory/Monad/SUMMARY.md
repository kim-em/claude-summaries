---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Monad
generated: 2025-12-07T09:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 12
subdirs_count: 0
---

# Monad

## Overview

The `Monad/` directory contains the formalization of categorical monads and comonads in mathlib4. It implements the basic definitions (monads as endofunctors with unit and multiplication, comonads dually), Eilenberg-Moore algebras and coalgebras, the Kleisli category construction, Beck's monadicity and comonadicity theorems, and the fundamental relationship between adjunctions and (co)monads. The directory also establishes the classical result that monads are "just monoids in the category of endofunctors" and provides the bridge between category-theoretic monads and type-theoretic (programmer's) monads in Lean.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `Monad` and `Comonad` structures with unit/counit and multiplication/comultiplication natural transformations |
| Algebra.lean | Eilenberg-Moore algebras and coalgebras for (co)monads with their category structure |
| Adjunction.lean | Correspondence between adjunctions `L ⊣ R` and monads/comonads, including `Adjunction.toMonad` and comparison functors |
| Monadicity.lean | Beck's monadicity theorems showing when a functor is monadic (three versions plus reflexive monadicity theorem) |
| Comonadicity.lean | Dual Beck's comonadicity theorems showing when a functor is comonadic |
| Kleisli.lean | Kleisli category construction for a monad with morphisms `X ⟶ T Y` and dual co-Kleisli category |
| EquivMon.lean | Equivalence `Monad C ≌ Mon (C ⥤ C)` proving monads are monoids in the category of endofunctors |
| Types.lean | Bridge between Lean's type-based `Control.Monad` and category-theoretic `CategoryTheory.Monad` on `Type` |
| Limits.lean | Limits and colimits in categories of (co)algebras, showing forgetful functor creates limits and preserves/creates colimits |
| Coequalizer.lean | Beck coequalizer construction showing any algebra is a reflexive coequalizer (in fact split coequalizer) of free algebras |
| Equalizer.lean | Dual Beck equalizer construction showing any coalgebra is a coreflexive equalizer (split equalizer) of cofree coalgebras |
| Products.lean | Product and coproduct monad examples: `X ⨿ -` (either monad) with equivalence to under category, `X ⨯ -` (writer comonad) with equivalence to over category |

## Subdirectories

(none)

## Search Tags

monad comonad eilenberg-moore algebra coalgebra kleisli adjunction monadicity comonadicity beck-theorem reflexive-coequalizer split-coequalizer monoid-endofunctor category-theory monadic-functor comonadic-functor type-monad lawful-monad comparison-functor descent
