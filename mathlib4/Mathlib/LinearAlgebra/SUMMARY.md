---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 38
subdirs_count: 34
---

# LinearAlgebra

## Overview

The `LinearAlgebra/` directory contains mathlib4's comprehensive formalization of linear algebra, spanning foundational theory (vector spaces, linear maps, bases, dimension) through advanced topics (tensor products, exterior algebras, Clifford algebras, root systems). Core functionality includes bilinear and multilinear maps, determinants and traces for endomorphisms, matrix theory with extensive linear algebra operations, quotient spaces with projections to complements, and specialized algebraic structures. The directory covers both abstract theory (finite-dimensional spaces, basis-independent constructions, dimension theory) and concrete constructions (product/pi spaces, direct sums, free modules, finitely-supported functions), plus classical groups (general linear, special linear, symplectic, unitary).

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
- [ ] `Span/` - Span of sets in modules
- [ ] `SymmetricAlgebra/` - Symmetric algebras
- [ ] `TensorAlgebra/` - Tensor algebras
- [ ] `TensorPower/` - Tensor powers
- [ ] `TensorProduct/` - Tensor products of modules

## Search Tags

linear-algebra vector-spaces modules linear-maps bilinear-maps determinant trace basis dimension tensor-products quadratic-forms clifford-algebras exterior-algebras projections quotients special-linear-group symplectic-group unitary-group free-modules finite-dimensional interpolation lagrange vandermonde affine-spaces root-systems eigenspaces matrices multilinear alternating dual-spaces sesquilinear-forms
