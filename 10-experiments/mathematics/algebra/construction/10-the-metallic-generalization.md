# 10. The Metallic Generalization

> **The self-reference equation admits an integer parameter: $x = k + 1/x$. By Internality, $k$ may only take values the system has already produced. Each admissible $k$ yields a metallic mean $\sigma_k$, and only $k = 1$ regenerates Conservation.**

---

## Question

The self-reference equation (topic 01) is $x = 1 + 1/x$. The coefficient "1" entered as the labeled unit from arithmetic. *Is that coefficient forced, or is it one value of a parameter? And if it is a parameter, what constrains it?*

## Dependencies

- [01. The self-reference equation](01-the-self-reference-equation.md) — $x = 1 + 1/x$ and its characteristic form $x^2 - x - 1 = 0$.
- [02. The two roots](02-the-two-roots.md) — the quadratic has two roots.
- [03. Vieta's relations](03-vietas-relations.md) — $\phi + \psi = 1$, $\phi\psi = -1$.
- [04. The degenerate triple](04-the-degenerate-triple.md) — $\phi\psi + (\phi + \psi) = 0$.
- [Arithmetic: 08. Fibonacci](../../arithmetic/construction/08-fibonacci.md) — the integers the system produces.

## Commitment

| | Commitment | Forces |
|---|---|---|
| **A2** | The unit coefficient in $x = 1 + 1/x$ is a **parameter**, not a constant. | A family of self-reference equations $x = k + 1/x$, one per admissible $k$. |

A2 is **chosen**. Nothing requires the coefficient to vary; the framework operates without A2, with $\phi$ as the sole eigenvalue of self-reference.

But the **constraint on $k$ is forced, by Internality.** There is no outside from which to import a value. Any $k$ must therefore be a value the system has already produced. Arithmetic produces the Fibonacci sequence (arithmetic topic 08), so:

$$k \in \{1, 2, 3, 5, 8, 13, 21, 34, \ldots\}$$

This is the substantive content of A2. Without Internality, $k$ would range over all integers and the parameter would be unconstrained — an imported degree of freedom. With Internality, the family is generated from within, and each member has a **birth position**: the index at which its defining integer first appears.

## Construction

For admissible $k$, the self-reference equation is

$$x = k + \frac{1}{x} \qquad \Longleftrightarrow \qquad x^2 - kx - 1 = 0$$

By topic 07 (general polynomials) this monic quadratic has two roots. By the quadratic formula:

$$\sigma_k = \frac{k + \sqrt{k^2+4}}{2}, \qquad \bar\sigma_k = \frac{k - \sqrt{k^2+4}}{2}$$

**The degree is always exactly 2.** $k^2 + 4$ is never a perfect square for $k \ge 1$: if $k^2 + 4 = m^2$ then $(m-k)(m+k) = 4$, whose only integer solution has $k = 0$. So $\sqrt{k^2+4}$ is irrational for every admissible $k$, and each $\sigma_k$ generates a genuine quadratic extension — never collapsing to a rational.

**Vieta's relations generalize** (topic 03):

$$\sigma_k + \bar\sigma_k = k \qquad \sigma_k \cdot \bar\sigma_k = -1$$

The **product is invariant across the entire family**. Only the sum carries $k$.

### Only $k = 1$ regenerates Conservation

Topic 04 showed that for the fundamental equation the two Vieta relations sum to zero — the degenerate triple, Conservation regenerated inside algebra. Applying the same combination to general $k$:

$$\sigma_k\bar\sigma_k + (\sigma_k + \bar\sigma_k) = -1 + k = k - 1$$

$$\boxed{\sigma_k\bar\sigma_k + (\sigma_k + \bar\sigma_k) = 0 \iff k = 1}$$

**This is forced, and it is the structurally important result of this topic.** The parameter family exists, but only its first member closes on $\Sigma = 0$. Every other $k$ leaves a residue $k - 1 \ne 0$.

So A2 does not put the overtones on equal footing with $\phi$. It does the opposite: it shows that $\phi$ is the **unique member of its own family** that satisfies the framework's founding postulate, and that the others are structurally subordinate — available, but not self-conserving.

## What this articulates

- **The fundamental is distinguished from within.** Before A2, $\phi$ was the only eigenvalue and its primacy was unexamined. After A2, $\phi$ is one of infinitely many candidates and is singled out by Conservation alone. That is a stronger position, not a weaker one.
- **Internality does real work.** The constraint on $k$ is the framework's third postulate acting as a genuine restriction on an otherwise free parameter. Drop Internality and A2 becomes arbitrary.
- **The invariant is the product.** Across the whole family, $\sigma_k \bar\sigma_k = -1$ — the polar pair from arithmetic, unchanged. Polarity is family-invariant; Conservation is not.

## All four standing properties respected

- **Conservation:** regenerated only at $k = 1$, as shown above. For $k > 1$ the residue is $k - 1$; the overtone does not close on zero and is marked as subordinate rather than admitted as an equal.
- **Polarity:** ✓ preserved across the entire family — $\sigma_k \bar\sigma_k = -1$ for every $k$, the two roots always straddling the polar pair (one positive $> 1$, one negative of modulus $< 1$).
- **Closure:** ✓ each $\sigma_k$ lies in the quadratic extension $\mathbb{Q}(\sqrt{k^2+4})$, admitted by the same Closure argument as topic 08.
- **Self-Reference:** ✓ every family member is by construction a fixed point of $x \mapsto k + 1/x$; the whole family is self-referential in the same sense as $\phi$.
- **Internality of Relations:** ✓ the admissible values of $k$ are drawn from the system's own output, not supplied externally. This is the topic's load-bearing use of Internality.

## Comparison

The values $\sigma_k$ are known in the literature as the **metallic means**: $\sigma_1 = \phi$ (golden), $\sigma_2 = 1+\sqrt2$ (silver), $\sigma_3 = (3+\sqrt{13})/2$ (bronze). Their continued fractions are $[k; k, k, k, \ldots]$ — the same purely periodic form as $\phi = [1; 1, 1, \ldots]$, which is the continued-fraction expression of self-reference.

The framework's contribution is not the family, which is standard, but **the constraint and the selection**: Internality restricts $k$ to produced values, and Conservation then singles out $k = 1$ from within the family. Standard treatments introduce the metallic means as a definitional generalization with no principle distinguishing any member.

## Transferability

**Engages:** Self-Reference + Internality + Conservation.

**Prediction:** Any lens that admits a parameterized self-reference relation will find (a) the parameter constrained to values that lens has itself produced, and (b) exactly one parameter value at which the relation closes on $\Sigma = 0$. The others will be available but non-conserving.

## What this enables

The family has a uniform algebraic property that the fundamental alone did not reveal: [11. The metallic means are Pisot units](11-metallic-means-are-pisot-units.md).
