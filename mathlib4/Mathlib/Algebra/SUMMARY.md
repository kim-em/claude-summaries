---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra
generated: 2025-12-01T14:30:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: preliminary
files_count: 32
subdirs_count: 46
---

# Algebra

## Overview

The `Algebra/` directory contains the foundations of algebraic structures in mathlib4, organized hierarchically from basic to complex structures. It implements the core algebraic hierarchy (notation → groups → groups-with-zero → rings → fields) and extends it with advanced constructions including quaternions, polynomials, free algebras, homological algebra, and specialized algebraic systems. The directory contains both the fundamental type class definitions that define algebraic structures and substantial theory development for specific algebraic objects like continued fractions, graded monoids, and Lie algebras.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Documents the algebraic hierarchy structure and folder organization (notation → group → group-with-zero → ring → field) |
| HierarchyDesign.lean | Library note documenting design principles for extending the algebraic hierarchy, explaining when to introduce new typeclasses and trade-offs between extension vs mixin approaches |
| Quaternion.lean | Defines quaternion algebras `ℍ[R, a, b, c]` and standard quaternions `ℍ[R]` over commutative rings, with ring/star-ring/algebra structures and division ring structure for ordered fields |
| Free.lean | Free algebraic constructions: free magmas, free semigroups, and their universal properties expressing adjointness |
| GradedMonoid.lean | Additively-graded multiplicative structures over sigma types where `(*) : A i → A j → A (i + j)` |
| RingQuot.lean | Direct construction of quotients of semirings by arbitrary relations via ideal generation, with universal properties |
| Polynomial.lean | Entry point for univariate polynomial theory (46 files/subdirs) |
| MvPolynomial/ | Multivariate polynomial theory |
| FreeAlgebra.lean | Free algebra construction over a commutative semiring with universal property |
| DualNumber.lean | Dual numbers (automatic differentiation, jet spaces) |
| Quaternion.lean | Quaternion algebras and Hamilton's quaternions |
| QuaternionBasis.lean | Quaternion basis theory |
| CubicDiscriminant.lean | Discriminant theory for cubic polynomials |
| QuadraticDiscriminant.lean | Discriminant theory for quadratic forms |
| Quandle.lean | Quandles and racks (self-distributive algebraic structures from knot theory) |
| LinearRecurrence.lean | Linear recurrence relations |
| ModEq.lean | Modular arithmetic and congruences |
| GeomSum.lean | Geometric sum formulas |
| Exact.lean | Exact sequences in algebra |
| FiveLemma.lean | The five lemma from homological algebra |
| Symmetrized.lean | Symmetrization operations on algebraic structures |
| TrivSqZeroExt.lean | Trivial square-zero extensions |
| IsPrimePow.lean | Prime power characterization |
| NeZero.lean | Non-zero type class for constants |
| AlgebraicCard.lean | Algebraic cardinality theory |
| Opposites.lean | Opposite algebras and rings |
| Quotient.lean | General quotient constructions for algebraic structures |
| PEmptyInstances.lean | Algebraic instances for the empty type |
| Expr.lean | Expression manipulation for algebra |
| Notation.lean | Entry point for algebraic notation definitions |

## Subdirectories

