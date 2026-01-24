---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Logic
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: nightly-testing
status: complete
files_count: 13
subdirs_count: 7
---

# Logic

## Overview

The `Logic/` directory provides comprehensive foundational infrastructure for mathematical logic in mathlib4, serving as one of the earliest and most fundamental imports. At its core are basic logic properties (equality, heterogeneous equality, congruence) and type predicates (IsEmpty, Nonempty, Unique, Denumerable), along with extensive relation theory covering reflexive/transitive/equivalence closures, composition, and pairwise relations. The directory expands into seven major subdirectories that build the essential type-theoretic machinery used throughout mathlib: `Function/` establishes comprehensive function properties (injectivity, surjectivity, bijectivity) with iteration and semiconjugation theory; `Equiv/` provides the complete theory of type equivalences (bijections) including partial equivalences for manifold charts and specialized equivalences for all standard type constructors; `Embedding/` defines bundled injective functions with set-theoretic operations; `Encodable/` implements constructively countable types with encode/decode functions, lattice operations, and Pi types over finite domains; `Small/` controls universe polymorphism via the Small typeclass for types embeddable into specified universe levels; `Nontrivial/` formalizes types with at least two distinct elements (crucial for algebra and linear algebra); and `Godel/` proves the Beta Function Lemma for encoding sequences in formal arithmetic. The directory also includes specialized topics like existence uniqueness notation (`∃!`), the hydra game termination proof using well-founded relations, relators for parametricity, and universe level management. These files establish the logical and type-theoretic building blocks used pervasively throughout mathlib, with carefully separated decidable vs. classical namespaces and extensive tactic support.

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

- [x] `Embedding/` - Bundled injective functions (`α ↪ β`) with basic operations, conversions to/from equivalences, constructions for standard type constructors, and set-theoretic operations (codomain restriction, image embeddings, subset inclusions)
- [x] `Encodable/` - Constructively countable types with encode/decode functions to ℕ; includes core typeclass, instances for type constructors, ULower for universe lowering, constructive choice functions, lattice operations, and Pi types over finite domains
- [x] `Equiv/` - Comprehensive type equivalence theory: bundled bijections (`α ≃ β`) with explicit inverses, partial equivalences for manifold charts, specialized equivalences for products/sums/options/lists/multisets/finsets/arrays/finite types, permutations, and connections to embeddings/functors; includes Fin subdirectory with finite type conversions and cyclic rotations
- [x] `Function/` - Comprehensive function infrastructure: core properties (injective/surjective/bijective), combinators (composition/swap/update/iteration), specialized predicates (fixed points/semiconjugation/commutativity/dependency), and advanced constructs (heterogeneous n-ary functions/fiber partitions/coequalization)
- [x] `Godel/` - Gödel's Beta Function Lemma proving arithmetically definable encoding/decoding of finite sequences via Chinese Remainder Theorem with coprime moduli; key technical result for Gödel's First Incompleteness Theorem
- [x] `Nontrivial/` - Nontrivial typeclass for types with at least two distinct elements; fundamental for algebra (distinguishing rings where 0 ≠ 1) and linear algebra (positive dimension); includes constructors, instances for type constructors, and relationship with Unique/Subsingleton
- [x] `Small/` - Small typeclass for types embeddable into specified universe levels; provides noncomputable Shrink model with equivShrink equivalence, instances for type constructors, propagation theorems via injective/surjective functions, and specialized instances for lists/sets

## Search Tags

logic foundations basic-logic relations equivalence encodable denumerable unique nonempty empty hydra-game existence-uniqueness pairwise relator fact-typeclass well-founded-relations lean4 mathlib
