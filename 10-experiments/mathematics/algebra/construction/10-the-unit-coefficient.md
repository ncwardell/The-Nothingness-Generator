# 10. The Unit Coefficient

> **The "1" in $x = 1 + 1/x$ is not a free choice. Conservation admits no other value.**

---

## Question

The self-reference equation is $x = 1 + 1/x$ (topic 01). Its coefficient is the unit "1", inherited from the labeling commitment in arithmetic. Vieta's relations and the degenerate triple were then derived from it. *Was that coefficient forced, or was it one value among many that would have served equally well?*

## Dependencies

- [01. The self-reference equation](01-the-self-reference-equation.md) — $x = 1 + 1/x$, i.e. $x^2 - x - 1 = 0$.
- [03. Vieta's relations](03-vietas-relations.md) — the sum and product of the two roots.
- [04. The degenerate triple](04-the-degenerate-triple.md) — $\phi\psi + (\phi + \psi) = 0$, Conservation regenerated.

## Commitment

None. The test is a counterfactual on structure already derived: no new object is admitted, and nothing is carried in from outside.

## Construction

Suppose the coefficient were some other value $k$ — that is, suppose self-reference took the form $x = k + 1/x$, or

$$x^2 - kx - 1 = 0$$

By topic 03, Vieta's relations for this equation give

$$r_1 + r_2 = k \qquad r_1 r_2 = -1$$

The **product is unchanged**: it is $-1$ for every $k$. Polarity survives any coefficient.

By topic 04, Conservation is regenerated inside algebra when the two Vieta relations sum to zero. Applying that same combination here:

$$r_1 r_2 + (r_1 + r_2) = -1 + k = k - 1$$

$$\boxed{r_1 r_2 + (r_1 + r_2) = 0 \iff k = 1}$$

For every other coefficient the combination leaves a residue $k - 1 \ne 0$. The degenerate triple does not close, and Conservation is not regenerated.

The coefficient was never free. **Polarity permits any $k$; Conservation permits only $k = 1$.**

## What this articulates

- **A choice that was not a choice.** The unit coefficient entered topic 01 from arithmetic's labeling commitment and was carried forward without examination. It turns out to be the only value the postulates allow.
- **The two relations do different work.** The product relation is coefficient-blind — Polarity is indifferent to the coefficient. The sum relation carries it, and Conservation reads the sum. Where the two relations were previously a pair, they are now distinguished by what each is sensitive to.
- **A test, not an extension.** Nothing new is admitted here. The counterfactual coefficient is entertained and then eliminated; the value system is exactly as it was.

## All four standing properties respected

- **Conservation:** ✓ this topic *is* Conservation acting as a selector. It is the property that does the eliminating.
- **Polarity:** ✓ preserved under every $k$ — the product $-1$ is invariant. Polarity is shown to be the weaker constraint of the two.
- **Closure:** ✓ no value outside $\mathbb{Q}(\sqrt 5)$ is admitted; the counterfactual roots are entertained and discarded.
- **Self-Reference:** ✓ the form $x = k + 1/x$ is self-referential for any $k$; self-reference alone does not fix the coefficient. It takes Conservation.
- **Internality of Relations:** ✓ the test uses only relations already derived in topics 03 and 04. No external criterion decides the outcome.

## Comparison

In standard mathematics the family $x^2 - kx - 1 = 0$ is studied for its own sake; its roots are called the *metallic means*, of which $\phi$ ($k=1$) is one member among infinitely many, with no principle preferring any. The framework does not generate that family — it generates a single equation and, when asked whether the coefficient was forced, finds that it was.

The difference is directional. Standard treatment: here is a family, $\phi$ is one member. Here: here is $\phi$, and the family is the space of things Conservation rules out.

## Transferability

**Engages:** Conservation + Polarity.

**Prediction:** In any lens, a parameter that survives Polarity may still be eliminated by Conservation. Where a lens carries an unexamined constant, the test is whether the conservative combination closes on zero for any other value.

## What this enables

Topic 01's coefficient is now established as forced rather than inherited, closing a gap in the chain from arithmetic's labeling commitment through to the degenerate triple. Nothing downstream changes; what changes is that it no longer *could* have.
