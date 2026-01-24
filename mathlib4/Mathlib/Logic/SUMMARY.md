---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic
generated: 2026-01-25T18:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: nightly-testing
status: preliminary
files_count: 13
subdirs_count: 7
---

# Logic

## Overview

The `Logic/` directory provides foundational mathematical logic infrastructure for mathlib4, serving as one of the earliest imports. It contains core logic properties (equality, heterogeneous equality, congruence), fundamental type predicates (emptiness, nonemptiness, uniqueness, denumerability), relation theory (reflexive/transitive/equivalence closures, composition, pairwise relations), and specialized topics including existence uniqueness notation, the hydra game termination proof, and relators for parametricity. These files establish basic logical building blocks used throughout mathlib, with carefully separated decidable vs. classical namespaces and extensive tactic support.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core logic properties and foundational lemmas; one of mathlib's earliest imports; includes equality/HEq congruence theorems, subsingleton instances, the `Fact` typeclass wrapper for elementary propositions, decidability helpers, and basic propositional logic; imports fundamental tactics (Attr.Register, AdaptationNote, Basic) |
| Relation.lean | Comprehensive relation closures and operations: reflexive (`ReflGen`), transitive (`TransGen`), reflexive-transitive (`ReflTransGen`), and equivalence (`EqvGen`) closures for unbundled relations; relation composition (`∘r`), mapping under functions, join operations, and foundational reflexive/symmetric/transitive properties |
| Denumerable.lean | Denumerable (countably infinite) types as typeclass extending Encodable; provides constructive bijection with ℕ via encode/decode functions proven to be inverses; includes `ofNat` for extracting the n-th element and various typeclass instances |
| Hydra.lean | Termination proof for the hydra game: models hydra heads as multisets with well-founded labels, defines `CutExpand` relation for valid moves (cutting head with label `a` grows back finitely many heads with smaller labels), proves game always terminates via well-foundedness using Finsupp.Lex ordering; follows Peter LeFanu Lumsdaine's MathOverflow proof |
| ExistsUnique.lean | Defines `ExistsUnique` (notation `∃!`) for unique existence; includes macro system enforcing single-binder usage to prevent confusion between `∃! (x : α), ∃! (y : β), p x y` and `∃! q : α × β, p q.1 q.2`; supports binder predicates like `∃! x ∈ s, p x`; provides intro/elimination lemmas |
| IsEmpty.lean | `IsEmpty` typeclass expressing types with no elements; includes instances for `Empty`, `PEmpty`, `False`, `Fin 0`, products/sums of empty types; proves emptiness propagates through functions (surjections, compositions); complements `Nonempty` |
| Nonempty.lean | Extra facts about `Nonempty` (defined in Lean core); key lemmas include forall/exists conversions (`Nonempty.forall`, `Nonempty.exists`), `exists_const_iff` relating existentials to nonemptiness, and instances for sigma types, subtypes, products; includes classical `arbitrary` extraction via choice |
| Unique.lean | `Unique` typeclass for types with exactly one term (inhabited subsingleton); implemented as type (not Prop) for good definitional properties of default term; includes `Unique.mk'` constructor, propagation through surjective/injective functions, instances for units and pi types over empty domains |
| Lemmas.lean | Additional basic logic lemmas requiring `tauto` or `split_ifs` tactics; includes iff associativity/commutativity, `dite`/`ite` distributivity laws, and `Prop.forall`/`Prop.exists` characterizations (`(∀ p : Prop, f p) ↔ f True ∧ f False`) |
| Pairwise.lean | Pairwise relations: `Pairwise r` means `r i j` for all `i ≠ j`; connects injectivity to pairwise inequality (`injective_iff_pairwise_ne`); includes monotonicity, composition with injective/surjective functions, and `Set.Pairwise` for relations on set elements |
| Relator.lean | Relator framework for parametricity and function/data relations: `LiftFun` (notation `R ⇒ S`) lifts relations through functions; defines totality properties (LeftTotal, RightTotal, BiTotal) and uniqueness properties (LeftUnique, RightUnique) for establishing relational correspondences |
| OpClass.lean | Typeclass for opposite operations; mechanism for systematically deriving dual/opposite algebraic structures |
| UnivLE.lean | Universe level inequalities and universe lifting utilities; technical infrastructure for managing Lean's universe hierarchy |

## Subdirectories

- [x] `Embedding/` - Embeddings between types (injective functions with additional structure)
- [x] `Encodable/` - Encodable types (countably infinite or finite types with encode/decode to ℕ)
- [ ] `Equiv/` - Type equivalences (bijections) and related constructions
- [ ] `Function/` - Function properties and constructions (composition, inverses, injectivity, surjectivity)
- [ ] `Godel/` - Gödel-related results and encoding
- [ ] `Nontrivial/` - Nontrivial types (at least two distinct elements)
- [ ] `Small/` - Small types (embeddable into a universe level)

## Search Tags

logic foundations basic-logic relations equivalence encodable denumerable unique nonempty empty hydra-game existence-uniqueness pairwise relator fact-typeclass well-founded-relations lean4 mathlib
