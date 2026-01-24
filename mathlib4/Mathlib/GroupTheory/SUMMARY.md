---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory
generated: 2026-01-24T23:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 38
subdirs_count: 19
---

# GroupTheory

## Overview

The `GroupTheory/` directory provides comprehensive formalization of group theory spanning foundational constructions to advanced classification theorems. At its foundation are subgroup-level theories (Subgroup/, Submonoid/, Subsemigroup/ with centers and centralizers), coset theory establishing Lagrange's theorem and quotient constructions (Coset/, QuotientGroup/ with isomorphism theorems), and congruence relations (Congruence/) yielding kernel-range correspondences. The directory encompasses major structural results including the Sylow theorems, Schur-Zassenhaus theorem on coprime complements, nilpotent and solvable group characterizations, p-group theory with fixed point theorems, and the structure theorem for finite abelian groups (FiniteAbelian/ decomposition into prime power cyclic groups with duality results). Free constructions include free groups (FreeGroup/) with Nielsen-Schreier theorem proving subgroups of free groups are free, Church-Rosser reduction systems for normal forms, cyclically reduced words establishing strong torsion-freeness, free abelian groups (Abelianization/) via commutator quotients, and coproducts (Coprod/) providing universal properties for free products. Group actions (GroupAction/) receive extensive treatment through orbit-stabilizer theory, Burnside's lemma, transitivity/primitivity hierarchies, Jordan's theorems on primitive permutation groups, Iwasawa's lemma, block systems, equivariant homomorphisms, domain actions (DomAct/), and sub-mul-actions (SubMulAction/). Permutation groups (Perm/) are formalized via cycle decomposition, cycle types as conjugacy invariants, sign homomorphisms, and maximal subgroup classifications (fragments of O'Nan-Scott). Concrete group families (SpecificGroups/) include cyclic groups with primality-based cyclicity results, dihedral groups (symmetries of regular n-gons), quaternion groups (generalized dicyclic groups), Klein four-groups, Z-groups (cyclic Sylow subgroups), and alternating groups (simplicity of A₅, 3-cycle generation). Coxeter groups (Coxeter/) formalize reflection groups with Coxeter matrices from Lie theory (types A,B,D,E,F,G,H,I), length functions on reduced words, descent sets, braid relations, and inversion sequences. Localization theory covers commutative monoid localization (MonoidLocalization/) with universal properties, Grothendieck group construction, ordered structures, and finiteness preservation, plus non-commutative Ore localization (OreLocalization/) for settings where multiplication doesn't commute. Group extensions (GroupExtension/) are formalized as short exact sequences with splitting theory, sections, conjugacy relations, and connections to semidirect products. Additional topics include element orders (OrderOfElement.lean), torsion theory (Torsion.lean torsion/torsion-free groups), Archimedean ordered groups (Archimedean.lean cyclicity results, ArchimedeanDensely.lean), HNN extensions (HNNExtension.lean with Britton's lemma), commutator theory (Commutator/ with Hall-Witt identity and Three Subgroups Lemma), class equations, double cosets, the Eckmann-Hilton argument, Frattini subgroups, Goursat's lemma, presented groups, transfer homomorphisms, regular wreath products, divisible groups with divisible hulls, and various finiteness conditions. Together, these provide both the theoretical infrastructure for abstract group theory and computational machinery for explicit group-theoretic calculations, serving as foundation for representation theory, Lie theory, and algebraic geometry within mathlib4.

## Key Files

| File | Purpose |
|------|---------|
| Sylow.lean | Sylow theorems: existence of p-subgroups, conjugacy of Sylow subgroups, congruence properties of Sylow counts |
| OrderOfElement.lean | Order of group elements: IsOfFinOrder predicate, orderOf function, properties of finite/infinite order |
| Index.lean | Subgroup index theory and Lagrange's theorem: index definitions, divisibility properties, relative indices |
| Nilpotent.lean | Nilpotent groups: upper/central series, lower central series, nilpotency class, ascending/descending central series |
| Solvable.lean | Solvable groups: derived series, IsSolvable predicate, commutator subgroups |
| PGroup.lean | p-groups: IsPGroup definition, fixed point theorems, prime power order properties |
| FreeAbelianGroup.lean | Free abelian groups as abelianization of free groups, universal property, lift/map functoriality |
| Torsion.lean | Torsion groups and torsion-free groups: Monoid.IsTorsion, CommGroup.torsion subgroup, IsTorsionFree |
| Complement.lean | Subgroup complements: IsComplement, left/right transversals, coprime complement theorem |
| SchurZassenhaus.lean | Schur-Zassenhaus theorem: existence of complements for normal subgroups of coprime index |
| HNNExtension.lean | HNN extensions: construction adjoining stable letter with conjugation relations, Britton's lemma |
| Archimedean.lean | Archimedean ordered groups: cyclicity of subgroups with minimal positive elements, integer subgroups |
| ArchimedeanDensely.lean | Archimedean densely ordered groups (additional properties beyond basic Archimedean) |
| ClassEquation.lean | Class equation relating group order to conjugacy class sizes |
| Commensurable.lean | Commensurability of subgroups (finite index intersection) |
| CommutingProbability.lean | Commuting probability in finite groups |
| CosetCover.lean | Coset covering theory |
| CoprodI.lean | Indexed coproducts of groups |
| DedekindFinite.lean | Dedekind-finite groups (injective endomorphisms are surjective) |
| Divisible.lean | Divisible groups (equation solvability properties) |
| DivisibleHull.lean | Construction of divisible hull for abelian groups |
| DoubleCoset.lean | Double cosets HgK for subgroups H and K |
| EckmannHilton.lean | Eckmann-Hilton argument (two compatible monoid structures yield commutative group) |
| Exponent.lean | Group exponent (LCM of element orders) |
| Finiteness.lean | Finiteness conditions for groups |
| FixedPointFree.lean | Fixed-point-free group actions |
| Frattini.lean | Frattini subgroup (intersection of maximal subgroups) |
| Goursat.lean | Goursat's lemma on subgroups of direct products |
| IndexNormal.lean | Index-related properties for normal subgroups |
| NoncommCoprod.lean | Non-commutative coproduct (free product) of groups |
| NoncommPiCoprod.lean | Non-commutative product over indexed family |
| PresentedGroup.lean | Groups defined by generators and relations |
| PushoutI.lean | Indexed pushouts of groups |
| Rank.lean | Group rank (cardinality of minimal generating set) |
| RegularWreathProduct.lean | Regular wreath product construction |
| Schreier.lean | Schreier's subgroup theorem |
| SemidirectProduct.lean | Semidirect product of groups |
| Transfer.lean | Transfer homomorphism |

## Subdirectories

- [x] `Abelianization/` - Abelianization functor: core construction as quotient by commutator subgroup, universal property via lift operation, functorial map operation, equivalences between abelianizations, finiteness preservation (finite/fintype instances)
- [x] `Commutator/` - Commutator theory: element/subgroup commutators `⁅g₁,g₂⁆`, Three Subgroups Lemma via Hall-Witt identity, normality and characteristic properties, centralizer/center relationships, quotient commutativity characterization, finite generation when commutatorSet is finite, center index bounds
- [x] `Congruence/` - Congruence relations on monoids/groups: equivalence relations preserving operations, quotient constructions with algebraic instances, kernel-congruence correspondence, homomorphism lifting via universal property, isomorphism theorems (quotientKerEquivRange, quotientQuotientEquivQuotient), big operator preservation, opposite congruences
- [x] `Coprod/` - Binary coproduct (free product) `M ∗ N`: construction via congruence on `FreeMonoid (M ⊕ N)`, universal property with lift operation, canonical embeddings (inl/inr), functorial map, swap isomorphism, projections, group structure, associativity and unit laws
- [x] `Coset/` - Coset theory: left/right coset equivalence relations, quotient type `α ⧸ s`, canonical map QuotientGroup.mk, membership characterizations, bijections between left/right cosets and subgroups (leftCosetEquivSubgroup), product decompositions (groupEquivQuotientProdSubgroup), Lagrange's theorem (card_subgroup_dvd_card), fiber equivalences for homomorphisms
- [x] `Coxeter/` - Coxeter groups and systems: Coxeter matrices (symmetric, diagonal=1, off-diagonal≠1) with standard Lie types (A,B,D,E,F,G,H,I), group presentation via simple reflections, length function (minimum word length), reduced words, descent sets (IsLeftDescent/IsRightDescent), braid relations (alternating word theorem), reflections (conjugates of simples), inversions (IsLeftInversion/IsRightInversion), inversion sequences with no-duplicate theorem for reduced words
- [x] `FiniteAbelian/` - Structure theorem for finite abelian groups: decomposition as direct sum of cyclic groups of prime power order (ZMod (p^e)), finitely generated case with free part (ℤ^n) plus torsion, duality results (isomorphism to character group when enough roots of unity exist), both additive and multiplicative versions
- [x] `FreeGroup/` - Free groups: quotient construction via reduction relation on `List (α × Bool)`, Church-Rosser theorem for reduction, universal property (lift), monad structure, concrete/abstract presentations (FreeGroup α vs IsFreeGroup typeclass), Nielsen-Schreier theorem (subgroups of free groups are free via groupoid methods), maximal reduction algorithm computing normal forms, cyclically reduced words proving strong torsion-freeness, basis equivalence theorems, orbit structure under group actions
- [x] `GroupAction/` - Group actions: orbits, stabilizers, fixed points (Defs.lean, Basic.lean), block systems for primitive actions, pretransitive/preprimitive/quasipreprimitive hierarchies, multiple primitivity and k-transitivity, Jordan's theorems on primitive permutation groups (2-pretransitivity criteria with swaps/3-cycles), equivariant homomorphisms (MulActionHom, DistribMulActionHom), orbit-stabilizer theorem, Burnside's lemma, class formula, conjugation action (ConjAct), Iwasawa's lemma, period/support theory, plus subdirectories DomAct/ (domain actions on functions) and SubMulAction/ (invariant subsets, stabilizer/fixing subgroup actions, closures, combinations)
- [x] `GroupExtension/` - Group extensions: short exact sequences `1 → N → E → G → 1`, extension equivalences via commutative diagrams, sections (right inverses to projection), splittings (section homomorphisms), conjugacy relations on splittings, connection between split extensions and semidirect products (any split extension equivalent to semidirect product extension), foundation for group cohomology classification
- [x] `MonoidLocalization/` - Commutative monoid localization: characteristic predicate (IsLocalizationMap) with universal properties (elements of submonoid become units, surjectivity, equality conditions), quotient construction via congruence relations, mk' construction and lift universal homomorphism, away maps (localization at powers of single element), Grothendieck group (localization at top submonoid making all elements invertible), ordered structures on localizations, monoids with zero (triviality when 0 inverted), cardinality bounds (#(Localization S) ≤ #M), finiteness preservation (FG monoid at FG submonoid is FG)
- [x] `Order/` - Minimum order of monoid/group elements: definition as infimum of element orders, equivalence with minimum nontrivial subgroup cardinality, characterization for torsion-free groups (infinite minimum order), explicit computation for ℤ/nℤ (minimum order = smallest prime factor of n)
- [x] `OreLocalization/` - Ore localization for non-commutative monoids: Ore set definition (submonoids satisfying Ore condition allowing common factors/summands to be rearranged), construction of localized monoids `R[S⁻¹]` as quotients with division notation `/ₒ`, monoid/module structure with universal mapping properties, cardinality bounds for localized structures, extension of commutative localization to non-commutative settings
- [x] `Perm/` - Permutation groups (symmetric groups): support theory (elements not fixed, disjointness, swaps), sign/parity homomorphism (`sign : Perm α →* ℤˣ`), finite permutation properties (conjugation, order, support), list-based constructions (formPerm, cyclic permutations from rotations), Fin permutations (decomposition, ranges, sign computations), centralizer subgroups with orbit-stabilizer cardinality, maximal subgroups (intransitive case of O'Nan-Scott), plus subdirectory Cycle/ (cycle decomposition theorem, cycle types as conjugacy invariants, Cauchy's theorem)
- [x] `QuotientGroup/` - Quotient groups: quotient group structure `G/N` for normal subgroup N, canonical quotient homomorphism mk', lifting/mapping homomorphisms through quotients, Noether's isomorphism theorems (first: quotientKerEquivRange, second: quotientInfEquivProdNormalQuotient, third: quotientQuotientEquivQuotient, correspondence/lattice theorem: comapMk'OrderIso), finiteness deduction from kernel-range conditions (fintypeOfKerLeRange, fintypeOfKerOfCodom, fintypeOfDomOfCoker), modular congruence equivalence (additive congruence mod p ↔ equality in quotient by zmultiples p)
- [x] `SpecificGroups/` - Concrete group families: cyclic groups (IsCyclic predicate, generator existence, prime order cyclicity, exponent characterizations, finite simple abelian classification), dihedral groups DihedralGroup n (symmetries of regular n-gons), quaternion groups QuaternionGroup n (generalized dicyclic groups of order 4n), Klein four-groups (IsKleinFour for order 4 exponent 2), Z-groups (cyclic Sylow subgroups with semidirect product characterization), alternating groups (even permutations, index-two characterization, 3-cycle generation, simplicity of A₅), plus subdirectory Alternating/ (centralizers for conjugacy enumeration, Klein four-group in A₄, maximal subgroups)
- [x] `Subgroup/` - Specialized subgroup theory: centers (subgroup of elements commuting with everything, characteristic property, conjugacy class bijections, commutative group equivalence), centralizers (subgroups commuting with given sets, normalizer action on subgroups, homomorphism N(H)→Aut(H) with kernel C(H)), saturated subgroups (g^n ∈ H implies n=0 or g ∈ H, characterization via natural/integer powers, kernel saturation for torsion-free targets), simple groups (IsSimpleGroup for exactly two normal subgroups, preservation under surjective homomorphisms/isomorphisms)
- [x] `Submonoid/` - Submonoid theory: center of monoid (elements commuting with everything, CommMonoid instance, decidability, isomorphisms between centers of isomorphic monoids), centralizer of subset (elements commuting with given subset, decidability, subset ordering), left inverses submonoid (S.leftInv as submonoid of left inverses, MulEquiv between S.leftInv and S when S consists of units, Group instance on IsUnit.submonoid M)
- [x] `Subsemigroup/` - Subsemigroup foundations: center of semigroup as subsemigroup (definition, commutativity instance, membership, decidability), centralizer of subset as subsemigroup (definition, membership, relationships with center, closure properties), foundational constructions extended to submonoids/subgroups/subrings elsewhere

## Search Tags

group-theory sylow lagrange nilpotent solvable p-group torsion free-group free-abelian-group group-action permutation coset quotient-group subgroup complement schur-zassenhaus hnn-extension semidirect-product coproduct archimedean cyclic element-order index abelianization commutator coxeter localization
