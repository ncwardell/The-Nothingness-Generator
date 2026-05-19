# 02. The Two Roots

> **The self-reference equation has exactly two solutions: $\phi$ and $\psi$. They are the eigenvalues of self-reference.**

---

## Question

The self-reference equation $x^2 - x - 1 = 0$ is in place. *What values of $x$ satisfy it?*

## Dependencies

- [01. The self-reference equation](01-the-self-reference-equation.md) — $x^2 - x - 1 = 0$.

## Commitment

None. The roots are forced by the equation.

## Construction

The equation $x^2 - x - 1 = 0$ has discriminant $\Delta = 1 + 4 = 5$. By the quadratic formula:

$$x = \frac{1 \pm \sqrt{5}}{2}$$

This gives two roots:

$$\phi = \frac{1 + \sqrt{5}}{2} \approx 1.618 \qquad \psi = \frac{1 - \sqrt{5}}{2} \approx -0.618$$

Two roots — exactly. Forced by the degree of the polynomial. No commitment selects how many; the equation has the number of roots its degree dictates.

## Multiplicative polarity, not additive

A vocabulary clarification. The framework's "polar pair" vocabulary in [arithmetic](../../arithmetic/arithmetic.md) refers to **additive polarity**: pairs that sum to zero ($\{1, -1\}$, $\{F(n), -F(n)\}$). The two roots $\phi$ and $\psi$ are *not* polar in that sense — $\phi + \psi = 1$, not $0$.

They are polar in a different sense: $\phi\psi = -1$ (forced by [Vieta](03-vietas-relations.md), topic 03). Their *product* is the negation of the unit. This is **multiplicative polarity** — a structurally distinct relation.

Both polarities are real consequences of the framework's standing properties, applied at different operational levels (additive in arithmetic, multiplicative in algebra). Where this chain refers to "$\phi$ and $\psi$ as a polar pair," the multiplicative reading is intended.

## All four standing properties respected

- **Conservation:** the two roots together satisfy the conservative sum (see Vieta, topic 03).
- **Polarity:** the two roots form a multiplicative polar pair ($\phi\psi = -1$, see clarification above). They are mutually constrained: each is what the other is not, in the algebraic sense made precise by Vieta.
- **Closure:** the roots involve $\sqrt{5}$, which is not in the integer value system. Closure forces internal extension to algebraic numbers — specifically, to $\mathbb{Q}(\sqrt{5})$.
- **Self-Reference:** $\phi$ and $\psi$ are the *eigenvalues* of self-reference — the values for which $x = 1 + 1/x$ is satisfied.
- **Internality of Relations:** the relations among the roots (sum, product) are algebraic and internal.

## Comparison

In standard mathematics, $\phi$ is the golden ratio. Its conjugate $\psi = 1 - \phi = -1/\phi$ is the second root.

## Transferability

**Engages:** Self-Reference + Polarity (two roots forming a polar pair).

**Prediction:** Any lens engaging the same self-reference structure produces two eigenvalues forming a polar pair.

## What this enables

The two roots have algebraic relations to each other. Vieta's formulas make these explicit: [03. Vieta's relations](03-vietas-relations.md).
