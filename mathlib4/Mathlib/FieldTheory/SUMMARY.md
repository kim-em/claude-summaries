---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory
generated: 2026-01-24T23:00:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 31
subdirs_count: 11
---

# FieldTheory

## Overview

The `FieldTheory/` directory provides a comprehensive, modern formalization of field theory spanning foundational to advanced topics. At its core, the directory develops the theory of field extensions: intermediate fields as lattice structures with adjunction operators, finite-dimensional and algebraic extensions with tower laws, and minimal polynomials with their conjugacy classes. Building on this foundation, it establishes the complete machinery of Galois theory through the Fundamental Theorem (both finite and infinite cases via profinite topology), connecting intermediate fields to closed subgroups of Galois groups, with specialized results for abelian extensions and the normal basis theorem.

The directory encompasses several major theoretical frameworks: algebraically closed fields with explicit algebraic closure construction and classification by transcendence degree; splitting fields with existence and uniqueness theorems; separable and purely inseparable extensions with their degree theories and tower multiplicativity; perfect fields characterized by Frobenius bijectivity; and normal extensions with normal closures. Advanced topics include differential field theory with Liouville's theorem on integration in finite terms, the Abel-Ruffini theorem proving the insolubility of the quintic, Kummer theory of cyclic extensions, linear disjointness of fields, and finite field theory with Galois fields and cyclic Galois groups.

The formalization also covers specialized areas: rational functions (univariate and multivariate) as field extensions with degree and valuation theory, fixed fields under group actions, separable closures, perfect closures in prime characteristic, primitive element theorem, Ax-Grothendieck theorem, Chevalley-Warning theorem, and the Krull topology on absolute Galois groups. The directory provides the essential infrastructure for algebraic number theory, algebraic geometry, and modern arithmetic geometry.

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

- [x] `Differential/` - Differential field theory with logarithmic derivatives and Liouville's theorem: proves all finite-dimensional extensions in characteristic zero are Liouville extensions (elements expressible via logarithmic derivatives); follows Rosenlicht's approach to integration in finite terms using Galois theory and normal closures
- [x] `Finite/` - Finite fields theory: cardinality as prime powers, Fermat's little theorem, cyclic unit groups, Frobenius endomorphism, Galois fields GF(p^n) as splitting fields with uniqueness, finite field extensions are Galois with cyclic Galois groups, explicit trace/norm formulas, indicator polynomials
- [x] `Galois/` - Complete Galois theory: Fundamental Theorem of Galois Theory establishing the Galois correspondence between intermediate fields and subgroups for finite extensions; extends to infinite Galois theory via Krull topology with closed subgroups; profinite structure of Galois groups; abelian and cyclic extensions; normal basis theorem; general IsGaloisGroup predicate for group actions
- [x] `IntermediateField/` - Intermediate field infrastructure: SetLike structure with lattice operations, map/comap along algebra homomorphisms, scalar tower mechanics (restrictScalars, extendScalars, lift); adjunction theory with complete lattice structure via Galois insertion; algebraicity and finite-dimensionality propagation; power bases and minimal polynomials in simple extensions
- [x] `IsAlgClosed/` - Algebraically closed fields and algebraic closures: every polynomial splits and has roots, irreducibles have degree 1; explicit construction of algebraic closure as quotient of multivariate polynomial ring; uniqueness up to isomorphism; classification by characteristic and transcendence degree; spectral mapping theorem for polynomials over algebraically closed fields
- [x] `Minpoly/` - Minimal polynomial theory: monic polynomial of smallest degree having element as root; irreducibility over fields, divisibility properties; extension to integrally closed domains with fraction field compatibility; conjugate roots as equivalence relation (IsConjRoot) with conjugacy classes; quotient polynomial minpolyDiv for trace form duality
- [x] `MvRatFunc/` - Multivariate rational function fields: rank (vector space dimension over base field) of FractionRing(MvPolynomial σ F) equals max(#F, #σ, ℵ₀) via transcendental elements and cardinality bounds
- [x] `Normal/` - Normal extensions theory: algebraic extensions where minimal polynomials split completely; equivalent to being splitting field for finite extensions; restriction and lifting of algebra homomorphisms through normal subfields; normal closure construction as supremum of embeddings with uniqueness and closure operator properties; Galois conjugacy via orbit structure
- [x] `PurelyInseparable/` - Purely inseparable extensions: elements outside base have inseparable minimal polynomials; characterizations via powers (x^(q^n) ∈ F); exponent theory with iterated Frobenius maps; relative perfect closure as maximal purely inseparable subextension; tower laws proving separable/inseparable degrees are multiplicative; epimorphism property in category of fields
- [x] `RatFunc/` - Rational function field K(X) as FractionRing(K[X]): field structure with numerator/denominator in coprime form with monic denominators; lifting mechanisms for homomorphisms; polynomial embedding (constants C, indeterminate X) with evaluation; degree theory as intDegree = deg(num) - deg(denom); X-adic valuation for polynomials and rational functions
- [x] `SplittingField/` - Splitting field theory: concrete construction via recursive root adjunction through quotients of multivariate polynomials; IsSplittingField predicate characterizing when extension is generated by roots where polynomial splits; existence and uniqueness up to isomorphism; finite-dimensionality; embeddings into any field that splits the polynomial

## Search Tags

field-theory field-extensions galois-theory separable-extensions perfect-fields algebraic-closure splitting-fields intermediate-fields minimal-polynomials normal-extensions purely-inseparable kummer-extensions abel-ruffini galois-groups primitive-element tower-law linear-disjoint fixed-fields frobenius separable-closure finite-fields rational-functions differential-fields algebraically-closed