- [x] `Notation/` - Basic algebraic notation and symbols (complete)
- [x] `Group/` - Semigroups, monoids, groups (52 files/subdirs) - foundational layer (complete)
- [x] `GroupWithZero/` - Monoids/groups with zero adjoined (36 files/subdirs) (complete)
- [x] `Ring/` - Additive groups with one, semirings, rings (55 files/subdirs) (complete)
- [x] `Field/` - Division rings and fields: fundamental type classes (`DivisionSemiring`, `DivisionRing`, `Semifield`, `Field`), rich theory of division arithmetic, rational casting, geometric series, periodic functions, instance transfer, conjugation actions, and bundled subfield structures (complete)
- [x] `Algebra/` - Algebra structures over rings (26 files/subdirs) (complete)
- [x] `Module/` - Modules over rings: comprehensive theory of semimodules and modules with `Module R M` typeclass, congruences and quotients, linear equivalences and automorphisms, linear maps and endomorphism rings, submodules with complete lattice structure, localization at multiplicative sets, presentations by generators/relations, torsion theory, and ℤ-lattices in normed spaces (complete)
- [x] `Polynomial/` - Univariate polynomial theory (41 files, 3 subdirs): `R[X]` structure wrapping `AddMonoidAlgebra R ℕ`, comprehensive theory including degree/coefficients with leading/trailing variants, evaluation as ring homomorphisms with irreducibility preservation, formal and Hasse derivatives, division algorithms with Euclidean domain structure, roots with multiplicities and factorization, polynomial module structures, and advanced topics (Laurent polynomials, Taylor expansion, Descartes' rule of signs) (complete)
- [x] `MvPolynomial/` - Multivariate polynomial theory: `MvPolynomial σ R` represents `R[X_i : i ∈ σ]` with arbitrary variable type, built on `AddMonoidAlgebra`, provides evaluation/renaming, degree analysis (`degrees`, `degreeOf`, `totalDegree`), equivalences, monadic operations, derivations/partial derivatives, monomial division, and Schwartz-Zippel lemma (complete)
- [x] `MonoidAlgebra/` - Monoid algebras and group rings: `MonoidAlgebra R M := M →₀ R` construction with convolution product, comprehensive algebraic structure (semiring/ring/algebra instances), support analysis, degree theory (supDegree/infDegree), internal grading structure, division by monomials (divOf/modOf), no zero divisors under UniqueProds condition, and conversions to DirectSum (complete)
- [x] `FreeMonoid/` - Free monoid construction over arbitrary types: `FreeMonoid α` as synonym for `List α` with concatenation multiplication, universal property `lift : (α → M) ≃ (FreeMonoid α →* M)`, embedding `of : α → FreeMonoid α`, operations (length, membership, map, reverse), counting homomorphisms, finite symbol sets, and `TwoUniqueProds` property for factorization uniqueness (complete)
- [x] `FreeAbelianGroup/` - Canonical isomorphism `FreeAbelianGroup X ≃+ (X →₀ ℤ)` with transported support/coefficient notions and `TwoUniqueSums` property (complete)
- [x] `FreeAlgebra/` - Cardinality theory for free algebras: proves `#(FreeAlgebra R X) = lift #R ⊔ lift #X ⊔ ℵ₀` for nontrivial R and nonempty X, with specialized results for empty generators and subsingleton base rings, and bounds for `Algebra.adjoin` (complete)
- [x] `BigOperators/` - Big sum and product operations: complete infrastructure for finite sums (`∑`) and products (`∏`) built on three-layer hierarchy (List → Multiset → Finset) for commutative monoids, extended to rings (distributivity, products-of-sums, binomial formulas), groups with zero (zero-propagation, scalar actions), and finitely-supported functions, plus 15 specialized files covering variant notations (finprod/finsum), expectations, type-specific operations (Fin/Option/Pi/intervals), and connections to modular arithmetic, summation by parts, and structures with top/bottom elements (complete)
- [x] `Order/` - Ordered algebraic structures synthesizing algebra and order theory: bundled/unbundled typeclasses for ordered groups/rings/monoids/modules/fields with fine-grained monotonicity control, Hahn embedding theorem, Cauchy completion construction, floor/ceiling functions, archimedean theory, classical inequalities (Bernoulli, Cauchy-Schwarz, Chebyshev, rearrangement), Kleene algebras, quantales, absolute values, interval arithmetic, and nonnegative/positive subtype theories (complete)
- [x] `Star/` - Star algebras and involution operations: core typeclasses (`InvolutiveStar`, `StarMul`, `StarRing`, `StarModule`) defining structures with antiautomorphic star operation, theory of self-adjoint/unitary/normal elements, star-preserving morphisms and substructures, CHSH/Tsirelson inequalities, and algebraic foundations for C*-algebras and quantum mechanics (complete)
- [x] `Lie/` - Lie algebras and Lie modules: foundational definitions (`LieRing`, `LieAlgebra`, `LieModule`) with Jacobi identity and Leibniz rule, comprehensive theory (subalgebras, ideals, quotients, representation theory), classification theory (nilpotent/solvable/semisimple via lower central and derived series), major theorems (Engel, Lie, Cartan subalgebra existence and properties), classical Lie algebras (sl/sp/so), sl₂ representation theory, Killing/trace forms, derivations (all inner for Killing algebras), weight space decompositions with root systems for semisimple algebras, and irreducibility results for simple Lie algebras (complete)
- [x] `Homology/` - Homological algebra: complete framework building from short complexes (three-object diagrams with dual homology data, exactness, snake lemma) to general homological complexes with arbitrary index types, homotopy category (quotient by homotopy with triangulated structure via mapping cones), derived category (localization at quasi-isomorphisms with shift sequences, t-structure, Ext groups), complex shape embeddings (extension/restriction/truncation functors), functorial resolutions (projective resolutions via iterative kernels), and model category factorizations (CM5b axiom for derived functor applications) (complete)
- [x] `Category/` - Comprehensive categorical treatment of algebraic structures: bundled categories for groups, monoids, rings, modules, algebras, bialgebras, coalgebras, Hopf algebras with complete infrastructure (forgetful functors, all limits/colimits, adjunctions, monoidal structures via tensor products), major results (AddCommGrpCat and ModuleCat as abelian categories with Grothendieck AB axioms, ℤ-modules ≃ abelian groups, essential smallness of FG categories, enough injectives/projectives), and specialized theories (presheaves/sheaves of modules, topological modules, continuous cohomology, Kähler differentials for algebraic geometry) (complete)
- [x] `CharP/` - Characteristic p theory: `CharP R p` typeclass for rings where `ℕ → R` kernel is generated by `p`, `ringChar`/`ExpChar` functions, Frobenius endomorphism `x ↦ x^p`, binomial formulas for prime powers, characteristic preservation through homomorphisms/quotients/products, characteristic-cardinality relationships, mixed vs equal characteristic theory, and specialized results for characteristic 2 rings (complete)
- [x] `CharZero/` - Characteristic zero theory: `CharZero R` typeclass requiring injective `ℕ → R` cast (stronger than `CharP R 0`), fundamental cast injectivity lemmas, proof that characteristic zero structures are infinite, quotient theory for scalar multiples in cyclic subgroups of division rings, and transport of characteristic zero property across injective additive monoid homomorphisms (complete)
- [x] `DirectSum/` - Direct sum constructions for algebraic structures: basic definition `DirectSum ι β := Π₀ i, β i` with `⨁` notation, module theory with universal properties, additively-graded rings/algebras where `A i → A j → A (i + j)`, internal grading connecting subobjects to carrier types, constructive decomposition theory with canonical equivalences, linear maps with block-diagonal matrices, equivalence with finsupp, additive characters, and orthogonal idempotent decompositions (complete)
- [x] `GCDMonoid/` - Monoids with normalization functions, GCD, and LCM: core typeclasses (`NormalizationMonoid`, `GCDMonoid`, `NormalizedGCDMonoid`) defining canonical representatives and GCD/LCM operations, concrete instances for ℕ/ℤ/PUnit, operations on multisets/finsets, and proof that GCD domains are integrally closed (complete)
- [x] `EuclideanDomain/` - Euclidean domains: nontrivial commutative rings with division/remainder satisfying `b * (a / b) + a % b = a` and well-founded relation ensuring GCD termination, generalized to transfinite case with arbitrary well-ordered degree sets, includes GCD/LCM algorithms, Bézout's lemma, extended Euclidean algorithm, and canonical instances for fields and integers (complete)
- [x] `Divisibility/` - Divisibility theory: foundational divisibility relations in algebraic structures from semigroups to commutative monoids, defines `a ∣ b ↔ ∃ c, b = a * c`, primal elements and decomposition monoids, divisibility in products/homomorphisms/finite types, units dividing everything with invariance under unit multiplication, and relatively prime elements where common divisors are units (complete)
- [x] `NoZeroSMulDivisors/` - Scalar multiplication without zero divisors: `NoZeroSMulDivisors R M` typeclass ensuring `c • x = 0 ↔ c = 0 ∨ x = 0`, heterogeneous generalization of `NoZeroDivisors` providing characteristic-independent torsion-freeness, with scalar injectivity lemmas, characteristic zero theory, equivalence to `IsAddTorsionFree` for ℕ/ℤ scalars, and instances for products/functions (complete)
- [x] `Prime/` - Prime elements in commutative monoids with zero: `Prime p` predicate requiring nonzero, non-unit, and `p ∣ a * b → p ∣ a ∨ p ∣ b`, equivalence with irreducible elements in decomposition monoids, power divisibility theory, and homomorphism transport (complete)
- [x] `Regular/` - Regular elements: core theory of left/right/fully regular elements where multiplication is injective, `IsSMulRegular` for module-theoretic generalization, closure under products/powers/units, behavior under `MulOpposite`/product types/Pi types/universe lifting, and proof that `0` is regular iff structure is trivial (complete)
- [x] `Central/` - Central algebras over commutative rings: `Algebra.IsCentral K D` typeclass where center equals base ring image, core results on centrality preservation under isomorphisms/opposite algebras/base field extensions, instances for matrix algebras and endomorphism algebras on free modules, and tensor product decomposition theorems (complete)
- [x] `ContinuedFractions/` - Comprehensive continued fraction theory covering theoretical foundations (GCF/SCF/RCF types, dual convergent computation methods via `convs`/`convs'`, recurrence relations, determinant formulas, equivalence proofs) and practical computation (standard floor/fractional decomposition algorithm, correctness/convergence with error bounds `|v - Aₙ/Bₙ| ≤ 1/(Bₙ * Bₙ₊₁)`, Fibonacci lower bounds on denominators, and termination characterization for rationals) (complete)
- [x] `AddTorsor/` - Additive torsors (principal homogeneous spaces): `AddTorsor G P` typeclass providing transitive and free additive group actions with `+ᵥ` (vadd) and `-ᵥ` (vsub) operations, complete cancellation theory, point reflection equivalences, and instances for products and Pi types (complete)
- [x] `AddConstMap/` - Bundled maps and equivalences semiconjugating shifts: `f (x + a) = f x + b` property with comprehensive theory for circle lifts, monotonicity on fundamental intervals, group structure on automorphisms, and floor ring constructions (complete)
- [x] `AffineMonoid/` - Finitely generated cancellative torsion-free commutative monoids that embed into ℤⁿ, with unique sums/products and irreducible element characterization (complete)
- [x] `Azumaya/` - Azumaya algebras: noncommutative algebras generalizing central simple algebras over commutative rings, defined via tensor product isomorphism with endomorphisms, with instances for the base ring itself and matrix algebras (complete)
- [x] `BrauerGroup/` - Foundational definitions for Brauer group of a field: `CSA K` structure for finite-dimensional central simple algebras, `IsBrauerEquivalent` relation where algebras are equivalent if their matrix rings are isomorphic, proof that Brauer equivalence is an equivalence relation, and `BrauerGroup K` as the quotient type classifying central simple algebras up to Morita equivalence (complete)
- [~] `Colimit/` - Direct limits (colimits) of algebraic structures in directed systems: general DirectLimit construction for any algebraic structure with explicit equivalence relations, specialized quotient-based constructions for modules/abelian groups/rings built on DirectSum/FreeCommRing, proof that modules are direct limits of finitely generated submodules, tensor product preservation results (preliminary)
- [ ] `Jordan/` - Jordan algebras (3 files/subdirs) (pending)
- [ ] `NonAssoc/` - Non-associative algebras (4 files/subdirs) (pending)
- [ ] `PresentedMonoid/` - Monoids by generators and relations (3 files/subdirs) (pending)
- [ ] `QuadraticAlgebra/` - Quadratic algebras (5 files/subdirs) (pending)
- [ ] `SkewMonoidAlgebra/` - Skew monoid algebras (6 files/subdirs) (pending)
- [ ] `SkewPolynomial/` - Skew polynomial rings (3 files/subdirs) (pending)
- [ ] `Squarefree/` - Squarefree elements (3 files/subdirs) (pending)
- [ ] `Tropical/` - Tropical algebra (min-plus and max-plus semirings) (5 files/subdirs) (pending)
- [ ] `Vertex/` - Vertex algebras (4 files/subdirs) (pending)
- [ ] `Pointwise/` - Pointwise operations on sets (3 files/subdirs) (pending)

## Search Tags

algebra algebraic-hierarchy groups rings fields modules polynomial quaternion free-algebra graded-monoid homological-algebra lie-algebra star-algebra category-theory characteristic-p gcd-monoid euclidean-domain divisibility continued-fractions azumaya brauer-group tropical-algebra vertex-algebra bigoperators ordered-algebra
