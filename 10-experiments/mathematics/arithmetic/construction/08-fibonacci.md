# 08. Fibonacci

> **The only self-referential dynamic available: at order 2, four coefficient pairs exist, two are periodic, and the survivors differ only by sign.**

---

## Question

Operations are in place ($+, -, \cdot, /$). Iteration is admissible (forward and backward). The value system contains $\{1, -1, 0\}$ but no integers beyond. *What self-referential dynamics are available to generate new values internally, respecting Closure — and how many are there?*

## Dependencies

- [05. Addition and subtraction](05-addition-and-subtraction.md) — addition is in place.
- [06. Iteration and time](06-iteration-and-time.md) — iteration is admissible.
- [07. Backward iteration](07-backward-iteration.md) — iteration is bidirectional.

## Commitment

**None.** Earlier drafts committed here to "minimal order with minimal coefficients," on atomicity grounds. That commitment is not needed: the candidates are not infinite and then narrowed by taste — **only four exist**, and Closure eliminates all but one up to sign. The construction below enumerates them.

The reason the field is finite is [Internality](../../../../01-postulates/internality.md). A recurrence's coefficients must be *values*, and the only values generated so far are $\{1, -1, 0\}$ (topics 02 and 04). Coefficients outside that set are not available to be chosen — they have not been generated. This is *generative availability*, not minimality; see [Polarity](../../../../03-the-grammar/02-polarity.md) (Reading note) for the general form of the argument.

## Construction

A self-referential sequence has $F(n)$ depending on prior $F$ values. Walk the candidates:

- **Order 0** ($F(n) = c$): no prior reference; not self-referential.
- **Order 1** ($F(n) = a \cdot F(n-1)$): references one prior value. The eigenvalue $a$ is a free parameter; not self-determining.
- **Order 2** ($F(n) = a \cdot F(n-1) + b \cdot F(n-2)$): references two prior values. Eigenvalues are determined as roots of the characteristic polynomial $x^2 - ax - b = 0$ — internally determined.

Minimum order for a self-determining self-referential structure: 2.

### The coefficients are not freely chosen

An order-2 recurrence is $F(n) = a F(n-1) + b F(n-2)$. Its coefficients must be **values**, and the value system at this point contains only $\{1, -1, 0\}$. Nothing else has been generated, so nothing else is available.

- $b = 0$ collapses the recurrence to order 1 — already excluded as not self-determining.
- $a = 0$ leaves $F(n) = bF(n-2)$, which is two uncoupled order-1 chains, not a genuine order-2 self-reference.

So $a, b \in \{1, -1\}$: **exactly four candidates.** Enumerate all of them, with $F(0) = 0$, $F(1) = 1$ (the only values available for initial conditions):

| $(a,b)$ | Characteristic | Roots | Sequence | Generates? |
|---|---|---|---|---|
| $(1, 1)$ | $x^2 - x - 1$ | $\phi, \psi$ (real, $\|\phi\| > 1$) | $0,1,1,2,3,5,8,13,\ldots$ | **yes** |
| $(1, -1)$ | $x^2 - x + 1$ | complex, $\|r\| = 1$ | $0,1,1,0,-1,-1,0,\ldots$ | no — period 6 |
| $(-1, 1)$ | $x^2 + x - 1$ | real, $\|r_{\max}\| > 1$ | $0,1,-1,2,-3,5,-8,\ldots$ | **yes** |
| $(-1, -1)$ | $x^2 + x + 1$ | complex, $\|r\| = 1$ | $0,1,-1,0,1,-1,\ldots$ | no — period 3 |

**Two candidates are eliminated by Closure.** $(1,-1)$ and $(-1,-1)$ have characteristic roots on the unit circle: they are periodic and never leave $\{0, 1, -1\}$. They generate no new values, so they fail this topic's requirement — the question asked for a dynamic that *generates new values internally*.

