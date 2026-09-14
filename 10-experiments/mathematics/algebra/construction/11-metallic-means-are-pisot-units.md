# 11. The Metallic Means Are Pisot Units

> **Every metallic mean is a quadratic Pisot unit — forced, in one line, by the invariant Vieta product $\sigma_k \bar\sigma_k = -1$. The framework's reciprocal relation *is* the Pisot condition.**

---

## Question

The metallic family $\sigma_k$ exists (topic 10), with invariant product $\sigma_k \bar\sigma_k = -1$. *Does that invariant have consequences beyond bookkeeping — does it place the whole family in a distinguished class?*

## Dependencies

- [10. The metallic generalization](10-the-metallic-generalization.md) — the family $\sigma_k$ and its Vieta relations.
- [03. Vieta's relations](03-vietas-relations.md) — the product relation this topic uses.
- [08. Field extensions](08-field-extensions.md) — algebraic integers and conjugates in a quadratic extension.

## Commitment

None. The result is forced by the Vieta product established in topic 10.

## Construction

### Definitions

An **algebraic integer** is a root of a monic polynomial with integer coefficients. Its **conjugates** are the other roots of that polynomial.

A **Pisot number** is a real algebraic integer $\alpha > 1$ all of whose conjugates have modulus strictly less than 1.

An algebraic **unit** is an algebraic integer whose inverse is also an algebraic integer — equivalently, one whose norm is $\pm 1$.

### The proof

$\sigma_k$ is a root of $x^2 - kx - 1$, which is **monic with integer coefficients** (topic 10, with $k$ a produced integer). So $\sigma_k$ is an algebraic integer, and by topic 10 the polynomial is irreducible for every admissible $k$ — so $\sigma_k$ has degree exactly 2 and exactly one conjugate, $\bar\sigma_k$.

**Step 1 — $\sigma_k > 1$.** $\sigma_k = \tfrac{1}{2}(k + \sqrt{k^2+4}) > \tfrac{1}{2}(k + k) = k \ge 1$.

**Step 2 — the conjugate lies inside the unit circle.** By the Vieta product,

$$\sigma_k \bar\sigma_k = -1 \implies |\bar\sigma_k| = \frac{1}{\sigma_k} < 1$$

using Step 1. The conjugate's modulus is the *reciprocal* of the root.

**Step 3 — $\sigma_k$ is a unit.** The norm of $\sigma_k$ in $\mathbb{Q}(\sqrt{k^2+4})$ is the product of its conjugates, $\sigma_k \bar\sigma_k = -1$. Norm $-1$ is a unit.

$$\boxed{\text{Every } \sigma_k \text{ is a quadratic Pisot unit.}}$$

The whole proof is the single relation $\sigma_k \bar\sigma_k = -1$ read twice: once as "the conjugate is the reciprocal" (Pisot) and once as "the norm is $-1$" (unit).

### The framework content

The Pisot condition is *"the root exceeds 1 and its conjugate is trapped inside the unit circle."* In the framework's vocabulary that is exactly the **polar reciprocal relation**: two quantities whose product is the negative unit, one expanding and one contracting, neither able to move without the other.

This is not an analogy drawn after the fact. The relation doing the work — product $= -1$ — is the same relation topic 03 identified as Polarity regenerated inside algebra. **Polarity and the Pisot property are the same statement**, read in two vocabularies. The framework does not need to reach for the Pisot condition; it has been carrying it since topic 03.

## What this articulates

- **A family-level invariant from a family-invariant relation.** Topic 10 showed Conservation distinguishes $k = 1$ while Polarity is family-invariant. This topic shows what the family-invariant relation buys: membership in a distinguished class, uniformly, for every $k$.
- **The contraction is the reciprocal of the expansion.** $|\bar\sigma_k| = 1/\sigma_k$ exactly — not approximately, for every $k$. The two roots are a reciprocal pair by construction.
- **Boundedness from Polarity.** Because every conjugate is trapped inside the unit circle, powers $\sigma_k^n$ approach integers: $\sigma_k^n + \bar\sigma_k^n$ is an integer for every $n$, and $\bar\sigma_k^n \to 0$. The integer sequences of the family (Fibonacci for $k=1$, Pell for $k=2$, …) are the visible residue of that vanishing conjugate.

## All four standing properties respected

- **Conservation:** ✓ the norm is exactly $-1$ for every $k$ — the polar unit, invariant across the family. Nothing accumulates.
- **Polarity:** ✓ this topic *is* Polarity, in the form $\sigma_k \bar\sigma_k = -1$: one root beyond the unit, its complement within it. The Pisot property is the algebraic name for that pairing.
- **Closure:** ✓ both roots lie in $\mathbb{Q}(\sqrt{k^2+4})$; conjugation is an internal operation on that field (topic 08).
- **Self-Reference:** ✓ the reciprocal relation $|\bar\sigma_k| = 1/\sigma_k$ is self-referential in form — each root's modulus is determined by the other's.
- **Internality of Relations:** ✓ conjugation is a field automorphism, defined entirely within the extension. No external reference is used to locate the conjugate.

## Comparison

**The mathematics is standard.** That $x^2 - kx - 1$ generates Pisot units is not new; the framework's contribution is that this family arrives *forced* by Internality and Polarity rather than posited.

**Where Pisot numbers matter outside.** For self-similar (substitution) tilings, the inflation factor being Pisot is a **necessary** condition for the tiling to have pure point diffraction — sharp Bragg peaks, the experimental signature of a quasicrystal rather than aperiodic disorder. (Sufficiency is the open *Pisot substitution conjecture*; the necessity direction is established.)

Comparing the family against observed quasicrystal symmetries:

| Observed symmetry | Inflation factor | Minimal polynomial | Family member |
|---|---|---|---|
| 5-fold / 10-fold (Penrose, decagonal, icosahedral) | $1.618034$ | $x^2 = 1x + 1$ | **$\sigma_1$, golden** |
| 8-fold (octagonal, Ammann–Beenker) | $2.414214$ | $x^2 = 2x + 1$ | **$\sigma_2$, silver** |
| 12-fold (dodecagonal) | $3.732051$ | $x^2 = 4x - 1$ | **no** — wrong sign |

**The correspondence is partial and must be stated as such.** It fails in both directions: dodecagonal quasicrystals are real and well characterized, and $2+\sqrt3$ is Pisot but is *not* a metallic mean; conversely $\sigma_3$ and beyond correspond to no observed quasicrystal symmetry. The family is a **subset** of the admissible inflation factors, not an enumeration of realized ones.

What is genuinely notable is narrower: the two quasicrystal families whose inflation factors *are* metallic means are $k = 1$ and $k = 2$ — the two lowest members, the ones with the earliest birth positions in topic 10. Whether that is structural or coincidental is **open**, and this topic claims nothing about it.

## Transferability

**Engages:** Polarity + Closure.

**Prediction:** Any lens articulating a reciprocal polar pair — two quantities whose product is the negative unit, one expanding beyond the unit and one contracting within it — will find the expanding member is a Pisot number of that lens's value system, and will find its powers approaching the lens's integers.

## What this enables

The vanishing conjugate is what makes each family member's integer sequence well defined and its powers near-integral — the structural ground for any later topic that needs those sequences. Nothing in this chain depends on the *external* correspondence noted under Comparison, which is recorded as observation only.
