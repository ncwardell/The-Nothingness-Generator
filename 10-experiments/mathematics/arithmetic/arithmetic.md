# Arithmetic

*The substrate of mathematical articulation: values, operations, and integer generation through self-referential dynamics.*

---

## What this module is

Arithmetic is a subdomain of the [mathematics experiment](../mathematics.md). It is the lens that articulates the *specific* values and operations of mathematics: the polar pair, zero, addition/subtraction, multiplication/division, the integers via Fibonacci+Zeckendorf.

This file is the **module overview**. The atomic step-by-step articulation lives in [`construction/`](construction/).

## What arithmetic does and does not do

**What arithmetic generates:**

- The polar pair $\{1, -1\}$ and zero.
- Operations $+, -, \cdot, /$.
- The Fibonacci sequence.
- The integers $\mathbb{Z}$ via Zeckendorf composition + polar reflection.

**What arithmetic alone does *not* do:**

- It does not bootstrap. Pure arithmetic is the substrate of mathematical structure; it produces specific values and computations. The bootstrap requires articulating relations among arithmetic structures algebraically — that is the role of the [algebra subdomain](../algebra/algebra.md).

This distinction matters. Standard usage often blends arithmetic and algebra; here they are separated to make the boundary visible. Arithmetic provides the substrate; algebra articulates the structure.

## Dependencies

- [Postulates](../../../01-postulates/), [standing properties](../../../03-the-grammar/), [the process](../../../02-the-process/) — the framework's foundation.

## Commitments

| | Commitment | Forces |
|---|---|---|
| **C1** | Strong polarity | Polar bisection produces a single paired complement. |
| **C2** | Labels: "1", "−1" | "−1" forced as polar partner of "1". |
| **C3** | Addition (binary form of $\Sigma$) | Subtraction forced as polar partner. Identity, inverses, associativity, commutativity forced by coherence with $\Sigma$. |
| **C4** | Iteration / time *(reframed as forced — see note below)* | Multiplication forced as iterated addition; division forced as iterated subtraction. |
| **C5** | Self-referential iteration of minimal order with minimal coefficients and minimal initial conditions | Fibonacci: $F(n) = F(n-1) + F(n-2)$, $F(0)=0, F(1)=1$. |

That is arithmetic's full commitment list. Each commitment cascades through *all four* standing properties (Closure, Polarity, Self-Reference, Internality of Relations).

**A note on C4.** What was committed here as "iteration is admissible" is forced by [Self-Reference](../../../03-the-grammar/03-self-reference.md) at the operational level. Operations on outputs are admitted by the standing properties: Closure makes outputs internal, Self-Reference references internal structure, and [Internality of Relations](../../../03-the-grammar/04-internality-of-relations.md) forbids external restriction on what operations take as inputs. The time-index is the structural articulation of repeated self-application, not a semantic overlay. The argument is available within arithmetic itself — no later lens required. See [Topic 06](construction/06-iteration-and-time.md#commitment) for the full derivation.

**A note on C5.** The minimality justification is a substrate-level articulation. When [algebra](../algebra/algebra.md) introduces the self-reference equation $x^2 = x + 1$, C5 is retroactively recognized as forced — Fibonacci is the unique integer recurrence whose characteristic equation is the framework's seed in algebraic form. From within arithmetic alone, minimality is the strongest available argument; with algebra in view, the forcing becomes visible. See [Topic 08 — What minimality is shadowing](construction/08-fibonacci.md#what-minimality-is-shadowing).

## What arithmetic produces

| Phase | Topics | Generates |
|---|---|---|
| **I — Forced primitives** | 01–03 | $\{E, -E\}$, value $0$, negation map $\nu$ |
| **II — Operations** | 04–07 | Labels $\{1, -1, 0\}$; $+, -, \cdot, /$; iteration in both directions |
| **III — Self-referential generation** | 08–11 | Fibonacci, NegaFibonacci, Zeckendorf-composed positives, polar-reflected negatives — $\mathbb{Z}$ |
| **IV — Forced extensions** | 12–14 | Order, rationals $\mathbb{Q}$, powers |

After Phase IV, arithmetic is substantially complete as a substrate. The articulation of structural relations among these (the bootstrap) lives in [algebra](../algebra/algebra.md).

## The chain

### Phase I — Forced primitives

- **[01. Polar bisection](construction/01-polar-bisection.md)** — the polar pair $\{E, -E\}$
- **[02. Zero](construction/02-zero.md)** — the value of the polar sum
- **[03. The polar relation](construction/03-the-polar-relation.md)** — the negation map

### Phase II — Operations

- **[04. Labeling the pair](construction/04-labeling-the-pair.md)** — "1", "−1"
- **[05. Addition and subtraction](construction/05-addition-and-subtraction.md)** — additive operations
- **[06. Iteration and time](construction/06-iteration-and-time.md)** — multiplication and division as second-order
- **[07. Backward iteration](construction/07-backward-iteration.md)** — iteration's polar partner; time as bidirectional

### Phase III — Self-referential generation of integers

- **[08. Fibonacci](construction/08-fibonacci.md)** — the minimal self-referential dynamic recurrence
- **[09. NegaFibonacci](construction/09-negafibonacci.md)** — Fibonacci's polar partner via backward iteration
- **[10. Zeckendorf composition](construction/10-zeckendorf-composition.md)** — every positive integer as a unique sum of non-consecutive Fibonacci atoms
- **[11. Negative integers](construction/11-negative-integers.md)** — $\mathbb{Z}$ closed under polarity

### Phase IV — Forced extensions

- **[12. Order](construction/12-order.md)** — comparison via sign + subtraction
- **[13. Rationals](construction/13-rationals.md)** — $\mathbb{Q}$ from division (Closure forces extension)
- **[14. Powers](construction/14-powers.md)** — iterated multiplication (and roots as polar partner)

## Why integer generation uses Fibonacci+Zeckendorf, not successor

[Closure](../../../03-the-grammar/01-closure.md) forbids external posit. New values must emerge from within. Successor (Peano) externally posits "the next integer." Fibonacci is internal: each new value is generated by addition applied to existing values. Zeckendorf composition extends this to all positive integers without external posit.

The integers are not points on a pre-existing line; they are unique compositions of self-referential atoms.

## Forced vs. chosen, in the lens of itself

**Chosen:**

- The lens itself: articulating via arithmetic.
- C1–C3 (strong polarity, labels, addition as binary form of Σ).
- C5 *within arithmetic alone* (on minimality grounds); reframed as forced once algebra articulates the self-reference equation.

**Forced (given the choices):**

- The polar pair, zero, the negation map.
- Subtraction (forced by Polarity at the operational level), division (forced by Polarity applied to multiplication).
- **Iteration and time (forced by Self-Reference at the operational level — what was previously C4).**
- The Fibonacci sequence (forced by C5; structurally forced by seed-identity once algebra is in view).
- The integers via Zeckendorf composition; their negatives via polar reflection.

## Importing this module

Subdomains that build on arithmetic reference this file. Arithmetic provides:

- Values: $\mathbb{Z}$ (integers).
- Operations: $+, -, \cdot, /$.
- Dynamic generators: Fibonacci.
- Composition: Zeckendorf.

The most immediate subdomain that imports arithmetic is **[algebra](../algebra/algebra.md)**, which articulates the algebraic structure of the relations among arithmetic objects.

## Status

Phases I–III complete. Arithmetic is complete as a substrate. The bootstrap of the combined arithmetic+algebra package lives in [algebra](../algebra/algebra.md).
