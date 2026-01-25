---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Filter
generated: 2026-01-26T21:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 31
subdirs_count: 4
---

# Filter

## Overview

The `Filter/` directory provides comprehensive formalization of filter theory in mathematics. Filters abstract two key ideas: limits (sequences, functions at points or infinity) and "eventual" behavior (things happening for large enough values, near points, or almost everywhere). The directory includes core definitions (Filter structure, principal filters), fundamental operations (map, comap, Tendsto), lattice structure (complete lattice on filters), and extensive theory on filter bases, ultrafilters, convergence, boundedness, pointwise operations, and specialized filters (cofinite, atTop/atBot). This infrastructure forms the foundation for topology, measure theory, and analysis in Mathlib.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core Filter structure definition: sets with univ, upward closure, and intersection; defines principal filters (𝓟), Eventually (∀ᶠ), Frequently (∃ᶠ), Tendsto, IsBounded/IsCobounded; foundational file with minimal dependencies |
| Basic.lean | Complete lattice structure on Filter α via Galois insertion; proves Filter is monadic functor; lattice operations (⊓, ⊔, ⨅, ⨆), NeBot typeclass for non-trivial filters, map/comap Galois connection |
| Map.lean | Push-forward (map) and pull-back (comap) operations on filters; monad structure, Galois connection between map and comap, composition lemmas |
| Tendsto.lean | Convergence with respect to filters: Tendsto definition and basic properties, characterizations via Eventually, composition lemmas |
| Pointwise.lean | Pointwise algebraic operations on filters: addition (f + g), multiplication (f * g), negation (-f), inversion (f⁻¹), scalar operations; makes Filter α a semigroup/monoid when α is |
| Prod.lean | Product filters: filter on α × β from filters on α and β; relationship with neighborhoods and convergence in product spaces |
| Pi.lean | Filters on Pi types (dependent products); component-wise filter operations |
| Cofinite.lean | Cofinite filter (sets with finite complement); proves cofinite = atTop for ℕ; relationship with finite sets |
| CountableInter.lean | Filters closed under countable intersections; CountableInterFilter typeclass |
| CountablyGenerated.lean | Countably generated filters: IsCountablyGenerated typeclass, IsCountableBasis, HasCountableBasis, CountableFilterBasis structure |
| CountableSeparatingOn.lean | Countably separating families of sets for filters |
| CardinalInter.lean | Generalization to cardinal-indexed intersections |
| Cocardinal.lean | Cocardinal of a filter (dual notion to cardinality) |
| Extr.lean | Local extrema with respect to filters: IsMinFilter, IsMaxFilter, IsExtrFilter; versions for sets (IsMinOn, etc.); composition with monotone functions, algebraic operations on extrema |
| IsBounded.lean | Boundedness with respect to filters: IsBounded (eventually bounded by uniform bound), IsCobounded (frequently bounded, doesn't tend to infinity); extensive API for boundedness in ordered types |
| Lift.lean | Lifting operations on filters; functorial properties |
| Curry.lean | Currying for filters (uncurrying filter operations) |
| FilterProduct.lean | Filter products and their properties |
| NAry.lean | N-ary operations on filters |
| Partial.lean | Filters on partial functions (Part type) |
| Interval.lean | Interval filters in ordered types |
| Finite.lean | Finite filters and their properties |
| ENNReal.lean | Filter operations specific to extended non-negative reals |
| EventuallyConst.lean | Eventually constant predicates and functions with respect to filters |
| IndicatorFunction.lean | Indicator functions and filters |
| Ker.lean | Kernel of filter homomorphisms |
| ListTraverse.lean | Traversal of lists with respect to filters |
| Ring.lean | Ring structure on filters |
| SmallSets.lean | Small sets with respect to filters |
| Subsingleton.lean | Subsingleton filters (filters with at most one element) |
| ZeroAndBoundedAtFilter.lean | Filters for functions that are zero or bounded at a filter |

## Subdirectories

- [ ] `AtTopBot/` - Filters at top and bottom (atTop, atBot) for ordered types
- [ ] `Bases/` - Filter bases and their properties
- [ ] `Germ/` - Germs of functions modulo filters (equivalence classes of eventually equal functions)
- [ ] `Ultrafilter/` - Ultrafilters (maximal proper filters) and their properties

## Search Tags

filter eventually frequently tendsto limit convergence cofinite atTop atBot map comap principal filter-basis ultrafilter NeBot bounded cobounded pointwise Galois-connection monad lattice extrema neighborhood measure-theory topology analysis
