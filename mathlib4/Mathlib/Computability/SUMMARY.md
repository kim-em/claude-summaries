---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Computability
generated: 2025-12-08T20:15:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 22
subdirs_count: 1
---

# Computability

## Overview

The `Computability/` directory contains the formalization of computability theory and theoretical computer science foundations in mathlib4. It encompasses three major areas: (1) **formal language theory** including regular languages, automata (DFA, NFA, epsilon-NFA), regular expressions, context-free grammars, and the Myhill-Nerode theorem; (2) **computability theory** including primitive recursive functions, partial recursive functions, Turing machines (TM0, TM1, TM2, Post-Turing machines), encodings, the halting problem, Rice's theorem, Turing degrees, and many-one reductions; and (3) **complexity theory** including the Ackermann function (proven non-primitive-recursive but computable) and the Akra-Bazzi theorem for analyzing divide-and-conquer recurrences. The directory provides a complete progression from basic language definitions through automata theory to universal computation models and undecidability results. The AkraBazzi subdirectory contains a full formalization of the Akra-Bazzi theorem using a sum-based formulation, establishing asymptotic bounds for divide-and-conquer recurrences—a practical tool for algorithm analysis that complements the theoretical foundations in the parent directory.

## Key Files

| File | Purpose |
|------|---------|
| Language.lean | Core definition of formal languages as sets of strings over an alphabet; implements Kleene algebra structure with union, concatenation, and Kleene star; includes Arden's lemma and language reversal operations |
| DFA.lean | Deterministic Finite Automata: state machines with unique transition paths; defines `DFA.accepts` for language recognition and `Language.IsRegular` predicate; proves the pumping lemma for regular languages |
| NFA.lean | Nondeterministic Finite Automata: automata with multiple possible transitions from each state; allows nondeterministic computation paths for language recognition |
| EpsilonNFA.lean | Epsilon-NFA: nondeterministic automata extended with epsilon (empty string) transitions allowing state changes without consuming input |
| RegularExpressions.lean | Formal definition of regular expressions (formal language theory version, not POSIX regex): defines inductively as zero/epsilon/char/plus/comp/star; mirrors Kleene algebra definition |
| ContextFreeGrammar.lean | Context-free grammars for defining context-free languages beyond regular languages |
| MyhillNerode.lean | Myhill-Nerode theorem relating language regularity to equivalence relations on strings |
| Primrec.lean | Primitive recursive functions: least collection of ℕ → ℕ functions closed under projections, composition, zero, successor, and primitive recursion; uses pairing functions and defines `Nat.Primrec` predicate and `Primcodable` type class for encodable types |
| Partrec.lean | Partial recursive functions: extension of primitive recursive functions with unbounded search (μ-operator); represents the class of computable functions |
| PartrecCode.lean | Code representation and evaluation for partial recursive functions; implements a universal partial recursive function |
| Ackermann.lean | Two-argument Ackermann function: fast-growing recursive function proven to be computable but not primitive recursive; proves `not_primrec₂_ack` and `computable₂_ack` |
| TuringMachine.lean | TM2 model: Turing machines with multiple stacks; part of a progression TM0 → TM1 → TM2 with increasing expressiveness; defines `Stmt`, `Cfg`, `Machine`, `step`, `init`, `eval`, and `Supports` for essentially-finite state sets |
| PostTuringMachine.lean | TM0 and TM1 models: foundational Turing machine variants based on Wang B-machines; simpler precursors to the TM2 model |
| Tape.lean | Tape data structure for Turing machines: represents the infinite tape with head position and cells |
| TMConfig.lean | Configuration types for Turing machine instantaneous descriptions (machine state + tape state) |
| TMToPartrec.lean | Equivalence proof: shows Turing machines and partial recursive functions compute the same class of functions |
| TMComputable.lean | Computability via Turing machines: defines what it means for a function to be TM-computable |
| Halting.lean | The halting problem and Rice's theorem: proves undecidability results about Turing machines and partial recursive functions; demonstrates existence of universal partial recursive function |
| Reduce.lean | Many-one reductions between computational problems: formal framework for comparing problem difficulty |
| TuringDegree.lean | Turing degrees: equivalence classes of problems under Turing reducibility; measures relative computability |
| Encoding.lean | Encodings of types into strings over an alphabet: defines `Encoding` and `FinEncoding` structures with encode/decode functions; includes examples like `finEncodingNatBool`, `finEncodingNatΓ'`, `unaryFinEncodingNat`, used for defining TM computability |

## Subdirectories

- [x] `AkraBazzi/` - Akra-Bazzi theorem for analyzing divide-and-conquer recurrences: proves `T(n) ∈ Θ(n^p (1 + ∑_{u=0}^{n-1} g(u) / u^{p+1}))` for recurrences `T(n) = ∑ a_i T(r_i(n)) + g(n)` where `r_i(n) ≈ b_i n`; includes theory of polynomially-growing functions and sum transforms (complete)

## Search Tags

computability-theory recursion-theory turing-machines automata-theory formal-languages regular-languages context-free-grammars DFA NFA epsilon-NFA regular-expressions primitive-recursive partial-recursive computable halting-problem undecidability rice-theorem turing-degrees many-one-reduction kleene-algebra ackermann-function akra-bazzi divide-and-conquer complexity-theory encodings myhill-nerode pumping-lemma universal-machine churchturing-thesis
