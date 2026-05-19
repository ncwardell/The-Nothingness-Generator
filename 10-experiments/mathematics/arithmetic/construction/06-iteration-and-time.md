# 06. Iteration and Time

> **Operations can be applied over time — repeated. Iteration is the commitment; multiplication and division are forced as the iterated forms of addition and subtraction.**

---

## Question

Addition and subtraction are in place — first-order operations. The value system is small ($\{1, -1, 0\}$). *Can operations be applied repeatedly, and what does that admit structurally?*

## Dependencies

- [05. Addition and subtraction](05-addition-and-subtraction.md) — additive operations, polar-paired.

## Commitment

None. **Iteration is forced by [Self-Reference](../../../../03-the-grammar/03-self-reference.md) at the operational level.**

The argument:

1. By [Closure](../../../../03-the-grammar/01-closure.md), the output of an operation is in the value system.
2. Operations take values from the system as inputs.
3. By [Self-Reference](../../../../03-the-grammar/03-self-reference.md), internal structural relations reference internal things — and outputs of operations are internal.
4. Therefore an operation applied to its own previous output is admitted by the standing properties.
5. To *forbid* such application would require imposing an external restriction on what operations can take as inputs — but [Internality of Relations](../../../../03-the-grammar/04-internality-of-relations.md) forbids invoking external standards to restrict structurally-available moves.

Iteration is the operational expression of Self-Reference, parallel to how [subtraction](05-addition-and-subtraction.md) was forced as Polarity's operational expression. The standing properties apply at the operational level (precedent: Polarity forcing operation pairs); Self-Reference at the operational level forces operations applied to their own outputs.

The label "time" is not a semantic overlay. It is the name for the structural index of repeated self-application — internal articulation of an internal relation, not external interpretation.

Iteration is not a new *operation*; it is a *mode of applying* existing operations. Multiplication and division are not new commitments either; they are the forms operations take under iteration:

- **Multiplication** is addition iterated over time.
- **Division** is subtraction iterated over time.

All forced — neither iteration itself nor its operational consequences are separate commitments.

## Construction

Given the additive pair $\{+, -\}$ and iteration forced by Self-Reference at the operational level, we can apply each operation $n$ times. The result of applying $+$ to the same operand $n$ times is what we call **multiplication**:

$$a \cdot n \equiv \underbrace{a + a + \cdots + a}_{n \text{ times}}$$

By [Polarity](../../../../03-the-grammar/02-polarity.md) at the operational level, the polar partner of multiplication is the iterated form of subtraction — **division**:

$$a / n \equiv \text{the value } b \text{ such that } b \cdot n = a$$

Equivalently, division is multiplication's inverse.

## Multiplication and division as second-order operations

This framing matters. The operations we already had:

- $+, -$ are **first-order**: they combine two values into one.

The operations now articulated:

- $\cdot, /$ are **second-order**: they combine first-order operations *over time* — they describe what happens when first-order operations are repeated.

Multiplication and division are not novel operations; they are the same additive operations, *viewed iteratively*. The framework's claim is that this is structurally significant: time enters not as a new postulate but as the dimension along which iteration unfolds.

## All four standing properties respected

- **Conservation:** multiplication and division preserve the conservative budget. Adding $a$ to itself $n$ times produces a balanced contribution; iterating subtraction inversely.
- **Polarity:** division forced as polar partner of multiplication. ✓
- **Closure:** the result of $a \cdot n$ may not be in the currently-populated value system. Closure forces an internal extension — by self-referential generation, in Phase III. (The framework defers the extension; iteration alone does not posit new values.)
- **Self-Reference:** iteration is itself self-referential — applying an operation to its own previous output. This is the structural meaning of "second-order over time."
- **Internality of Relations:** the iteration relation is internal — defined by repeated application of an internal operation.

## What time is

A note: time enters here as the *index* of iteration — the discrete steps that distinguish first application from second. Time is not yet a continuous parameter; it is just "how many times have we iterated." Continuous time would require additional commitments not made here.

This articulation of time is consistent with the [framework's emphasis on self-reference as foundational](../../../../03-the-grammar/03-self-reference.md): time is not pre-given; it is what iteration of self-referential operations articulates.

## Comparison

In standard mathematics, multiplication is iterated addition and division is iterated subtraction. The framing here is the same; the structural emphasis differs: multiplication is not a separate operation but a temporal mode of addition.

## Transferability

**Engages:** Polarity (iterated operations come in pairs) + Self-Reference (iteration as self-application).

**Prediction:** Any lens admitting iteration of base operations articulates the same second-order structure: a multiplication-like operation paired with a division-like operation, both as iterated forms of the lens's additive pair.

## What this enables

With iteration in place, sequences of values can be generated. The minimal self-referential sequence — the one matching the framework's self-reference structure — is **[07. Fibonacci](08-fibonacci.md)**.
