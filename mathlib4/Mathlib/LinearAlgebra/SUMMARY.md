---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra
generated: 2026-01-26T00:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 38
subdirs_count: 34
---

# LinearAlgebra

## Overview

The `LinearAlgebra/` directory provides mathlib4's comprehensive and rigorous formalization of linear algebra, developing both abstract theory and computational tools from foundational definitions through sophisticated advanced structures. The treatment begins with core module theory (linear maps, bilinear/multilinear/alternating maps, bases with coordinate representations, linear independence, span operations) and finite-dimensional vector spaces (dimension theory with rank-nullity theorems, dual spaces with perfect pairings, quotient modules with correspondence theorems). Matrix theory bridges concrete computation with abstract algebra through explicit equivalences between matrices and linear maps, comprehensive determinant/trace/rank theory, and classical matrix groups (general linear, special linear, symplectic, unitary).

Advanced algebraic constructions provide the framework for modern applications: tensor products (with universal property, basis constructions, right-exactness, and graded variants for super-algebras), exterior algebras (alternating maps, wedge products, grading by exterior powers), Clifford algebras (quadratic forms, Pin/Spin groups, isomorphisms to quaternions/complex numbers), symmetric algebras (free commutative algebras, polynomial ring isomorphisms), and tensor/exterior/symmetric powers with categorical structures. Specialized geometric theories include affine spaces (affine maps, affine combinations, barycentric coordinates, simplices, Ceva's theorem), projectivization (quotient by scalars, projective subspaces, geometric operations), quadratic forms (polar forms, isometries, Sylvester's law of inertia for reals, canonical forms over complex numbers, categorical monoidal structure), bilinear forms (orthogonality, nondegeneracy, dual bases, dual lattices), and sesquilinear forms (Hermitian forms, star ring structures).

The directory systematically develops dimension theory across algebraic contexts: cardinal-valued rank for general modules, natural-number finrank for finite-dimensional spaces, rank-nullity theorems for division rings and commutative domains (via localization), tower laws for field extensions, dimension formulas for constructions (products, quotients, direct sums, tensor products), Erdős-Kaplansky theorem for infinite-dimensional duals, and strong rank condition ensuring invariant basis number. Eigenspace theory follows Axler's basis-independent approach with generalized eigenspaces, characteristic/minimal polynomial connections, triangularizability over algebraically closed fields, and semisimple/nilpotent endomorphism classifications.

