# 04. Labeling the Pair

> **Commit to labels: $\{1, -1\}$ for the polar pair. The label "1" is the unit of distinction.**

---

## Question

The polar pair, zero, and the negation map are in place. To articulate further structure (operations, equations, dynamics), we need to refer to specific values. *What labels do we commit to for the polar pair?*

## Dependencies

- [01. Polar bisection](01-polar-bisection.md), [02. Zero](02-zero.md), [03. The polar relation](03-the-polar-relation.md) — the polar pair, its sum, and its negation map are in place.

## Commitment

**Labels.** We commit to calling one element of the polar pair "1" and the other "−1". The commitment is purely conventional — the polar pair is structurally symmetric, neither element is privileged. The choice respects polarity: the label and its negation come together (we cannot label "1" without labeling "−1"; the negation map forces the second label).

**Atomicity:** This is one labeling commitment, not two. The polar map forces the second label once the first is chosen.

## Construction

From topic 01, the polar pair is $\{E, -E\}$. The polar relation (topic 03) gives the negation map $\nu: E \mapsto -E$.

We commit:

$$E \mapsto 1, \quad \nu(E) = -E \mapsto -1$$

The label "1" is now the **unit of distinction**: the magnitude of the polar bisection, normalized. Its negation, "−1", is forced by polarity once the first label is chosen.

We have, with this commitment, three labeled values:

- $1$ — the unit of distinction
- $-1$ — its polar complement (forced)
- $0$ — the polar sum (from topic 02)

## Comparison

In standard mathematics, $1$ is the multiplicative identity. Here, $1$ enters as the *unit of distinction* — before any operation is defined. Its multiplicative role appears later when multiplication is committed.

## Transferability

**Engages:** Polarity (labeled).

**Prediction:** Any lens articulating the polar pair will have a labeling — a "primary" pole and its complement, with labels that are mutually negating. Specific labels are lens-specific (vocabulary varies); the *structural fact* of mutually-negating labels transfers.

## What this enables

With labeled values $\{1, -1, 0\}$, we have enough to commit to operations. The first operational commitment — polarity-respecting — is [05. Addition and subtraction](05-addition-and-subtraction.md).
