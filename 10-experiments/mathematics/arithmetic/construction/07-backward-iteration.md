# 07. Backward Iteration

> **Iteration's polar partner is backward iteration. Time has two directions; both are forced by polarity at the iteration level.**

---

## Question

Topic 06 committed iteration — applying operations forward over time. By Polarity, every commitment forces its polar partner. *What is iteration's polar partner?*

## Dependencies

- [06. Iteration and time](06-iteration-and-time.md) — iteration is committed; multiplication and division are forced.

## Commitment

None new. The polar partner of iteration is forced by Polarity at the iteration level.

## Construction

Iteration applied an operation repeatedly, indexed by an iteration count $n$. The index $n$ goes forward: 1, 2, 3, ... — each step adds one application.

By [Polarity](../../../../03-the-grammar/02-polarity.md), every commitment must come with its polar partner. Iteration's polar partner is **backward iteration** — applying the operation in reverse, with the index running backward: 0, −1, −2, ... — each step *removes* one application.

This is forced. Once forward iteration is admitted, backward iteration cannot be excluded; it would violate Polarity at the operational level.

## Two ways the polar partner manifests

**At the operation level.** Forward iteration of $+$ gives multiplication. Backward iteration of $+$ gives division. (This is already the polar pair of operations from topic 06.)

**At the temporal level.** Forward iteration extends a sequence into the future ($n = 1, 2, 3, \ldots$). Backward iteration extends the same sequence into the past ($n = 0, -1, -2, \ldots$). The two directions of time are themselves a polar pair.

The two manifestations are aspects of one fact: iteration is bidirectional. The forward direction generates multiplication and forward sequence terms; the backward direction generates division and past sequence terms. Both are available; neither is privileged.

## All four standing properties respected

- **Conservation:** backward iteration preserves $\Sigma = 0$ — moving values "earlier" in a sequence doesn't add or remove conservative content.
- **Polarity:** ✓ — this topic *is* polarity at the iteration level.
- **Closure:** the sequence values produced by backward iteration are still in the value system (or extend it internally, by the same Closure-respecting mechanism that forward iteration uses).
- **Self-Reference:** backward iteration is structurally self-referential — each backward step depends on values produced by earlier backward steps.
- **Internality of Relations:** the backward iteration relation is internal to the value system.

## Comparison

In standard mathematics, recurrences are routinely extended to negative indices, and operations have well-defined inverses. The framework's contribution: backward iteration is *forced by Polarity*, not a separate definition. Forward and backward iteration are not two operations; they are two directions of one operation.

## Transferability

**Engages:** Polarity (at the iteration / temporal level).

**Prediction:** Any lens that admits iteration must articulate the bidirectional nature of time/iteration. Sequences must extend backward as well as forward; processes must have their reverses.

## What this enables

With both directions of iteration available, the self-referential dynamic Fibonacci can be applied in both directions. Forward Fibonacci gives the standard sequence; backward Fibonacci gives [NegaFibonacci](09-negafibonacci.md), the polar partner of Fibonacci.

But first, the forward direction is articulated: [08. Fibonacci](08-fibonacci.md).
