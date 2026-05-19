# 06. Linear Equations

> **The simplest algebraic equation: $ax + b = 0$. Linear equations are forced once algebraic articulation is admitted; they are simpler than the self-reference equation.**

---

## Question

The self-reference equation (topic 01) was selected as the *minimal* self-referential algebraic equation. But it is degree 2. Lower-degree polynomial equations also exist. *What is the simpler case — the linear equation — and what does it articulate?*

## Dependencies

- [Arithmetic](../../arithmetic/arithmetic.md) — provides operations.
- [01. The self-reference equation](01-the-self-reference-equation.md) — algebraic articulation is committed (commitment A1).

## Commitment

None new. Linear equations are forced once algebraic articulation is admitted; they are simpler than the equations already in play.

## Construction

A linear equation has the form:

$$ax + b = 0$$

where $a, b$ are values from the value system (integers, rationals) and $a \neq 0$. The unique solution:

$$x = -b/a$$

This is a degree-1 polynomial equation. It is *not* self-referential in the same sense as the quadratic — $x$ appears only once, not at multiple powers. The equation determines $x$ from $a$ and $b$ externally.

## Linear is not self-referential, but it is articulable

Topic 01 noted that the minimum self-referential equation is degree 2, because lower degrees do not have $x$ at multiple powers. Linear equations don't articulate self-reference. But they are still articulable algebraically — they are part of the algebra's vocabulary.

So linear equations are forced not as articulations of self-reference but as the simpler case in the polynomial hierarchy: every algebra includes its lower-degree equations, and degree 1 is simpler than degree 2.

## All four standing properties respected

- **Conservation:** $ax + b = 0$ is in conservative form (sums to zero).
- **Polarity:** the solution $x = -b/a$ has its polar partner $b/a$ (the negative). The equation $ax - b = 0$ has solution $b/a$, and the two equations are polar.
- **Closure:** the solution may extend the value system from $\mathbb{Z}$ to $\mathbb{Q}$ (which is already done in arithmetic topic 13). Closure preserved.
- **Self-Reference:** linear equations are *not* self-referential. They are part of the algebraic articulation vocabulary, but they don't articulate self-reference specifically.
- **Internality of Relations:** the linear equation is internal — articulated using internal operations.

## Comparison

In standard mathematics, linear equations are introductory algebra. Their solution method ($x = -b/a$) is straightforward. The framework's contribution: linear equations are forced as the simplest case of algebraic articulation, complementing the self-reference equation (which is the simplest self-referential case).

## Transferability

**Engages:** Algebraic articulation (commitment A1).

**Prediction:** Any lens admitting algebraic articulation includes linear-equation-like cases as the simplest articulable form.

## What this enables

With both linear and quadratic equations available, the natural generalization is to arbitrary-degree polynomials: [07. General polynomials](07-general-polynomials.md).
