# 08. Field Extensions

> **The value system extends from $\mathbb{Q}$ to $\mathbb{Q}(\sqrt 5, i)$ to admit $\phi, \psi, i$. The extension is internal, forced by Closure when polynomial roots are admitted.**

---

## Question

The roots $\phi, \psi, i$ are not rationals. They were admitted in topics 02 and 05 as algebraic objects. *What is the structure of the value system that contains them, and is the extension internal?*

## Dependencies

- [Arithmetic](../../arithmetic/arithmetic.md) — provides $\mathbb{Q}$.
- [02. The two roots](02-the-two-roots.md) — $\phi, \psi$ require $\sqrt 5$.
- [05. The complex unit](05-the-complex-unit.md) — admits $i$.
- [07. General polynomials](07-general-polynomials.md) — polynomial roots in general.

## Commitment

None new. Field extensions are forced by Closure when polynomial roots are admitted to the value system.

## Construction

The rationals $\mathbb{Q}$ form a field — closed under $+, -, \cdot, /$. When polynomial equations with rational coefficients have roots not in $\mathbb{Q}$, those roots must be admitted to a larger value system. The natural construction is **field extension**.

### $\mathbb{Q}(\sqrt 5)$

The self-reference equation $x^2 - x - 1 = 0$ has roots $\phi = (1 + \sqrt 5)/2$ and $\psi = (1 - \sqrt 5)/2$. These require $\sqrt 5$. The smallest field containing $\mathbb{Q}$ and $\sqrt 5$ is:

$$\mathbb{Q}(\sqrt 5) = \{ a + b \sqrt 5 : a, b \in \mathbb{Q} \}$$

This is a 2-dimensional vector space over $\mathbb{Q}$. It contains $\phi$ and $\psi$.

### $\mathbb{Q}(i)$

The complex unit $i = \sqrt{-1}$ is admitted by topic 05. The smallest field containing $\mathbb{Q}$ and $i$ is:

$$\mathbb{Q}(i) = \{ a + b i : a, b \in \mathbb{Q} \}$$

Also 2-dimensional over $\mathbb{Q}$. The Gaussian rationals.

### $\mathbb{Q}(\sqrt 5, i)$

The framework needs both $\sqrt 5$ and $i$. The smallest field containing $\mathbb{Q}$, $\sqrt 5$, and $i$ is $\mathbb{Q}(\sqrt 5, i)$:

$$\mathbb{Q}(\sqrt 5, i) = \{ a + b \sqrt 5 + c i + d \sqrt 5 \cdot i : a, b, c, d \in \mathbb{Q} \}$$

A 4-dimensional vector space over $\mathbb{Q}$.

This is the value system the arithmetic+algebra package operates in by the time topic 05 is reached.

## Why this is forced internally

Each extension is constructed as a quotient of polynomial rings:

- $\mathbb{Q}(\sqrt 5) \cong \mathbb{Q}[x] / (x^2 - 5)$
- $\mathbb{Q}(i) \cong \mathbb{Q}[x] / (x^2 + 1)$
- $\mathbb{Q}(\sqrt 5, i) \cong \mathbb{Q}(\sqrt 5)[x] / (x^2 + 1)$

Each quotient is constructed *internally* using polynomial operations on $\mathbb{Q}$ (or extensions thereof). No external posit is invoked. By Closure, the extensions are forced when roots not in the base field are admitted.

## All four standing properties respected

- **Conservation:** ✓ — extended fields preserve $\Sigma = 0$ structure.
- **Polarity:** ✓ — every element of the extension has its polar complement (additive inverse).
- **Closure:** ✓ — this topic *is* Closure made explicit at the level of field extensions.
- **Self-Reference:** the extensions are constructed by polynomial quotients, where polynomials articulate self-referential dynamics (topic 01). Self-reference threads through.
- **Internality of Relations:** the field operations are internal to each extension.

## Comparison

In standard mathematics, $\mathbb{Q}(\sqrt 5)$, $\mathbb{Q}(i)$, $\mathbb{Q}(\sqrt 5, i)$ are studied in algebraic number theory. The framework's contribution: these extensions are forced by Closure when polynomial roots are admitted; they are not separate posits.

## Transferability

**Engages:** Closure (extension forced by polynomial root admission).

**Prediction:** Any lens admitting algebraic structure with polynomial roots requires field-extension-like internal extensions.

## What this enables

The full value system $\mathbb{Q}(\sqrt 5, i)$ is now articulated. The algebra subdomain has produced everything it needs: the self-reference equation, its roots, Vieta's relations, the degenerate triple, the complex unit, linear and general polynomials, field extensions. The bootstrap can be verified: [09. The bootstrap](09-the-bootstrap.md).
