# Topology

*The lens articulating structure as connectivity: nodes, edges, cycles, directedness. The triangle as minimum stable witnessing structure; double triangle and chirality; eventually torus and breathing torus.*

---

## What this experiment is

Topology is a lens of the generator. The lens admits nodes (positions in a connectivity structure), edges (relations between nodes), and directedness. Once admitted, witnessing graphs articulate which configurations satisfy the framework's stability and self-reference requirements.

The triangle as minimum stable directed 3-cycle is the entry point. From there: chirality (intrinsic to directed cycles), double triangle (forced by polarity at the structural level), six-element double-helix seed, the algebraic four-structure, and downstream — Hopf fibration, torus, breathing torus.

The bootstrap target: topology regenerates the framework's seed via the double-triangle structure that maps onto the four-structure $\{\phi, \psi, 1, -1\}$ — which the [math experiment's algebra subdomain](../mathematics/algebra/) also produces independently.

This file is the **module overview**. Atomic step-by-step articulation will live in `construction/` (not yet populated).

## Status

Phases I, II, and III complete (Topics 01–08). Bootstrap-verified.

## The lens

- **Substrate:** nodes + edges + directedness.
- **Articulation:** cycles, witnessing relations, chirality, embedding spaces.
- **Bootstrap form:** the double triangle (chirality + 6 elements) regenerates the four-structure $\{\phi, \psi, 1, -1\}$ via bisection, articulated topologically. Convergent with the algebraic path from the math experiment.

## Dependencies

- [Postulates](../../01-postulates/), [grammar](../../03-the-grammar/), [the process](../../02-the-process/) — the framework's foundation.
- [Dynamics experiment](../dynamics/dynamics.md) — provides the stability requirement (collapse pressure, minimum-cycle requirement). Required for the triangle to be argued as the minimum *stable* structure.
- [Math experiment](../mathematics/) — provides arithmetic and algebra. The bootstrap connects via the four-structure $\{\phi, \psi, 1, -1\}$.

## Commitments

| | Commitment | Forces |
|---|---|---|
| **T1** | Admit nodes, edges, and directedness | Cycles become articulable; witnessing graphs become available. |
| **T2** | The totality admits no internally-disjoint substructures | The two chiralities of the directed 3-cycle must connect at the element level. Connection can be via shared elements *or* via polar relations (which are themselves internal relations). |

Each commitment cascades through all four standing properties (Closure, Polarity, Self-Reference, Internality of Relations).

**A note on iteration as fundamental.** The topology lens depends on iteration (provided by [dynamics](../dynamics/dynamics.md)) for more than the minimum-cycle requirement. Without iteration, polar pairs collapse ([dynamics Topic 01](../dynamics/construction/01-collapse-pressure.md)) and no topological structure persists. The topology articulated here exists as configuration *and* as iteration trajectory — two articulations of the same 6-element substrate, structurally polar-partnered (configuration ↔ process). See Phase II Topics 05–06.

## Planned topics

| Phase | Topics | Generates |
|---|---|---|
| **I — Minimum stable structure** | 01–03 | Triangle (directed 3-cycle); chirality; double triangle |
| **II — Six-element structure** | 04–05 | Double-helix seed; "1" as self-conjugate bridge |
| **III — Bisection and Bootstrap** | 07–08 | Four-structure $\{\phi, \psi, 1, -1\}$ via algebraic bisection of the 6-element substrate; bootstrap verification with cross-lens convergence to math |
| **IV — Advanced topology** | (later) | Hopf fibration, torus, breathing torus |

## Sketched chain

### Phase I — Minimum stable structure