**The two survivors generate identical magnitudes.** $(-1, 1)$ produces $0, 1, -1, 2, -3, 5, -8, \ldots$ — the same sequence as $(1,1)$ with alternating sign. They differ only in which polarity is carried along the iteration, and iteration is already bidirectional (topic 07) with sign already governed by Polarity. The two are the same structure read in two directions, not two structures.

What remains is therefore a single dynamic, fixed up to a sign convention:

$$F(n) = F(n-1) + F(n-2)$$

With $F(0) = 0, F(1) = 1$, it generates:

$$0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, \ldots$$

These are the **Fibonacci numbers**. Each is generated internally by addition. No external successor.

## What Fibonacci generates

The sequence introduces new values: $F(3) = 2, F(4) = 3, F(5) = 5, F(6) = 8, \ldots$ Each new Fibonacci value carries (by Polarity) its polar complement $-F(n)$.

## All four standing properties respected

- **Conservation:** Σ preserved — each new $F(n)$ comes with $-F(n)$.
- **Polarity:** every Fibonacci value has its negative.
- **Closure:** ✓ — central. New values are generated from within, by addition on existing values. The value system extends internally; no external posit.
- **Self-Reference:** the recurrence is self-referential by construction.
- **Internality of Relations:** internal recurrence relation.

## Why this is forced, not minimal

- Orders 0 and 1 do not produce a self-determined eigenvalue.
- At order 2, only $\{1, -1, 0\}$ have been generated, so only four coefficient pairs exist. Two are periodic and generate nothing; the remaining two are the same sequence up to sign.
- Initial conditions $0, 1$ are the only values available that do not make the sequence identically zero.

No flavor of [atomicity](../../../../02-the-process/atoms.md) is selected here. The field of candidates is finite because little has been generated, and Closure eliminates all but one of them.

## Note on the relation to algebra

An earlier draft of this topic justified Fibonacci by pointing *forward* to algebra: its characteristic polynomial is $x^2 = x + 1$, the self-reference equation, and algebra was said to show that this is what Self-Reference forces.

**That argument deferred, and has been withdrawn.** [Algebra topic 01](../../algebra/construction/01-the-self-reference-equation.md) derives $x^2 = x + 1$ *by taking the characteristic polynomial of the Fibonacci recurrence* — it lists this topic among its dependencies, and its own commitment note says it "only recognizes the algebraic shadow of an already-existing dynamic." Each side named the other as its warrant, so the argument was located nowhere in the loop. The defect is not the loop itself — mutual constitution is native here, as with $E$ and $-E$ — but that neither node held its own content. By [atomicity](../../../../02-the-process/atoms.md), a composite whose parts live elsewhere and never terminate is infinite descent, which Internality forbids.

The enumeration above replaces that argument and grounds Fibonacci **within arithmetic alone**, which is where it belongs. Algebra then legitimately builds on it, and the dependency runs one way only.

What survives, and is worth stating once each node stands on its own: the dynamic forced here at the substrate level turns out to have $x^2 = x + 1$ as its characteristic polynomial — the same form that Self-Reference takes when articulated as an equation. That is a **convergence between two levels of articulation**, and convergences are the framework's own strongest evidence (see [transferability](../../../../15-cross-domain-analysis/transferability.md)). It is evidence precisely *because* each derivation now holds its own content — the loop can be seen whole rather than only traversed. The repair did not remove a circle; it filled one.

## Comparison

In standard mathematics, Fibonacci is well-known. The framework's contribution: Fibonacci is the *Closure-respecting* generator of new values — the only mechanism by which the integer system extends without external posit.

## Transferability

**Engages:** Self-Reference + Closure + Polarity + iteration.

**Prediction:** Any lens engaging self-referential dynamic generation articulates an analogous minimal-order self-referential recurrence.

## What this enables

Fibonacci runs forward in time. By [topic 07 (backward iteration)](07-backward-iteration.md), it must also run backward. That is [09. NegaFibonacci](09-negafibonacci.md).
