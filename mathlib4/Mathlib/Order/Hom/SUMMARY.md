---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Hom
generated: 2026-01-26T08:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# Hom

## Overview

The `Hom/` directory contains the formalization of order homomorphisms (bundled monotone functions) and related morphisms between ordered structures. This includes the core `OrderHom` type (monotone maps), `OrderEmbedding` (order-preserving injections), and `OrderIso` (order isomorphisms), along with specialized variants that preserve additional structure such as lattice operations (`⊔`, `⊓`), completeness operations (`⨆`, `⨅`), and bounded elements (`⊤`, `⊥`). The directory defines both the bundled morphism types and their companion typeclasses following the `FunLike` design pattern.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `OrderHom` (bundled monotone functions `α →o β`), `OrderEmbedding` (`α ↪o β`, order-preserving injections), `OrderIso` (`α ≃o β`, order isomorphisms); companion typeclasses `OrderHomClass`, `OrderIsoClass`; constructions for composition, products, currying, duals, and pi types |
| Bounded.lean | Bounded order homomorphisms: `TopHom` (preserves `⊤`), `BotHom` (preserves `⊥`), `BoundedOrderHom` (monotone maps preserving both `⊤` and `⊥`); companion typeclasses `TopHomClass`, `BotHomClass`, `BoundedOrderHomClass` |
| Lattice.lean | Unbounded lattice homomorphisms: `SupHom` (preserves `⊔`), `InfHom` (preserves `⊓`), `LatticeHom` (preserves both join and meet); companion typeclasses `SupHomClass`, `InfHomClass`, `LatticeHomClass` |
| BoundedLattice.lean | Bounded lattice homomorphisms: `SupBotHom` (preserves `⊔` and `⊥`), `InfTopHom` (preserves `⊓` and `⊤`), `BoundedLatticeHom` (preserves `⊤`, `⊥`, `⊔`, and `⊓`); companion typeclasses |
| CompleteLattice.lean | Complete lattice homomorphisms: `sSupHom` (preserves `⨆`), `sInfHom` (preserves `⨅`), `FrameHom` (preserves `⨆`, `⊓`, and `⊤`), `CompleteLatticeHom` (preserves `⨆` and `⨅`); includes `CompleteLatticeHom.setPreimage` (set preimage as complete lattice homomorphism) |
| Order.lean | Lattice structure on order homomorphisms: if `β` is a complete lattice, then `α →o β` forms a complete lattice with pointwise operations; defines `Max`, `Min`, `Bot`, `Top`, `InfSet`, `SupSet` instances for `α →o β`; includes `iterate_sup_le_sup_iff` for iterated suprema |
| Set.lean | Order homomorphisms and sets: `Set.sumEquiv` (order equivalence between `Set (α ⊕ β)` and `Set α × Set β`), `OrderIso.setCongr` (order isomorphism between equal sets), `OrderEmbedding.orderIso` (order embedding as isomorphism to its range), `StrictMonoOn.orderIso`, `OrderIso.compl` (complement as order isomorphism to dual in Boolean algebras), interval isomorphisms (`OrderIso.Iic`, `OrderIso.Ici`, `OrderIso.Icc`) |
| Lex.lean | Lexicographic order and order isomorphisms: `OrderIso.sumLexIioIci` and `OrderIso.sumLexIicIoi` (linear order isomorphic to lexicographic sum of interval types), `Prod.Lex.prodUnique` and `Prod.Lex.uniqueProd` (lexicographic product with unique type), `Prod.Lex.prodLexAssoc` (associativity), `Prod.Lex.sumLexProdLexDistrib` (left distributivity), `Prod.Lex.prodLexCongr` (congruence) |
| WithTopBot.lean | Adjoining `⊤` and `⊥` to order maps: `WithTop.toDualBotEquiv` (duality between `WithTop αᵒᵈ` and `(WithBot α)ᵒᵈ`), `WithTop.coeOrderHom` and `WithBot.coeOrderHom` (coercion as order embedding), equivalences for types with top/bot elements, mapping operations (`WithTop.map`, `WithBot.map`), and properties of homomorphisms extended to `WithTop`/`WithBot` |

## Subdirectories

(none)

## Search Tags

order-homomorphism monotone-function bundled-morphism OrderHom OrderEmbedding OrderIso lattice-homomorphism SupHom InfHom LatticeHom BoundedOrderHom complete-lattice FrameHom sSupHom sInfHom lexicographic-order WithTop WithBot FunLike typeclasses order-preserving