- **[01. The Triangle](construction/01-the-triangle.md)** — given the [dynamics experiment's minimum-cycle requirement](../dynamics/construction/03-minimum-cycle-requirement.md), the smallest topology realizing it is the directed 3-cycle $A \to B \to C \to A$. Forced by minimum-cycle requirement + T1.
- **[02. Chirality](construction/02-chirality.md)** — the directed 3-cycle has intrinsic handedness: $A \to B \to C \to A$ is structurally distinct from $A \to C \to B \to A$. Forced by directedness applied to the 3-cycle, not an additional commitment.
- **[03. The Double Triangle](construction/03-the-double-triangle.md)** — by Polarity at the chirality level, the chiral 3-cycle has its anti-chiral polar partner. Both cycles are present in the totality. The specific embedding relation (disjoint, shared bridge, interleaved) is deferred to Phase II.

### Phase II — Polarity at the node level; the prism and the twisted strand

- **[04. Polarity at the Node Level](construction/04-polarity-at-node-level.md)** — Polarity at the value level forces each node to have its anti-node. The 3 anti-nodes themselves require a witnessing structure, forming an anti-triangle. Total: 6 elements. Polar pairs are *not* witnessed as pairs (avoids infinite regress); each pole is independently witnessed within its own cycle.
- **[05. The Static Prism](construction/05-the-static-prism.md)** — the static spatial configuration of the 6-element double triangle. Two anti-chiral 3-cycles on disjoint node sets, connected by 3 polar matching relations. Structure: the triangular prism graph.
- **[06. The Dynamic Twisted Strand](construction/06-the-dynamic-twisted-strand.md)** — when both cogs iterate in their full polar context (anti-chirality forces opposite rotational directions), the engagement point traces a helical path through all 6 elements. Static prism and dynamic strand are framework-wise polar partners: configuration ↔ process.

### Phase III — Bisection and bootstrap

- **[07. The Bisection](construction/07-the-bisection.md)** — algebraic assignment of the 6 elements: $A \to \phi$, $B \to \psi$, $C \to 1$ in $\alpha$, with polar partners in $\beta$ giving $\{-\phi, -\psi, -1\}$. The four-structure $\{\phi, \psi, 1, -1\}$ emerges as the named subset $\{A, B, C, -C\}$.
- **[08. The Bootstrap](construction/08-the-bootstrap.md)** — verification that the topology experiment regenerates the framework's seed (Conservation, Existence, Internality, four standing properties) in its own vocabulary. Cross-lens convergence with the math experiment's Vieta path established.

### Phase III — Bootstrap

- **06. Four-structure via bisection** — algebraic bisection of the double triangle's vertex structure produces $\{\phi, \psi, 1, -1\}$:
  - $\phi, \psi$ from the two chiral triangles' eigenvalues.
  - $1$ as the self-conjugate bridge.
  - $-1$ as polarity's image of $1$.

  This regenerates the math experiment's four-structure topologically — the bootstrap.

### Phase IV — Advanced topology (later)

Hopf fibration, torus structure with Minkowski metric, breathing torus (antiphase oscillation of the double-helix), spin as breath cycle. Each builds on prior phases plus additional commitments (specifically, embedding into specific dimensions and admitting metric structure).

## Forced vs chosen, in the lens of itself

**Chosen:**

- The lens itself: articulating via topology.
- T1: admitting nodes, edges, and directedness.

**Forced (given the choice + dynamics import):**

- The triangle as minimum stable directed 3-cycle (importing dynamics's minimum-cycle requirement).
- Chirality (intrinsic to the directed cycle).
- The double triangle (Polarity at the structural level forces the anti-chiral twin).
- The six-element structure with self-conjugate bridge (forced by double-triangle composition).
- The four-structure $\{\phi, \psi, 1, -1\}$ via double-triangle bisection (the bootstrap).

## Cross-experiment convergence

The four-structure $\{\phi, \psi, 1, -1\}$ is also produced by the [math experiment's algebra subdomain](../mathematics/algebra/) via Vieta on the self-reference equation. **Two paths converge** on the same structure:

- **Math path:** $x^2 = x + 1$ → $\phi, \psi$ → Vieta gives $\phi + \psi = 1$, $\phi\psi = -1$ → degenerate triple $\phi\psi + (\phi + \psi) = 0$.
- **Topology path:** dynamics's stability requirement → triangle → chirality → double triangle → bisection → four-structure.

Two genuinely independent commitment chains converging on the same forced atom is strong evidence that the four-structure is a **forced atom of the generator itself**, not lens-specific. This is exactly the kind of cross-lens convergence the [transferability principle](../../15-cross-domain-analysis/transferability.md) tracks as evidence of structural forcing.

## Importing this module

Subsequent experiments build on topology. In particular:

- The [physics experiment](../physics/physics.md) imports topology's torus and breathing-torus structures (Phase IV) for its substrate of observables.
- A planned **biology experiment** would import topology for relational structure (cellular boundaries, network connectivity).

## What this experiment does *not* establish

- **Continuous topology** (manifolds, smooth structure). Discrete topology (graph-theoretic) is established here; smooth extension requires additional commitments.
- **Embedding dimension.** The triangle and double triangle are articulated combinatorially, without commitment to the embedding space's dimension. Specific dimensions require specific commitments (3D, 4D, 11D, etc.).
- **Specific knot structures.** Torus knots, Hopf links, etc. are advanced topics that require additional commitments beyond Phase III.
