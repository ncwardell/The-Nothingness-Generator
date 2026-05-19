# 07. General Polynomials

> **Polynomials of arbitrary degree: $a_n x^n + a_{n-1} x^{n-1} + \cdots + a_0 = 0$. Forced once linear and quadratic articulations are in place.**

---

## Question

Linear equations (topic 06) are degree 1. The self-reference equation (topic 01) is degree 2. *What about higher degrees? Is there a forced generalization to polynomials of arbitrary degree?*

## Dependencies

- [Arithmetic](../../arithmetic/arithmetic.md) — provides operations including powers (topic 14).
- [01. The self-reference equation](01-the-self-reference-equation.md) — degree 2 articulation.
- [06. Linear equations](06-linear-equations.md) — degree 1 articulation.

## Commitment

None new. General polynomials are forced once specific-degree polynomials are in place; once degrees 1 and 2 are admitted, every degree is articulable.

## Construction

A polynomial of degree $n$ has the form:

$$P(x) = a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0$$

where $a_0, a_1, \ldots, a_n$ are coefficients (values from the field $\mathbb{Q}$ or its extensions), and $x^k$ uses powers (arithmetic topic 14).

The polynomial equation $P(x) = 0$ has solutions (roots). For degree 1: one root. For degree 2: two roots. For degree $n$: at most $n$ roots in the algebraic closure.

Polynomials are closed under:

- **Addition:** sum of two polynomials is a polynomial.
- **Multiplication:** product of two polynomials is a polynomial.
- **Composition:** composition of two polynomials is a polynomial.

These operations on polynomials inherit from the underlying field operations. They form a structure: the **polynomial ring** $\mathbb{Q}[x]$ (or over whatever field the coefficients live in).

## Why polynomials are forced

Once linear ($x$) and quadratic ($x^2$) terms are admissible, by closure under multiplication and addition, all higher powers and their combinations are admissible. Polynomial equations of arbitrary degree are then articulable.

The key insight: powers (arithmetic topic 14) and addition together generate all polynomials. No new commitment is needed.

## All four standing properties respected

- **Conservation:** polynomial equations $P(x) = 0$ are in conservative form.
- **Polarity:** roots of polynomials with real coefficients come in polar pairs (positive/negative for odd-degree polynomials with appropriate symmetry; complex conjugate pairs for those with complex roots). Polarity is preserved at the level of roots.
- **Closure:** roots may not be rational. By Closure, the value system extends internally to algebraic numbers, then to algebraic closures.
- **Self-Reference:** specific polynomials may articulate specific self-referential structures (the self-reference equation does this for degree 2). Higher-degree polynomials may articulate higher-order self-references.
- **Internality of Relations:** polynomial relations are internal — defined by internal operations on internal coefficients.

## Comparison

In standard mathematics, polynomials are foundational. The polynomial ring $\mathbb{Q}[x]$ (or $\mathbb{R}[x]$, $\mathbb{C}[x]$) is among the most studied structures. The framework's contribution: polynomials are forced once specific-degree cases are in place; the general structure is not a separate posit.

## Transferability

**Engages:** Algebraic articulation (closed under degree).

**Prediction:** Any lens admitting algebraic articulation generates a polynomial-ring-like structure: closed under addition, multiplication, composition.

## What this enables

With general polynomials in place, the algebraic numbers (roots of polynomials with rational coefficients) extend the value system. This makes explicit what was already implicit in topics 02, 05: [08. Field extensions](08-field-extensions.md).
