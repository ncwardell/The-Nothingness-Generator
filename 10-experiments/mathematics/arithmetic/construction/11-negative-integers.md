# 11. Negative Integers

> **Polarity forces every positive integer to have its complement. $\mathbb{Z}^+$ and $\mathbb{Z}^-$ together with $\{0\}$ form $\mathbb{Z}$, the integers as a polar whole.**

---

## Question

The positive integers $\mathbb{Z}^+$ are in the value system (topic 10). Polarity says every element has a polar complement. *What is the polar partner of the set of positive integers as a whole, and is it forced?*

## Dependencies

- [03. The polar relation](03-the-polar-relation.md) — the negation map $\nu$ is in place.
- [10. Zeckendorf composition](10-zeckendorf-composition.md) — the positive integers are in the value system.

## Commitment

None new. The negative integers are forced by Polarity applied to the positive integers — both individually and as a whole set.

## Construction

By [Polarity](../../../../03-the-grammar/02-polarity.md), every non-zero element of the totality has a polar complement. The positive integers $\mathbb{Z}^+ = \{1, 2, 3, 4, 5, \ldots\}$ are in the value system (topic 10). For each $n \in \mathbb{Z}^+$, its polar complement $-n$ must exist.

Apply the negation map $\nu$ (topic 03):

$$\nu(n) = -n \quad \text{for each } n \in \mathbb{Z}^+$$

This generates the **negative integers**:

$$\mathbb{Z}^- = \{-1, -2, -3, -4, -5, \ldots\}$$

Combined with $\mathbb{Z}^+$ and the value $0$ (topic 02), the value system is:

$$\mathbb{Z} = \mathbb{Z}^- \cup \{0\} \cup \mathbb{Z}^+$$

## The integers as a polar whole

The set $\mathbb{Z}$ has its own polar structure: $\mathbb{Z}^+$ and $\mathbb{Z}^-$ are themselves a polar pair (the positive half and the negative half), with $\{0\}$ as the conservative reference between them. This is polarity at the *set level* — applied to the integers as a whole.

The full ring of integers $\mathbb{Z}$ is internally consistent under polarity:

- Each integer has its complement.
- The set of positives has its complementary set of negatives.
- Together they sum (as a totality) to zero.

The set of integers itself articulates the postulates' polar structure at the value-system level.

## All four standing properties respected

- **Conservation:** ✓ — for every positive admitted, its negative is admitted; pairs sum to zero. The full set sums to zero formally (in the appropriate aggregation).
- **Polarity:** ✓ — at both individual and set levels.
- **Closure:** ✓ — negation is internal; applying it produces values that join the system internally.
- **Self-Reference:** the structure of $\mathbb{Z}$ is articulable from within (positives via Zeckendorf, negatives via polarity).
- **Internality of Relations:** the negation map is internal.

## Comparison

Standard mathematics constructs $\mathbb{Z}$ from $\mathbb{N}$ via Peano + extension, or via equivalence classes of pairs. The framework's construction generates positives via Fibonacci+Zeckendorf, then reflects via polarity. Same set; different internal articulation.

## Transferability

**Engages:** Polarity (at element and set levels).

**Prediction:** Any lens articulating a "positive" set of structures via self-referential generation articulates the corresponding "negative" set. The two together form a complete polar whole.

## What this enables

The integers are in place. Their polar structure is articulated. Two further forced extensions follow: order (comparison via sign + subtraction) and rationals (extension when division produces non-integers). The first is [12. Order](12-order.md).
