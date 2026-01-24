---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/CliffordAlgebra
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 14
subdirs_count: 0
---

# CliffordAlgebra

## Overview

The `CliffordAlgebra/` directory contains the formalization of Clifford algebras—associative algebras constructed from a module equipped with a quadratic form. Clifford algebras are defined as quotients of tensor algebras modulo the relation that identifies `ι m * ι m` with `Q m` for each vector `m`. The directory provides the universal property and lift mechanism, grading structure (ℤ₂-graded superalgebra), conjugation operations (involute, reverse, star), specialized subalgebras (even subalgebra with its own universal property), and important subgroups (Lipschitz group, Pin group, Spin group). It includes isomorphisms to other mathematical structures (complex numbers, quaternions, dual numbers, product algebras), computational tools (foldr/foldl recursion, contraction operations), and category-theoretic interpretations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of Clifford algebra as `RingQuot (CliffordAlgebra.Rel Q)` where `Rel` identifies `ι m * ι m` with `algebraMap R _ (Q m)`, provides canonical linear map `ι Q : M →ₗ[R] CliffordAlgebra Q`, universal property via `lift` (uniquely extending linear maps `f : M → A` satisfying `f m * f m = Q m` to algebra homomorphisms), and foundational algebra instances |
| Grading.lean | ℤ₂-grading structure: defines even/odd submodules `evenOdd Q (0\|1)` as supremum of even/odd powers of `(ι Q).range`, proves graded monoid structure `SetLike.GradedMonoid (evenOdd Q)`, provides graded algebra isomorphism `CliffordAlgebra Q ≃ₐ[R] ⨁ i : ZMod 2, evenOdd Q i`, and establishes that Clifford algebras are superalgebras |
| Even.lean | Even subalgebra universal property: defines `even Q` as the degree-0 component of the grading, introduces `EvenHom` type for bilinear maps satisfying `f m m = Q m` and `f u v * f v w = Q v • f u w`, provides `even.lift` establishing universal property that every such bilinear map corresponds uniquely to an algebra morphism from the even subalgebra, using morphisms-as-output-type trick from "Computing with the universal properties of the Clifford algebra" |
| Conjugation.lean | Antiautomorphisms on Clifford algebras: `involute` (grade involution negating each basis vector `ι m ↦ -ι m`), `reverse` (grade reversion reversing product order), involutivity proofs, commutativity of involute and reverse, and characterizations of evenOdd-membership under these operations |
| Star.lean | Star ring structure defining Clifford conjugation as `star x = reverse (involute x)`, providing involutive star operation compatible with multiplication, proves `star (ι Q m) = -ι Q m`, enabling constructions like unitary groups |
| Fold.lean | Recursive computation via universal property: `foldr` builds linear maps by folding bilinear maps along generators from the right (analogous to `list.foldr`), `foldl` via composition with reverse, induction principles `right_induction` and `left_induction` for building elements generator-by-generator, uses `Module.End R N` as output algebra type |
| Contraction.lean | Contraction operations and isomorphisms: `contractLeft` and `contractRight` contract multivectors by dual vectors `Module.Dual R M`, `changeForm` converts between Clifford algebras of different quadratic forms (difference must be bilinear), `equivExterior` proves module isomorphism to exterior algebra in characteristic ≠ 2 (following Grinberg & Bourbaki) |
| SpinGroup.lean | Pin and Spin groups: `lipschitzGroup Q` as subgroup closure of invertible `ι Q m`, `pinGroup` as infimum of Lipschitz group and unitary group, `spinGroup` as infimum of Pin group and even subalgebra, conjugation action preservation (vectors map to vectors under Lipschitz conjugation), group structures and homomorphisms |
| Equivs.lean | Isomorphisms to classical algebras: `CliffordAlgebraRing.equiv` (any ring as Clifford algebra over zero-dimensional space), `CliffordAlgebraComplex.equiv` (ℂ as Clifford algebra of one-dimensional ℝ-space with `Q (ι Q 1) = -1`, sending complex conjugation to involute), `CliffordAlgebraQuaternion.equiv` (quaternion algebra as Clifford algebra over R × R, sending quaternion conjugation to clifford conjugate), `CliffordAlgebraDualNumber.equiv` (dual numbers R[ε] as Clifford algebra with Q = 0) |
| Prod.lean | Direct sum decomposition: `equivProd` proves `CliffordAlgebra (Q₁.prod Q₂) ≃ₐ[R] (evenOdd Q₁ ᵍ⊗[R] evenOdd Q₂)` showing Clifford algebra of direct sum is graded tensor product of Clifford algebras, with orthogonality conditions for products of mapped elements |
| EvenEquiv.lean | Even subalgebra isomorphisms: `equivEven` shows every Clifford algebra is isomorphic to the even subalgebra of a one-dimension-larger algebra (with quadratic form `Q.prod (-QuadraticMap.sq)`), `evenEquivEvenNeg` shows even subalgebra is isomorphic to even subalgebra of negated quadratic form, provides `toEven`/`ofEven` and `evenToNeg` with behavior on conjugates |
| BaseChange.lean | Scalar extension for Clifford algebras: `equivBaseChange A Q` proves `CliffordAlgebra (Q.baseChange A) ≃ₐ[A] (A ⊗[R] CliffordAlgebra Q)` (complexification and more general base change when 2 is invertible in R), with `toBaseChange`/`ofBaseChange` and compatibility with involute/reverse operations |
| Inversion.lean | Vector inversion formulas: `invertibleιOfInvertible` shows vectors with invertible quadratic form values are themselves invertible, proves `⅟(ι Q m) = ι Q (⅟(Q m) • m)`, conjugation formulas `ι Q a * ι Q b * ⅟(ι Q a) = ι Q ((⅟(Q a) * polar Q a b) • a - b)` showing conjugation preserves the vector subspace |
| CategoryTheory.lean | Category-theoretic interpretation: `QuadraticModuleCat.cliffordAlgebra` functor from quadratic R-modules to R-algebras, sending quadratic module morphisms to algebra homomorphisms via `CliffordAlgebra.map`, functoriality proofs for identity and composition |

## Subdirectories

*(No subdirectories)*

## Search Tags

clifford-algebra quadratic-forms tensor-algebra universal-property grading superalgebra even-subalgebra involute reverse conjugation pin-group spin-group lipschitz-group complexification quaternions dual-numbers contraction foldr recursion base-change isomorphisms category-theory exterior-algebra star-ring
