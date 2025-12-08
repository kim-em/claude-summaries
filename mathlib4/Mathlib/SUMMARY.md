---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib
generated: 2025-12-01T14:30:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: preliminary
files_count: 2
subdirs_count: 33
---

# Mathlib

## Overview

The `Mathlib/` directory is the core of the mathlib4 library, containing the complete formalized mathematics content organized into subject-specific subdirectories. It includes two critical initialization files: `Init.lean` (which defines linter sets and is imported by virtually all Mathlib files) and `Tactic.lean` (which imports all 300+ tactics available in the library). The directory spans the breadth of modern mathematics including algebra, analysis, topology, category theory, number theory, logic, and specialized domains, along with supporting data structures, utilities, and proof tactics.

## Key Files

| File | Purpose |
|------|---------|
| Init.lean | Root initialization file imported by all Mathlib files; defines linter sets (mathlibStandardSet, nightlyRegressionSet, weeklyLintSet) and imports core linters for syntax checking, style enforcement, and code quality |
| Tactic.lean | Comprehensive import file for all 300+ tactics in Mathlib, including decision procedures (linarith, polyrith, ring), automation (simp, continuity, measurability), domain-specific tactics (category_theory, fun_prop, gcongr), and proof tools (tfae, choose, cases) |

## Subdirectories

- [x] `Algebra/` - Theoretical bedrock of mathlib4's algebraic hierarchy: complete stratified development from primitive notation through core hierarchy (Group/Ring/Field/Module/Algebra) to sophisticated frameworks (Lie algebras with classification, homological algebra with derived categories, categorical treatment as abelian categories), encompassing specialized theories (BigOperators, Order, CharP/CharZero, DirectSum, GCDMonoid, divisibility, free constructions, ContinuedFractions, Tropical, Azumaya/BrauerGroup, affine structures, non-associative algebras), systematic multiplicative/additive duality via to_additive, bundled morphisms with complete composition, lattice structures on subobjects with Galois insertions, and categorical infrastructure proving AddCommGrpCat/ModuleCat are abelian categories—foundation for mathlib's algebraic edifice from elementary number theory to algebraic geometry (complete)
- [x] `AlgebraicGeometry/` - Algebraic geometry foundations (schemes, morphisms, sheaves) (complete)
- [x] `AlgebraicTopology/` - Algebraic topology (simplicial sets, homology, fundamental groups) (complete)
- [x] `Analysis/` - Real and complex analysis (calculus, measure theory, functional analysis) (complete)
- [~] `CategoryTheory/` - Category theory framework (categories, functors, limits, adjunctions) (preliminary)
- [x] `Combinatorics/` - Combinatorial mathematics: comprehensive formalization spanning Ramsey theory (Hales-Jewett, Hindman), complete graph theory hierarchies (simple graphs, digraphs, multigraphs, quivers), enumerative techniques (Bell/Catalan numbers, Stirling numbers, integer partitions), extremal methods (Kruskal-Katona, LYM/Sperner, Turán, Szemerédi regularity), additive combinatorics (sumset theory, Roth's theorem), matroid theory, and optimization (complete)
- [x] `Computability/` - Computability theory and recursion theory: complete formalization spanning formal language theory (regular languages, automata, context-free grammars), computability theory (primitive/partial recursive functions, Turing machines, halting problem, Rice's theorem, Turing degrees), and complexity theory (Ackermann function, Akra-Bazzi theorem for divide-and-conquer analysis) (complete)
- [x] `Condensed/` - Condensed mathematics: categorical framework by Clausen-Scholze unifying continuous and discrete mathematics through sheaves on CompHaus with coherent topology; includes condensed sets, condensed modules (abelian category with AB axioms), categorical equivalences with Stonean/Profinite, explicit sheaf conditions, discrete condensed objects (adjunctions, locally constant functors), light condensed objects (universe-efficient variant on LightProfinite with abelian structure, internal projectivity, monoidal/cartesian closed structures), and solid modules (complete)
- [ ] `Control/` - Control theory and system dynamics (pending)
- [ ] `Data/` - Data structures and types (lists, sets, finite types, bit vectors, numeric types) (pending)
- [ ] `Deprecated/` - Deprecated definitions and theorems maintained for compatibility (pending)
- [ ] `Dynamics/` - Dynamical systems theory (pending)
- [ ] `FieldTheory/` - Field theory (extensions, Galois theory, algebraic closures) (pending)
- [ ] `Geometry/` - Geometric structures and theory (pending)
- [ ] `GroupTheory/` - Group theory (subgroups, quotients, group actions, representations) (pending)
- [ ] `InformationTheory/` - Information-theoretic concepts (pending)
- [ ] `Lean/` - Lean-specific metaprogramming utilities and extensions (pending)
- [ ] `LinearAlgebra/` - Linear algebra (vector spaces, matrices, linear maps, tensor products) (pending)
- [ ] `Logic/` - Mathematical logic (propositional logic, first-order logic, model theory basics) (pending)
- [ ] `Mathport/` - Mathport compatibility layer for porting from Lean 3 (pending)
- [ ] `MeasureTheory/` - Measure theory and integration (pending)
- [ ] `ModelTheory/` - Model theory (structures, theories, definability) (pending)
- [ ] `NumberTheory/` - Number theory (primes, divisibility, Diophantine equations, arithmetic functions) (pending)
- [ ] `Order/` - Order theory (partial orders, lattices, well-founded relations, ordinals) (pending)
- [ ] `Probability/` - Probability theory (pending)
- [ ] `RepresentationTheory/` - Representation theory of groups and algebras (pending)
- [ ] `RingTheory/` - Ring theory (ideals, modules, homological algebra, commutative algebra) (pending)
- [ ] `SetTheory/` - Set theory (cardinals, ordinals, ZFC foundations) (pending)
- [ ] `Std/` - Standard library compatibility and extensions (pending)
- [ ] `Tactic/` - All proof tactics and automation tools (186 subdirectories/files) (pending)
- [ ] `Testing/` - Testing utilities and frameworks (pending)
- [ ] `Topology/` - Point-set and algebraic topology (topological spaces, continuity, compactness, separation) (pending)
- [ ] `Util/` - General utility functions and metaprogramming helpers (pending)

## Search Tags

mathlib core mathematics formalized-math lean4 algebra analysis topology category-theory number-theory logic set-theory ring-theory group-theory field-theory linear-algebra measure-theory algebraic-geometry algebraic-topology combinatorics computability model-theory representation-theory order-theory probability tactics linters init
