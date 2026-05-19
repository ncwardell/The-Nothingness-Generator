# 13. Rationals

> **Division by integers that don't divide cleanly produces non-integer values. Closure forces internal extension to the rationals $\mathbb{Q}$.**

---

## Question

Division was committed in topic 06 as the polar partner of multiplication. Division of integer $a$ by integer $b$ may not produce an integer (e.g., $1 / 2$ is not in $\mathbb{Z}$). *What does Closure require when division produces values not in the current value system?*

## Dependencies

- [06. Iteration and time](06-iteration-and-time.md) — division is in place.
- [11. Negative integers](11-negative-integers.md) — $\mathbb{Z}$ is the current value system.

## Commitment

None new. Closure forces the extension internally; the rationals are not externally posited.

## Construction

Division of integer $a$ by non-zero integer $b$ produces a value $a / b$. By the definition of division as the inverse of multiplication, $a / b$ is the value $c$ such that $c \cdot b = a$.

For most pairs $(a, b)$ with $b \neq 0$, $c$ is not in $\mathbb{Z}$ (e.g., $1 / 2$, $3 / 7$, $-5 / 4$).

By [Closure](../../../../03-the-grammar/01-closure.md), these values cannot be externally posited. They must emerge internally. The internal mechanism is straightforward: each new value is constructed as a *pair* $(a, b)$ representing "$a$ divided by $b$," with equivalence under cancellation: $(a, b) \sim (ka, kb)$ for any non-zero integer $k$.

The set of equivalence classes is the **rationals** $\mathbb{Q}$:

$$\mathbb{Q} = \{ a / b : a, b \in \mathbb{Z}, b \neq 0 \} / \sim$$

Each rational is a structural composition of two integers (numerator and denominator), with the integers themselves being Zeckendorf compositions of Fibonacci atoms (and their polar reflections). So rationals are *compositions of compositions of self-referential atoms*. Internal at every level.

## What this gives

- **The value system extends to $\mathbb{Q}$.** All ratios of integers (with non-zero denominators) are now values.
- **Division is total on $\mathbb{Q} \setminus \{0\}$.** Every non-zero rational has a multiplicative inverse.
- **The value system is now a field** (with $+, -, \cdot, /$ all internal).

## All four standing properties respected

- **Conservation:** $\mathbb{Q}$ inherits the conservative structure of $\mathbb{Z}$. For each rational $a/b$, the polar partner $-a/b$ exists; their sum is zero.
- **Polarity:** ✓ — every rational has its polar complement.
- **Closure:** ✓ — rationals are constructed internally from existing integers and operations. No external posit.
- **Self-Reference:** rationals are compositions of integers, which are compositions of Fibonacci atoms. Self-reference at the foundational level extends through.
- **Internality of Relations:** the equivalence relation $(a, b) \sim (ka, kb)$ is internal — defined by integer multiplication.

## Comparison

In standard mathematics, $\mathbb{Q}$ is constructed from $\mathbb{Z}$ as equivalence classes of pairs. The framework's contribution: this construction is *forced by Closure* — it is not a separate posit but the internal extension required when division produces values outside the current system.

## Transferability

**Engages:** Closure + Polarity (rationals inherit polar structure from integers).

**Prediction:** Any lens with division-like operations on a value system must articulate the analogous extension to "ratios" — the equivalence-class construction.

## What this enables

The value system is now a field. The next forced extension is iteration of multiplication, which gives powers: [14. Powers](14-powers.md).
