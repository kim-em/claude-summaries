---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Filter
generated: 2026-01-26T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 31
subdirs_count: 4
---

# Filter

## Overview

The `Filter/` directory provides the complete formalization of filter theory in mathematics, serving as the foundation for topology, measure theory, and analysis in Mathlib. Filters abstract two fundamental ideas: limits (sequences, functions at points or infinity) and "eventual" behavior (properties that hold for large enough values, near points, or almost everywhere).

The directory is organized in four conceptual layers: (1) **Core infrastructure** includes the Filter structure as a complete lattice, map/comap operations forming a Galois connection, the monad structure, Tendsto for convergence, and NeBot for non-triviality. (2) **Specialized filters** provides atTop/atBot for limits at infinity in ordered types with extensive arithmetic preservation (monoid/group/ring/field operations, archimedean casts, completeness), the cofinite filter with countable intersection properties, and cardinal-indexed generalizations. (3) **Structural tools** includes filter bases (alternative representations via downward-directed collections), ultrafilters (maximal proper filters characterized by complement membership), and germs (equivalence classes of functions under eventual equality, with comprehensive algebraic structure). (4) **Operations and properties** provides pointwise algebraic operations, boundedness/coboundedness predicates, extrema with respect to filters, lifting operations, products and Pi types, indicator functions, and specialized constructions for rings, partial functions, and intervals.

The four subdirectories extend core theory with critical infrastructure: `AtTopBot/` formalizes limits at infinity with arithmetic preservation theorems for 19 different algebraic contexts; `Bases/` provides the filter basis formalism for convenient filter construction; `Germ/` defines local function behavior via eventual equality quotients with inherited algebraic structure; and `Ultrafilter/` establishes maximal filter theory including the ultrafilter lemma and hyperfilter construction.

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

- [x] `AtTopBot/` - Filters at top and bottom (atTop, atBot) for ordered types with comprehensive algebraic preservation theorems (19 files covering monoids, groups, rings, fields, archimedean structures, complete lattices)
- [x] `Bases/` - Filter basis theory providing alternative filter representations via downward-directed set collections
- [x] `Germ/` - Germs of functions modulo filters (equivalence classes under eventual equality) with inherited algebraic structures (monoid, group, ring, module, lattice)
- [x] `Ultrafilter/` - Ultrafilters (maximal proper filters) with monad structure, ultrafilter lemma, and hyperfilter construction

## Search Tags

filter eventually frequently tendsto limit convergence cofinite atTop atBot map comap principal filter-basis ultrafilter NeBot bounded cobounded pointwise Galois-connection monad lattice extrema neighborhood measure-theory topology analysis
