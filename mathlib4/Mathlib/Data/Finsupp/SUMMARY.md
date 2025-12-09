---
source_path: /Users/kim/projects/lean/lean4-2/downstream_releases/mathlib4/Mathlib/Data/Finsupp
generated: 2025-12-09T06:30:00Z
git_sha: 8630639169c28647dbae9f5b0132c77dcbfe2281
git_branch: bump_to_v4.26.0-rc2
status: preliminary
files_count: 27
subdirs_count: 1
---

# Finsupp

## Overview

The `Finsupp/` directory implements finitely supported functions `α →₀ M`, which are functions from `α` to `M` (where `M` has a zero) that are zero everywhere except on a finite set. This fundamental data structure underlies polynomials, multivariate polynomials, monoid algebras, and linear combinations in mathlib4. The directory provides the core definition, basic operations (single, update, erase, mapRange, embDomain), algebraic structure instances, ordering relations (lexicographic, pointwise), conversions to/from related types (DFinsupp, AList, Multiset), and specialized constructions for computational algebra (monomial orders, weights, antidiagonals).

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definition of `Finsupp α M` structure with support, underlying function, and membership proof; establishes notation `α →₀ M` |
| Basic.lean | Miscellaneous operations including graph, mapRange equivalence, mapDomain, comapDomain, filter, frange, and subtype_domain |
| Single.lean | `Finsupp.single a b` - the finsupp nonzero only at one point; includes update and erase operations for point modifications |
| Notation.lean | `fun₀ \| i => a` notation for creating finsupps via `Finsupp.single` and `Finsupp.update`; provides pretty-printing support |
| Order.lean | Pointwise order structures on finsupps; lifts partial orders, lattices, and ordered monoid structures from `α` to `ι →₀ α` |
| Lex.lean | Lexicographic ordering `Finsupp.Lex r s` on finsupps where domain is ordered by `r` and codomain by `s`; type synonym `Lex (α →₀ N)` |
| Weight.lean | Weight function `f.weight w = ∑ (f i) • (w i)` for classifying finsupps by weighted sums; includes degree (total sum) and finiteness results |
| MonomialOrder.lean | Monomial orders for Gröbner basis theory: well-founded orderings on `σ →₀ ℕ` compatible with addition; includes lexicographic example |
| WellFounded.lean | Well-foundedness results for lexicographic and product orders on finsupps; transfers results from DFinsupp |
| ToDFinsupp.lean | Conversions between `Finsupp` and homogeneous `DFinsupp` (dependent finsupp); equivalences `Finsupp.toDFinsupp` and `DFinsupp.toFinsupp` |
| AList.lean | Connections to association lists: `Finsupp.toAList` and `AList.lookupFinsupp` for converting between representations |
| Multiset.lean | Relationship between finsupps and multisets; operations involving multiset-like behavior |
| Antidiagonal.lean | Antidiagonal construction for finsupps; used in convolution and polynomial multiplication |
| BigOperators.lean | Integration with big operators (sums, products) over finsupp support |
| Encodable.lean | Encodability of finsupp types when domain and codomain are encodable |
| Ext.lean | Extensionality lemmas for finsupps |
| Fin.lean | Specialized results for finsupps with `Fin n` domain |
| Fintype.lean | Results for finsupps when the domain is a fintype |
| Indicator.lean | Indicator function constructions for finsupps |
| Interval.lean | Interval-related operations on finsupps |
| NeLocus.lean | "Not-equal locus" - the support of the difference of two finsupps |
| Option.lean | Finsupps with Option domain |
| PWO.lean | Partial well-ordering properties for finsupps |
| Pointwise.lean | Pointwise operations on finsupps treated as generalized multisets |
| PointwiseSMul.lean | Pointwise scalar multiplication operations |
| SMul.lean | Scalar multiplication structure on finsupps |
| SMulWithZero.lean | Scalar multiplication with zero absorption |

## Subdirectories

- [ ] `MonomialOrder/` - Additional monomial order constructions (e.g., graded lexicographic order)

## Search Tags

finsupp finitely-supported-functions sparse-functions polynomials monoid-algebra linear-combination lexicographic-order monomial-order weight degree grobner-basis support single maprange embedomain
