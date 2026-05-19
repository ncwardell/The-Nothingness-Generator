# 12. Order

> **Comparison among integers: $a < b$ iff $b - a$ is positive. Order is forced by sign + subtraction.**

---

## Question

The integers $\mathbb{Z}$ are in the value system (topic 11). They have polar structure (positives and negatives). *Is there a structural relation that orders them — that distinguishes "less than" from "greater than"?*

## Dependencies

- [05. Addition and subtraction](05-addition-and-subtraction.md) — subtraction is in place.
- [11. Negative integers](11-negative-integers.md) — $\mathbb{Z}$ is in the value system; positives and negatives are distinguished by polarity.

## Commitment

None. Order is forced by polarity (sign) plus subtraction.

## Construction

The polar structure on $\mathbb{Z}$ distinguishes positive from negative. Specifically:

- The positive integers are those values structurally aligned with $1$ (the unit of distinction).
- The negative integers are those structurally aligned with $-1$ (the polar partner).
- $0$ is neither positive nor negative.

This structural distinction is the **sign** of an integer. It is binary: positive, negative, or zero.

For any two distinct integers $a$ and $b$, we form the difference $b - a$ (using subtraction from topic 05). The sign of $b - a$ tells us their relative order:

- If $b - a$ is positive: $a < b$ (a is less than b).
- If $b - a$ is negative: $a > b$ (a is greater than b).
- If $b - a$ is zero: $a = b$.

The relations $<, >, \leq, \geq, =$ are all defined via subtraction + sign. None requires a separate commitment; all are forced.

## Order properties are forced

The standard order axioms are forced consequences of this construction, not separate posits:

- **Reflexivity** ($a \leq a$): forced by $a - a = 0$ and the convention that $a \leq b$ iff $b - a$ is non-negative.
- **Antisymmetry** (if $a \leq b$ and $b \leq a$ then $a = b$): forced by $b - a$ and $a - b$ being polar partners; both non-negative iff both zero.
- **Transitivity** (if $a \leq b$ and $b \leq c$ then $a \leq c$): forced by $(c - a) = (c - b) + (b - a)$ together with the additive structure on positives — the sum of two non-negative integers is non-negative.
- **Trichotomy** (exactly one of $a < b$, $a = b$, $a > b$): forced by sign trichotomy on $\mathbb{Z}$ — every integer is positive, negative, or zero, and these three are disjoint (Topic 11).

None of these is a separate axiom. Each is forced by subtraction, the polar structure on $\mathbb{Z}$, and the additive properties already in place.

## All four standing properties respected

- **Conservation:** order doesn't introduce new content; it is a structural relation derived from existing operations.
- **Polarity:** ✓ — order is the structural articulation of the polar pair (positive vs. negative) at the level of comparison.
- **Closure:** the order relation is closed on $\mathbb{Z}$ — comparing two integers produces a determinate result (less, greater, or equal).
- **Self-Reference:** order is internally articulated — defined by operations on the values themselves, not externally imposed.
- **Internality of Relations:** the order relation is internal — it lives in the value system, defined by internal operations.

## Comparison

In standard mathematics, order on $\mathbb{Z}$ is sometimes posited axiomatically and sometimes derived. The framework's contribution: order is *forced* by sign + subtraction. It is not a separate axiom; it is an articulation of the polar structure.

## Transferability

**Engages:** Polarity (sign-based) + subtraction.

**Prediction:** Any lens with a polar structure and a difference-like operation articulates an analogous order. The structural shape transfers; specific implementations vary.

## What this enables

With order in place, comparisons among integers are well-defined. The next forced extension addresses what happens when division produces non-integer results: [13. Rationals](13-rationals.md).
