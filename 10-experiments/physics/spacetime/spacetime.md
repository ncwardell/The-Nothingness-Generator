# Spacetime

*The arena: the breathing torus. The topological-and-dynamical commitment that provides the spatial-temporal structure for everything else physics articulates.*

---

## What this module is

Spacetime is the first subdomain of [physics](../physics.md). It articulates the *arena* — the topology and dynamics — on which the rest of physics is built. Other physics subdomains (spectrum, forces) import this one.

This file is the **module overview**. The atomic step-by-step articulation lives in [`construction/`](construction/).

## Dependencies

- [Mathematics experiment](../../mathematics/) — $\phi, \psi, i$, the two roots, the polar pair structure, complex extensions.
- [Postulates](../../../01-postulates/), [grammar](../../../03-the-grammar/), [the process](../../../02-the-process/) — the framework's foundation.

## Commitments

| | Commitment | Forces |
|---|---|---|
| **ST1** | The totality has 2D toroidal topology: $T^2 = S^1_{\text{depth}} \times S^1_{\text{time}}$ | Two distinct circular dimensions; closure; $\chi = 0$ as topological Conservation. |
| **ST2** | Breathing dynamics: the two strands ($\phi$, $\psi$) oscillate in antiphase on the torus | Spin and the spinor double cover; reciprocal expansion/contraction. |
| **ST3** | The two circles carry distinct physical roles: $S^1_{\text{depth}}$ is spatial, $S^1_{\text{time}}$ is temporal | Particles inhabit specific (depth, time) coordinates; spectrum and dynamics live in different circles. |

These three commitments are minimal for a self-grounding spacetime articulation. Each cascades through the four standing properties.

## What spacetime produces

| Topic | Generates |
|---|---|
| **[01. The breathing torus](construction/01-the-breathing-torus.md)** | $T^2$ topology; antiphase strand oscillation; the breathing as a dynamical structure |
| **02. Spin from breath cycles** *(planned)* | $4\pi$ periodicity for fermions; integer spin for bosons; the spinor double cover |
| **03. Dual dimensions** *(planned)* | Spatial resonance ($S^1_{\text{depth}}$) vs. temporal address ($S^1_{\text{time}}$); particle = (depth, time) |

## Forced vs. chosen

**Chosen:**

- 2-dimensional topology specifically (not 3D, 4D, 26D, etc.). This is a substantial commitment that should be examined.
- The torus rather than other closed 2-manifolds (sphere, Klein bottle, etc.). Defended on minimality + standing-property grounds: the torus has $\chi = 0$ (topological Conservation), two independent loops (Polarity), and natural self-referential winding.
- The "breathing" interpretation — antiphase oscillation between two strands. Other dynamics on a torus are conceivable.
- Distinct roles for the two circles (depth vs. time). The torus's two circles are *a priori* equivalent; assigning them distinct physical roles is a chosen move.

**Forced (given the choices):**

- Spin's $4\pi$ periodicity from breath cycles + Hopf fibration.
- The structural relation $pf = 1$ (with $p = 1/\phi$, $f = \phi$) constraining the breathing.
- The double-strand structure (forced by polarity at the dynamic level + the algebra's $\phi$/$\psi$ pair).

## Importing this module

A subdomain that builds on spacetime references this file. Spacetime provides:

- The topological arena ($T^2$).
- The breathing dynamics.
- The spin structure.
- The depth/time coordinate system.

The [spectrum](../spectrum/) subdomain imports this to articulate particles as inhabitants of $(d, t)$ coordinates. The [forces](../forces/) subdomain imports this to articulate force couplings as projections of breathing-torus structure.

## Status

Initial port. Topic 01 (the breathing torus) is articulated. Topics 02–03 are planned.
