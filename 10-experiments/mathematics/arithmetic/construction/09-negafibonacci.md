# 09. NegaFibonacci

> **Fibonacci going backward in time: $F(-n) = (-1)^{n+1} F(n)$. The polar partner of Fibonacci, forced by backward iteration applied to the recurrence.**

---

## Question

Fibonacci (topic 08) is a self-referential dynamic running forward. By Polarity, every commitment has its polar partner. Backward iteration (topic 07) is iteration's polar partner. *What does Fibonacci look like under backward iteration?*

## Dependencies

- [07. Backward iteration](07-backward-iteration.md) — backward iteration is forced as iteration's polar partner.
- [08. Fibonacci](08-fibonacci.md) — the forward dynamic recurrence.

## Commitment

None. NegaFibonacci is forced by applying backward iteration to Fibonacci.

## Construction

The Fibonacci recurrence $F(n) = F(n-1) + F(n-2)$ can be inverted to extend the sequence backward. Solve for $F(n-2)$:

$$F(n-2) = F(n) - F(n-1)$$

Apply this iteratively, starting from $F(0) = 0$ and $F(1) = 1$:

$$F(-1) = F(1) - F(0) = 1 - 0 = 1$$
$$F(-2) = F(0) - F(-1) = 0 - 1 = -1$$
$$F(-3) = F(-1) - F(-2) = 1 - (-1) = 2$$
$$F(-4) = F(-2) - F(-3) = -1 - 2 = -3$$
$$F(-5) = F(-3) - F(-4) = 2 - (-3) = 5$$

In general:

$$F(-n) = (-1)^{n+1} F(n)$$

This is the **NegaFibonacci sequence**: $\ldots, -3, 2, -1, 1, 0, 1, 1, 2, 3, 5, \ldots$ (reading the bidirectional sequence past zero into negative indices).

NegaFibonacci is Fibonacci's polar partner via the time-direction polarity. The values alternate in sign — this is forced by the backward-iteration of an additive recurrence.

## Significance

- **Fibonacci forward** generates positive growth from $\{0, 1\}$.
- **NegaFibonacci** is the same dynamic running backward in time, producing alternating-sign values.

The two together (the bidirectional Fibonacci sequence) span both forward and backward time. Each is the other's polar partner via time-direction.

## All four standing properties respected

- **Conservation:** the bidirectional sequence preserves $\Sigma = 0$ structurally — each NegaFibonacci value $F(-n) = (-1)^{n+1} F(n)$ is a polar reflection of a Fibonacci value, automatically inheriting conservative balance with it.
- **Polarity:** ✓ — NegaFibonacci is the polar partner of Fibonacci via backward iteration.
- **Closure:** NegaFibonacci values are integers; they live in the value system.
- **Self-Reference:** the recurrence is the same in both directions; the dynamic is self-referential whether forward or backward.
- **Internality of Relations:** backward iteration is internal (topic 07).

## Comparison

In standard mathematics, the NegaFibonacci sequence is the well-known extension of Fibonacci to negative indices. The framework's contribution: NegaFibonacci is forced by Polarity at the iteration level, not a separate definition.

## Transferability

**Engages:** Polarity (time-direction, applied to a self-referential dynamic).

**Prediction:** Any lens with a self-referential dynamic must articulate that dynamic's backward extension as a polar partner. Forward and backward dynamics together form a polar pair.

## What this enables

The bidirectional Fibonacci sequence generates a richer set of integer atoms (Fibonacci values plus their backward-iterated counterparts). Combined with Zeckendorf composition, this gives the basis for generating all positive and negative integers internally: [10. Zeckendorf composition](10-zeckendorf-composition.md).
