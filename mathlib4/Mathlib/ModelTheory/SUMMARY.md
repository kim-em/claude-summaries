---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/ModelTheory
generated: 2026-01-25T02:22:47Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 23
subdirs_count: 3
---

# ModelTheory

## Overview

The `ModelTheory/` directory contains a comprehensive formalization of first-order model theory, following the style of the Flypitch project (which proved the independence of the continuum hypothesis). It provides the complete infrastructure for first-order languages, structures, theories, and their semantic and syntactic properties, including fundamental results like the Compactness Theorem, Löwenheim-Skolem theorems, and Fraïssé theory. The directory spans from basic definitions of languages and structures through advanced topics like ultraproducts, complete types, definability, and categoricity, with specialized applications to ordered structures, algebraic structures, and arithmetic.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Foundational definitions: first-order languages (functions and relations of each arity), structures (interpretations of language symbols in types), and structure morphisms (Hom/Embedding/Equiv preserving function interpretations and relation interpretations); based on Flypitch project |
| Syntax.lean | First-order syntax: terms (variables and function applications), bounded formulas (using locally nameless representation with de Bruijn levels for bound variables), formulas, sentences, and theories; includes term/formula relabeling, substitution, and language map actions |
| Semantics.lean | Interpretation of syntax in structures: term realization, bounded formula realization, formula realization, sentence realization (M ⊨ φ), and theory models (T ⊨ φ); proves that syntactic operations (relabel, castLE, liftAt, subst) commute with semantic realization |
| Satisfiability.lean | Theory satisfiability and completeness: satisfiability (nonempty models), finite satisfiability, completeness (satisfiable theory deciding each sentence), and κ-categoricity (all models of size κ isomorphic); proves Compactness Theorem (satisfiable iff finitely satisfiable) and Upward Löwenheim-Skolem |
| Substructures.lean | First-order substructures: substructure lattice (CompleteLattice), closure operations, comap/map under homomorphisms, range of homomorphisms, domain/codomain restriction for Hom/Embedding, inclusion embeddings, and partial equivalences between substructures |
| Definability.lean | Definable sets: Set.Definable (sets definable with parameters), Set.Definable₁/Definable₂ (unary/binary specializations), DefinableSet Boolean algebra, Set.TermDefinable (functions expressible as terms); proves definability closed under finite-dimensional projections and term-definable functions closed under composition |
| ElementaryMaps.lean | Elementary embeddings: embeddings preserving formula realization in both directions, elementary diagrams (sentences with parameters satisfied by structure), and Tarski-Vaught Test for checking if embedding is elementary |
| Fraisse.lean | Fraïssé theory: ages of structures (finitely-generated structures embedding into them), Fraïssé classes (hereditary, joint embedding, amalgamation properties), Fraïssé limits (countable ultrahomogeneous structures); proves uniqueness of Fraïssé limits up to isomorphism and characterizes ages of countable structures |
| DirectLimit.lean | Direct limits of first-order structures: constructs direct limit of directed system of first-order embeddings, universal property (lift), and equivalence between limits of isomorphic systems |
| Types.lean | Complete types: type spaces T.CompleteType α (complete types over theory T with variables α implemented as maximal consistent theories in expanded language), typeOf (type of given tuple), realizedTypes (types realized in model); proves type space nonempty iff theory satisfiable and every type realized in some model |
| Order.lean | Ordered structures: Language.order (language with single ≤ relation), IsOrdered (designated order symbol), OrderedStructure (symbol interpreted as actual ≤), theories of preorders/partial orders/linear orders, DLO theory (dense linear orders without endpoints); proves DLO is ℵ₀-categorical and complete, and countable dense linear orders are Fraïssé limits |
| Complexity.lean | Quantifier complexity: atomic formulas (equality or relation symbols applied to terms), quantifier-free formulas (IsQF), prenex normal forms (IsPrenex - quantifiers followed by QF formula), toPrenex construction; proves prenex normal form has same realization as original |
| Encoding.lean | Encodings and cardinality: encodes terms and bounded formulas as lists for computability; proves cardinality bounds: #(L.Term α) ≤ max ℵ₀ #(α ⊕ Σ i, L.Functions i) and #(Σ n, L.BoundedFormula α n) ≤ max ℵ₀ (lift #α + lift L.card) |
| LanguageMap.lean | Language homomorphisms: maps between first-order languages preserving function/relation arities, with actions on terms, formulas, structures, and theories |
| PartialEquiv.lean | Partial equivalences: equivalences between substructures of two structures, used in Fraïssé amalgamation and back-and-forth arguments |
| Equivalence.lean | Formula equivalence: syntactic and semantic equivalence of formulas, with applications to normal forms and formula simplification |
| FinitelyGenerated.lean | Finitely generated structures: structures generated by finite sets, closure under finite generation, used extensively in Fraïssé theory to characterize ages |
| ElementarySubstructures.lean | Elementary substructures: substructures preserving formula satisfaction (not just atomic formulas like regular substructures) |
| Bundled.lean | Bundled structures: packaged first-order structures as objects in a category, enabling categorical reasoning about model-theoretic constructions |
| Graph.lean | Graph structures: interpretation of first-order relational languages as graphs, connecting model theory with graph theory |
| Quotients.lean | Quotient structures: quotients of first-order structures by congruence relations, with induced structure on quotient types |
| Skolem.lean | Skolem functions: Skolemization process adding function symbols witnessing existential formulas, used in Löwenheim-Skolem and completeness proofs |
| Ultraproducts.lean | Ultraproducts: constructions of ultraproducts and ultrapowers of first-order structures via ultrafilters; fundamental in model theory for compactness and saturation |

## Subdirectories

- [x] `Algebra/` - Model theory of algebraic structures (fields, rings)
- [x] `Arithmetic/` - Model theory of arithmetic (Presburger arithmetic)
- [x] `Topology/` - Model theory of topological structures

## Search Tags

model-theory first-order-logic mathematical-logic flypitch structures languages theories satisfaction compactness-theorem lowenheim-skolem fraisse elementary-embeddings definability types ultraproducts prenex-normal-form dlo categoricity complete-types skolemization direct-limits
