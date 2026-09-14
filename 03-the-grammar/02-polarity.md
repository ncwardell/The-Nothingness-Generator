# Polarity (Weak Form)

> **If the totality contains a non-zero net contribution, it must contain compensating contribution(s) summing to its negation.**

---

## Statement

Let the totality $T$ have an associated sum $\Sigma$ of element contributions, with $\Sigma = 0$ ([Conservation](../01-postulates/conservation.md)) and at least one element with non-zero contribution ([Existence](../01-postulates/existence.md), in the non-trivial reading). Then there exists at least one further element (or set of elements) whose contributions sum to the negation of the first.

Formally: if $E \in T$ has non-zero contribution and $\Sigma_T = 0$, then $\Sigma_{T \setminus \{E\}} = -E$.

## Derivation

The argument is direct arithmetic, given the two postulates and the standard reading of "sum":

1. By Existence, the totality contains some element $E$ with non-zero contribution.
2. By Conservation, the sum over the totality is zero: $\Sigma_T = 0$.
3. Therefore $\Sigma_T = E + \Sigma_{T \setminus \{E\}} = 0$.
4. Therefore $\Sigma_{T \setminus \{E\}} = -E$.

This is the weak form of polarity. It establishes that the totality must contain compensating contribution somewhere — but it does *not* establish that this compensation is concentrated in a single paired element $-E$. The compensation could be distributed across many elements.

## Status

**Strictly derivable** from Conservation + Existence (in the non-trivial reading) + standard arithmetic on sums.

## What this *does not* establish

A stronger form of polarity is sometimes asserted: "If $E$ exists, then a single paired $-E$ exists, such that $E + (-E) = 0$ and $E$, $-E$ are individually distinguishable." That stronger form requires additional assumptions — that the compensation is *concentrated* in a single paired complement element, and that this compensator is *distinguishable* from other elements. The postulates do not force either. Compensation could be distributed; compensators need not be individually labeled.

Any experiment that requires paired polarity — a clearly distinguished $E$ against a clearly distinguished $-E$ — is committing to those additional assumptions. The commitment must be made explicit when it is invoked.

## Reading note

It is tempting to say: "the minimal way to satisfy the weak form is the paired form, so paired polarity follows by minimality." Stated that way it does *not* establish paired polarity, because minimality is a selection principle — a commitment — and the postulates do not say "structure must be minimal."

But the usual objection to paired polarity fails for a different reason, and it is worth stating precisely, because it is the objection this framework attracts most often.

**The objection:** *a totality with compensation distributed across many elements satisfies the postulates equally well, so the paired form is one option among several.*

**Why it does not apply.** That objection compares totalities — it surveys the space of structures satisfying the postulates and observes that several do. **Surveying that space is a view from outside the totality, which [Internality](../01-postulates/internality.md) forbids.** The framework may not ask "which totalities satisfy the postulates?" It may only ask "what is articulable here, given what has been generated?"

Asked that way, distributed compensation is not an available alternative:

- $\Sigma = 0$ restricted to $E$ yields "$E$" and "**the rest**." That is the weak form, already derived above.
- Distributed compensation requires **partitioning the rest** — which requires plurality, and a criterion for telling one compensator from another.
- Neither has been generated. Plurality and discrimination are downstream products of the chain that polar bisection *begins*. Invoking them here imports them from outside.

So the paired form is not selected over the distributed form on grounds of economy. **It is the un-partitioned state — what the cut leaves when nothing further has been generated.** Distributed compensation is not a rejected alternative; at this point it is not constructible.

This is **generative availability**, and it differs in kind from minimality:

| | Says | Status |
|---|---|---|
| Minimality | among available options, take the smallest | a selection principle — **a commitment** |
| Generative availability | only one option is constructible yet | an availability constraint — **forced by Internality** |

An experiment invoking paired polarity therefore need not commit to a minimality principle. It needs to show that, at the point of use, no partition of the compensating remainder has yet been generated. Where richer structure *has* been generated, alternatives become articulable and genuine choices reappear — see [forced-vs-chosen](../02-the-process/forced-vs-chosen.md).

