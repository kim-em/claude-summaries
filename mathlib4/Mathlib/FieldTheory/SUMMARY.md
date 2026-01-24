---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory
generated: 2026-01-24T22:30:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: preliminary
files_count: 31
subdirs_count: 11
---

# FieldTheory

## Overview

The `FieldTheory/` directory contains a comprehensive formalization of field theory, including algebraic extensions, Galois theory, separability, perfect fields, splitting fields, intermediate fields, and minimal polynomials. It covers foundational concepts like field extensions and towers, advanced topics like the Abel-Ruffini theorem on solvability by radicals, and sophisticated theories including Kummer extensions, linear disjointness of fields, and purely inseparable extensions. The directory provides the infrastructure for reasoning about field embeddings, algebraic closures, fixed points under group actions, and relationships between different field extensions.

## Key Files

| File | Purpose |
|------|---------|
| Extension.lean | Extension of field embeddings: proves that F-embeddings of L into K extend to E when minimal polynomials split; defines `Lifts` structure for tracking field embeddings with partial order |
| Tower.lean | Finiteness of scalar towers: proves that in tower F/K/A, if A/F is finite then K/F is finite (under suitable conditions); establishes the tower law for finite-dimensional extensions |
| PrimeField.lean | Prime fields (ℚ in characteristic 0, ZMod p in characteristic p): proves subfield uniqueness and characterizes the smallest subfield of any field |
| AlgebraicClosure.lean | Relative algebraic closure: defines `algebraicClosure F E` as the maximal algebraic subextension (integral closure) of E/F, with preservation under algebra homomorphisms |
| Separable.lean | Separable polynomials and extensions: polynomial is separable iff coprime with its derivative; defines `IsSeparable K x` (minimal polynomial is separable) and `Algebra.IsSeparable K L` (every element is separable) |
| Perfect.lean | Perfect fields and rings: fields where every irreducible polynomial is separable; in prime characteristic p, equivalent to Frobenius map x↦xᵖ being bijective; includes Frobenius automorphism |
| AbelRuffini.lean | Abel-Ruffini theorem: proves if element is solvable by radicals then its minimal polynomial has solvable Galois group; defines `solvableByRad F E` intermediate field |
| KummerExtension.lean | Kummer extensions: for finite extension L/K of dimension n with all n-th roots of unity in K, characterizes cyclic extensions as splitting fields of Xⁿ-a; provides Galois group isomorphism to roots of unity |
| LinearDisjoint.lean | Linearly disjoint fields: two intermediate fields A and L over F are linearly disjoint if linearly independent families over F remain independent over the other field; equivalent characterizations via bases |
| Fixed.lean | Fixed fields under group actions: defines `FixedPoints.subfield G F` for elements fixed by group G acting on field F; basis for Fundamental Theorem of Galois Theory |
| Finiteness.lean | Finiteness conditions for field extensions |
| Cardinality.lean | Cardinality results for field extensions |
| CardinalEmb.lean | Cardinal bounds on field embeddings |
| PolynomialGaloisGroup.lean | Galois groups of polynomials: defines `Polynomial.Gal` as automorphisms of splitting field fixing base field |
| SplittingField.lean | Construction and properties of splitting fields (moved to subdirectory) |
| PrimitiveElement.lean | Primitive element theorem: finite separable extensions are simple extensions |
| IsSepClosed.lean | Separably closed fields: fields with no nontrivial separable algebraic extensions |
| IsPerfectClosure.lean | Perfect closure construction and properties |
| PerfectClosure.lean | Explicit construction of perfect closure in prime characteristic |
| SeparableClosure.lean | Separable closure: maximal separable algebraic extension |
| SeparableDegree.lean | Separable degree of field extensions |
| SeparablyGenerated.lean | Separably generated extensions |
| KummerPolynomial.lean | Polynomials of the form Xⁿ-a and their properties |
| AxGrothendieck.lean | Ax-Grothendieck theorem: injective polynomial maps on algebraically closed fields are surjective |
| AbsoluteGaloisGroup.lean | Absolute Galois group of a field |
| ChevalleyWarning.lean | Chevalley-Warning theorem on zeros of polynomial systems in finite fields |
| Isaacs.lean | Results from Isaacs' work on field theory |
| JacobsonNoether.lean | Jacobson-Noether theorem |
| KrullTopology.lean | Krull topology on Galois groups |
| Laurent.lean | Laurent series and related field constructions |
| NormalizedTrace.lean | Normalized trace maps in field extensions |
| Relrank.lean | Relative rank of field extensions |

## Subdirectories

- [x] `Differential/` - Differential field extensions and Liouville's theorem on integration in finite terms
- [x] `Finite/` - Finite field extensions: basic theory, Galois fields (finite fields as splitting fields), trace, polynomial properties over finite extensions
- [x] `Galois/` - Galois theory: Galois extensions (normal and separable), Galois closures, Galois groups, infinite Galois theory, abelian extensions, fundamental theorem
- [x] `IntermediateField/` - Intermediate fields in field extensions: basic theory, adjoining elements, algebraic intermediate fields
- [ ] `IsAlgClosed/` - Algebraically closed fields: basic properties, algebraic closure construction, classification, spectrum of rings
- [ ] `Minpoly/` - Minimal polynomials: basic theory, minimal polynomials over fields and integrally closed domains, conjugate roots, conjugacy classes
- [ ] `MvRatFunc/` - Multivariate rational functions and their rank properties
- [ ] `Normal/` - Normal extensions: definitions, basic properties, normal closure construction
- [ ] `PurelyInseparable/` - Purely inseparable extensions: basic theory, exponents, relationship to perfect closure, tower properties
- [ ] `RatFunc/` - Rational functions: basic definitions and constructions, degree theory, relationship to polynomials
- [ ] `SplittingField/` - Splitting fields: construction, uniqueness (IsSplittingField), fundamental properties

## Search Tags

field-theory field-extensions galois-theory separable-extensions perfect-fields algebraic-closure splitting-fields intermediate-fields minimal-polynomials normal-extensions purely-inseparable kummer-extensions abel-ruffini galois-groups primitive-element tower-law linear-disjoint fixed-fields frobenius separable-closure finite-fields rational-functions differential-fields algebraically-closed
