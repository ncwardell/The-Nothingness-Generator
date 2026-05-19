# 14. Powers

> **Iterated multiplication: $a^n$. Iteration applied to multiplication, just as multiplication was iteration applied to addition.**

---

## Question

Iteration (topic 06) is admissible. Iterated addition gave multiplication. Iterated subtraction gave division. *What about iterated multiplication? Iterated division?*

## Dependencies

- [06. Iteration and time](06-iteration-and-time.md) — iteration is committed; multiplication is iterated addition.
- [13. Rationals](13-rationals.md) — the value system includes $\mathbb{Q}$.

## Commitment

None new. Powers are forced by iteration applied to multiplication.

## Construction

Iteration of multiplication: applying $\cdot$ repeatedly with the same base. We name this **exponentiation** or **powers**:

$$a^n \equiv \underbrace{a \cdot a \cdot \cdots \cdot a}_{n \text{ times}}$$

By [Polarity](../../../../03-the-grammar/02-polarity.md) at the operational level, the polar partner of exponentiation is iteration of division — **roots** (or fractional exponents):

$$a^{1/n} \equiv \text{the value } b \text{ such that } b^n = a$$

Equivalently, roots are the inverse of powers.

## What powers do

- **Conservative aggregation at higher order.** $a^n$ aggregates $n$ copies of $a$ via multiplication, just as $a \cdot n$ aggregated $n$ copies via addition.
- **Hierarchy of operations.** Powers are third-order over time:
  - First-order: addition (and its polar partner subtraction).
  - Second-order: multiplication (iteration of addition); division (its polar partner).
  - Third-order: powers (iteration of multiplication); roots (its polar partner).
- **Recursion in principle goes higher.** Iterated powers would be fourth-order, and so on. Each additional iteration gives a new operational order.

## All four standing properties respected

- **Conservation:** ✓ — powers preserve the conservative structure (each multiplicative aggregation is balanced).
- **Polarity:** ✓ — roots forced as polar partner.
- **Closure:** powers of rationals may not be rational (e.g., $\sqrt{2}$). When this happens, Closure forces extension to a richer value system. Algebraic numbers (roots of polynomials with rational coefficients) become forced. This is articulated more explicitly in the algebra subdomain (topics on field extensions).
- **Self-Reference:** iteration of an operation on its own output is structurally self-referential.
- **Internality of Relations:** the power and root relations are internal, defined by iteration.

## Comparison

In standard mathematics, exponentiation is iterated multiplication; roots are its inverse. The framework's contribution: powers and roots are forced as third-order over time (iteration of iteration), with their polarity-pair structure preserved.

## Transferability

**Engages:** Polarity + iteration (applied recursively).

**Prediction:** Any lens admitting iteration must articulate higher-order operations — the iteration of operations is itself a meaningful operation.

## What this enables

The arithmetic substrate is now substantially complete: integers, rationals, order, operations through third order (addition, multiplication, exponentiation, with their polar partners). The bootstrap, however, requires articulating the *structural relations* among these — equations, identities, abstract structures. That is the role of the [algebra subdomain](../../algebra/algebra.md).