**Corollary.** Forcing is strongest where least has been generated, and weakens as a chain accumulates material. The framework's earliest moves are its most forced ones, not its most assumed.

## What follows

Weak polarity is invoked by:

- [Self-Reference](03-self-reference.md) — together with Internality, the compensating contribution must be referenced from within the totality, which contributes to the self-referential character of any complete account.

## What does *not* follow without further commitment

Weak polarity does not force:

- A specific notion of paired complement.
- A specific notion of distinguishability between $E$ and its compensator(s).
- Any algebraic structure beyond addition.
- Any specific count of compensating elements.
- Any geometric or topological relation between the original element and its compensators.

These require commitments listed at the [boundary](05-boundary.md).

## Composite articulations of compensation (not alternatives)

Binary (single complement, $\{E, -E\}$) is **the atom at the polarity level, by generative availability** (see the Reading note above). Atomicity is forced structurally by Internality (see [atoms.md](../02-the-process/atoms.md)); *which* atom obtains here is settled not by a flavor of minimality but by what is constructible at this point — and the un-partitioned cut is the only thing that is. Binary is forced, not one option among parallel candidates.

What might look like "alternative articulations" — ternary, n-ary, distributed, continuous — are **composites of binary at higher levels of articulation**, not alternative atoms. The order is structural, not temporal: atom first, composites after, on a bigger canvas. The math experiment already produces them as forced consequences.

### Binary (the atom)

| Aspect | Articulation |
|---|---|
| Compensation pattern | Single complement: $\{E, -E\}$ |
| Self-reference equation | $x^2 = x + 1$ (degree 2) |
| Eigenvalues | $\phi, \psi$ (two roots) |
| Conservative regeneration | $\phi\psi + (\phi + \psi) = 0$ (degenerate triple) |
| Complex unit | $i = \sqrt{\phi\psi}$ |
| Status | Bootstrap-verified (math experiment) |

### Ternary as composite

Cube roots of unity $\{1, \omega, \omega^2\}$ with $1 + \omega + \omega^2 = 0$.

Factorization: $x^3 - 1 = (x - 1)(x^2 + x + 1)$.

Decomposes into:
- $1$ (the real axis — binary atom $\{1, -1\}$)
- $\omega, \omega^2$ (a complex-conjugate binary pair, generated by the irreducible quadratic)

Threefold symmetry is **two binary structures composed**, not an alternative articulation. A forced consequence of binary under polynomial composition (degree 3).

### N-ary as composite

$n$-th roots of unity: roots of $x^n - 1 = 0$. Decompose into binary-conjugate pairs (for even $n$) plus the real roots ($x = 1$, and $x = -1$ for even $n$). Same pattern: $n$-fold symmetries are composites of binary atoms under polynomial composition of degree $n$.

### Distributed as composite

$N$ elements summing to zero is *already* what weak polarity gives: for any element $E$, the totality minus $E$ sums to $-E$. This is binary applied at the level of (one element vs the aggregate of the rest). Alternatively, pairwise decomposition: $N$ even gives $N/2$ binary pairs; $N$ odd gives $(N-1)/2$ pairs plus one element compensated by the rest.

### Continuous as composite

$\int \rho(x)\, dx = 0$ is the limit of binary sums. Each finite partition decomposes into binary pairs; the continuous structure emerges as the limit of composite-binary structures. Field-theoretic articulation is binary-at-the-atomic-level scaled across an indexing manifold.

### What this clarifies

The framework's commitment to binary isn't a choice among parallel articulations — it's establishing **the atom**. Once binary is established, the existing math+algebra package naturally produces ternary, n-ary, distributed, and continuous articulations as forced composites — through polynomial extensions, field extensions, integration, and limit operations.

The structural priority (binary first, composites after) follows from atomicity: the atom is what's irreducible at the level; composites are what's built from it on a larger canvas. The framework isn't running one articulation among many; it is running the atomic articulation, and its forced extensions cover the composite articulations.

The remaining open question is not "which articulation is privileged" but **whether these composite articulations transfer cleanly to test-lens experiments**. That is the [strong hypothesis](../15-cross-domain-analysis/the-strong-hypothesis.md)'s empirical content.
