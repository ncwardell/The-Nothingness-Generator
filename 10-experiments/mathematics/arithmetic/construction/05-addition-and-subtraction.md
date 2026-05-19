# 05. Addition and Subtraction

> **Addition is the binary form of $\Sigma$. Subtraction is forced as its polar partner — one commitment, two operations.**

---

## Question

The labeled values $\{1, -1, 0\}$ are in place. The postulate uses $\Sigma$ as an n-ary sum. *Can $\Sigma$ be articulated as a binary operation, and what comes with it by polarity?*

## Dependencies

- [01. Polar bisection](01-polar-bisection.md), [02. Zero](02-zero.md), [03. The polar relation](03-the-polar-relation.md), [04. Labeling the pair](04-labeling-the-pair.md) — labeled values $\{1, -1, 0\}$ and the negation map are in place.

## Commitment

**One commitment: addition is the binary form of $\Sigma$.** The conservation operator $\Sigma$ is given by the postulate as n-ary (it sums the totality). We articulate its binary form as $+: V \times V \to V$.

By [Polarity](../../../../03-the-grammar/02-polarity.md), every operation comes with its polar partner. Addition's polar partner is composition with the negation map: $a - b \equiv a + \nu(b)$. **Subtraction is forced**, not separately committed.

One commitment introduces both halves of the additive operation pair.

## Construction

The binary $+$ inherits four properties forced by coherence with the n-ary $\Sigma$:

- **Identity:** $0 + v = v$ (Conservation: adding zero leaves the conservative sum unchanged).
- **Inverses:** $v + (-v) = 0$ (Polarity: the polar pair sums to zero).
- **Associativity:** $(a + b) + c = a + (b + c)$ ($\Sigma$ is well-defined regardless of grouping).
- **Commutativity:** $a + b = b + a$ ($\Sigma$ is independent of element order).

These are not separate commitments. They are forced by the requirement that $+$ be the binary form of $\Sigma$.

Subtraction is defined via the negation map:

$$a - b \equiv a + \nu(b) = a + (-b)$$

The polar map $\nu$ already exists (topic 03); composing it with $+$ gives subtraction automatically.

## All four standing properties respected

- **Conservation:** $+$ is the binary form of $\Sigma$ and preserves it by construction.
- **Polarity:** subtraction is forced as polar partner.
- **Closure:** $+$ closes on the value system as currently populated ($\{1, -1, 0\}$): $1 + 0 = 1$, $1 + (-1) = 0$, $0 + 0 = 0$, etc. The result of $1 + 1$ is not yet in the value system; admitting it requires self-referential generation, which arrives in Phase III (Fibonacci).
- **Self-Reference:** $+$ is the binary form of the operation by which the totality sums itself.
- **Internality of Relations:** the "$+$" relation is internal — no external standard defines it.

## Comparison

In standard mathematics, addition and subtraction are usually paired with subtraction defined as addition of the inverse. The structural reason is polarity at the operational level — what the framework makes explicit.

## Transferability

**Engages:** Conservation + Polarity.

**Prediction:** Any lens that admits operations on a polar pair must articulate operations in polar pairs — never one operation alone.

## What this enables

With $+$ and $-$ in place, the next operational extension is iteration: applying operations repeatedly. That is [06. Iteration and time](06-iteration-and-time.md).