Specialized subdirectories complete the picture: affine geometry with simplices and Commandino's theorem, root systems from Lie theory with Weyl groups and Cartan matrices (including complete 𝔤₂ classification and Geck's semisimple Lie algebra construction), free modules over PIDs with Smith normal form and structure theorems, matrix subdirectories for characteristic polynomials (Cayley-Hamilton via Bar-Natan's elegant proof), determinant theory (Leibniz formula, totally unimodular matrices), GL(n) theory with GL(2) geometric classification, and irreducible matrices with graph-theoretic Perron-Frobenius foundations. The treatment unifies concrete computation (matrix operations, coordinate calculations, explicit bases) with abstract categorical perspectives (universal properties, functoriality, monoidal structures), providing a complete foundation for applications from numerical linear algebra through differential geometry and representation theory.

## Key Files

| File | Purpose |
|------|---------|
| BilinearMap.lean | Bilinear maps framework: semilinear maps `M →ₛₗ[ρ₁₂] N →ₛₗ[σ₁₂] P` with constructors (mk₂, mk₂'), operations (flip, lflip, lcomp, llcomp, compl₂, compr₂), and scalar multiplication as bilinear map (lsmul) |
| Determinant.lean | Determinant theory: basis-dependent family determinants (Basis.det as multilinear map), basis-independent endomorphism determinants (LinearMap.det as multiplicative homomorphism, returns 1 for infinite-dimensional spaces), isomorphism determinants (LinearEquiv.det), and conjugation properties (det_comm, det_conj) |
| Trace.lean | Trace of linear endomorphisms: basis-dependent construction (traceAux) proving basis independence (traceAux_eq), basis-independent trace (LinearMap.trace as linear map, returns 0 for infinite-dimensional spaces), and correspondence with matrix trace |
| Pi.lean | Linear maps with pi-type domains/codomains: pi construction (family of maps to product), single (embedding coordinates), proj (projection from product), diag (diagonal embedding), const (constant maps), and kernel/range relationships |
| Prod.lean | Linear maps on product spaces: projections (fst, snd), injections (inl, inr), product construction (prod from two maps), coproduct (coprod), product maps (prodMap, LinearEquiv.prodMap), and skew products (LinearEquiv.skewProd) |
| Lagrange.lean | Lagrange interpolation: basis divisor polynomials (basisDivisor evaluates to 1 at x, 0 at y when distinct), Lagrange basis polynomials (basis v i evaluates to 1 at v i, 0 at v j for i≠j), interpolation (interpolate v r produces polynomial with specified values at nodes), and uniqueness theorems for polynomial determination |
| Projection.lean | Projection to subspaces: linear projection along complements (linearProjOfIsCompl for decomposition E = p ⊕ q), characterization (f x = x for x∈p, f x = 0 for x∈q), equivalence between complements and projections (isComplEquivProj), and quotient equivalence (quotientEquivOfIsCompl) |
| SpecialLinearGroup.lean | Special linear group of modules: SpecialLinearGroup R V as linear automorphisms with determinant 1 (group structure, coercion to functions, extensionality), dual map action, base change for free finite modules, and equivalence with matrix special linear groups (Matrix.SpecialLinearGroup.toLin_equiv) |
| DFinsupp.lean | Linear algebra on dependent finitely supported functions: module structure, linear maps (lsingle, lmk, lapply, lsum), basis constructions, submodule operations, and support-based properties |
| LinearPMap.lean | Partial linear maps: linear maps defined on submodules (domain, ker, range, comp, sup, graph), Hahn-Banach style extension properties, and adjoint operations |
| AnnihilatingPolynomial.lean | Annihilating polynomials of endomorphisms: minimal conditions for polynomial vanishing, relationship to eigenvalues, and algebraic elements |
| Coevaluation.lean | Coevaluation maps for finite-dimensional spaces: dual pairing constructions and categorical completeness properties |
| Contraction.lean | Tensor contraction: contracting indices in multilinear maps, relationship to traces, and tensor network operations |
| ConvexSpace.lean | Convex spaces as vector space generalization: convex combinations as algebraic operations |
| Countable.lean | Countability properties of vector spaces and submodules |
| CrossProduct.lean | Cross product in three dimensions: vector product with characteristic properties, relationship to determinants, and geometric interpretations |
| FiniteSpan.lean | Finitely spanned submodules and their properties |
| FreeAlgebra.lean | Free algebra as tensor algebra compatibility layer |
| GeneralLinearGroup.lean | Import aggregator for general linear group theory (delegated to GeneralLinearGroup/ subdirectory) |
| Goursat.lean | Goursat's lemma for submodules: intersection and projection relationships |
| InvariantBasisNumber.lean | Invariant basis number property: finite bases of same module have same cardinality, strong rank condition, and basis exchange |
| Isomorphisms.lean | Standard isomorphisms between constructions: prod, pi, and finsupp equivalences |
| JordanChevalley.lean | Jordan-Chevalley decomposition existence and properties |
| LeftExact.lean | Left exactness of Hom functor and related functoriality |
| LinearDisjoint.lean | Linearly disjoint submodules in algebra extensions: independence conditions, tensor product characterizations, and field extension applications |
| Orientation.lean | Orientations on modules: alternating maps determining orientation equivalence classes, basis orientations, and sign conventions |
| PID.lean | Linear algebra over principal ideal domains: structure theorems, torsion modules, and Smith normal form setup |
| PiTensorProduct.lean | Tensor products indexed by types: multilinear construction of ⨂[R] i, M i with universal property, basis from bases, and algebraic operations |
| Ray.lean | Rays in modules: positive scalar multiples, projectivization relationship, and convexity properties |
| Reflection.lean | Reflection linear maps: geometric reflections through hyperplanes, orthogonal reflections, and involutive properties |
| SModEq.lean | Import aggregator for scalar modular equivalence (delegated to SModEq/ subdirectory) |
| Semisimple.lean | Semisimple modules: complete reducibility, Wedderburn-Artin theory connections |
| SesquilinearForm.lean | Import aggregator for sesquilinear forms (delegated to SesquilinearForm/ subdirectory) |
| StdBasis.lean | Standard basis for function spaces and pi types |
| SymplecticGroup.lean | Symplectic group: linear automorphisms preserving symplectic forms, group structure, and classical Sp(2n) |
| Transvection.lean | Transvection matrices: elementary row/column operations, generation of special linear groups, and Gaussian elimination |
| UnitaryGroup.lean | Unitary group: linear automorphisms preserving sesquilinear forms, conjugate-linear structure, and classical U(n) |
| Vandermonde.lean | Vandermonde matrices and determinants: evaluation maps from polynomials, determinant formulas, and interpolation connections |

## Subdirectories

- [x] `AffineSpace/` - Affine spaces and affine combinations
- [x] `Alternating/` - Alternating multilinear maps
- [x] `Basis/` - Basis theory and constructions
- [x] `BilinearForm/` - Bilinear forms on modules
- [x] `Charpoly/` - Characteristic polynomials
- [x] `CliffordAlgebra/` - Clifford algebras from quadratic forms
- [x] `Complex/` - Complex-specific linear algebra
- [x] `Dimension/` - Dimension theory for vector spaces
- [x] `DirectSum/` - Direct sum decompositions
- [x] `Dual/` - Dual spaces and double duals
- [x] `Eigenspace/` - Eigenspaces and eigenvalues
- [x] `ExteriorAlgebra/` - Exterior algebras
- [x] `ExteriorPower/` - Exterior powers
- [x] `FiniteDimensional/` - Finite-dimensional vector spaces
- [x] `Finsupp/` - Finitely supported functions
- [x] `FreeModule/` - Free modules and rank
- [x] `FreeProduct/` - Free products of modules
- [x] `GeneralLinearGroup/` - General linear groups
- [x] `LinearIndependent/` - Linear independence
- [x] `Matrix/` - Matrix theory and operations
- [x] `Multilinear/` - Multilinear maps
- [x] `PerfectPairing/` - Perfect pairings and duality
- [x] `PiTensorProduct/` - Indexed tensor products (subdirectory extension)
- [x] `Projectivization/` - Projectivization of vector spaces
- [x] `QuadraticForm/` - Quadratic forms
- [x] `Quotient/` - Quotient modules
- [x] `RootSystem/` - Root systems and Lie theory
- [x] `SModEq/` - Scalar modular equivalence (subdirectory extension)
- [x] `SesquilinearForm/` - Sesquilinear forms (subdirectory extension)
- [x] `Span/` - Span of sets in modules
- [x] `SymmetricAlgebra/` - Symmetric algebras
- [x] `TensorAlgebra/` - Tensor algebras
- [x] `TensorPower/` - Tensor powers
- [x] `TensorProduct/` - Tensor products of modules

## Search Tags

linear-algebra vector-spaces modules linear-maps bilinear-maps determinant trace basis dimension tensor-products quadratic-forms clifford-algebras exterior-algebras projections quotients special-linear-group symplectic-group unitary-group free-modules finite-dimensional interpolation lagrange vandermonde affine-spaces root-systems eigenspaces matrices multilinear alternating dual-spaces sesquilinear-forms
