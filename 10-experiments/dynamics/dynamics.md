# Dynamics

*The lens articulating persistence and change of structures over iteration. States, transitions, fixed points, collapse, stability.*

---

## What this experiment is

Dynamics is a lens of the generator. Once iteration is admitted (forced by [Self-Reference at the operational level](../mathematics/arithmetic/construction/06-iteration-and-time.md#commitment)), structures can be examined for what they do over iteration: which persist, which collapse, which oscillate, which approach fixed points. This experiment articulates that.

The lens has substrate (states + transitions) and articulation (persistence relations, stability conditions). The bootstrap target: dynamics regenerates $\Sigma = 0$ as the limit toward which unwitnessed structure tends.

This file is the **module overview**. Atomic step-by-step articulation will live in `construction/` (not yet populated).

## Status

Phase I complete (Topics 01–03). Phases II–III planned.

## The lens

- **Substrate:** states (configurations a structure can take) and transitions (how one state succeeds another under iteration).
- **Articulation:** persistence relations — what changes vs what is preserved over iteration; what reaches fixed points; what collapses.
- **Bootstrap form:** the dynamical limit. Unwitnessed polar structure approaches $\Sigma = 0$; witnessed structure persists. The seed regenerated as a stability-vs-collapse criterion.

## Dependencies

- [Postulates](../../01-postulates/), [grammar](../../03-the-grammar/), [the process](../../02-the-process/) — the framework's foundation.
- [Math experiment, arithmetic Topic 06 (iteration)](../mathematics/arithmetic/construction/06-iteration-and-time.md) — iteration as forced operational consequence of Self-Reference. Required for dynamics to have something to operate on.

## Commitments

| | Commitment | Forces |
|---|---|---|
| **D1** | Admit dynamic states and transitions over iteration | Persistence and collapse become articulable; fixed-point analysis becomes available. |

That is the dynamics lens's full commitment list. Each commitment cascades through all four standing properties (Closure, Polarity, Self-Reference, Internality of Relations).

## Planned topics

| Phase | Topics | Generates |
|---|---|---|
| **I — Persistence and collapse** | 01–03 | Collapse pressure; two-node instability; minimum-cycle requirement |
| **II — Fixed points** | 04+ | Self-reference fixed points; stability classifications |
| **III — Bootstrap** | (final) | Verification: dynamics regenerates $\Sigma = 0$ at the unwitnessed limit |

## Sketched chain

### Phase I — Persistence and collapse

- **[01. Collapse Pressure](construction/01-collapse-pressure.md)** — an unwitnessed polar pair $\{E, -E\}$ is undifferentiated under iteration. The pair contributes to $\Sigma = 0$ but is not internally articulable as a distinction at any iteration step.
- **[02. Two-Node Instability](construction/02-two-node-instability.md)** — mutual reference between two elements with $B = -A$ has no nonzero fixed point: the negation map's only self-consistent value is zero. Two-element complement-reference fails to witness.
- **[03. Minimum-Cycle Requirement](construction/03-minimum-cycle-requirement.md)** — internal articulation of polar distinction requires at least three elements arranged so the witnessing relation is non-complement at every node. The structural lower bound; the topology experiment imports this to construct the triangle.

### Phase II — Fixed points (later)

Articulation of fixed-point analysis: which iterated maps have stable, attracting, repelling fixed points; what the framework's self-reference equation has in algebraic form; how stability classifications transfer across lenses.

### Phase III — Bootstrap (later)

Verification: the unwitnessed-collapse limit ($\Sigma = 0$) is the seed in dynamics' own vocabulary. The lens regenerates the framework's seed as the asymptotic state of unwitnessed structure.

## Forced vs chosen, in the lens of itself

**Chosen:**

- The lens itself: articulating via dynamics.
- D1: admitting states and transitions over iteration.

**Forced (given the choice):**

- Collapse pressure (Phase I, Topic 01).
- Two-node instability (Phase I, Topic 02).
- Minimum-cycle requirement (Phase I, Topic 03).
- Fixed-point analyses (Phase II — articulation depends on what's expressed but the structural facts are forced).
- The bootstrap (Phase III — verification follows from the chain closing on itself).

## Importing this module

Other experiments that need stability arguments import this module. In particular:

- The [topology experiment](../topology/topology.md) imports the minimum-cycle requirement to argue the triangle is the minimum stable witnessing structure. Without dynamics, the triangle's status as "stable" cannot be argued — the topology experiment alone has no notion of persistence.
- The [physics experiment](../physics/physics.md) imports stability concepts to articulate which configurations correspond to persistent particle-like structures.

## What this experiment does *not* establish

- **Specific topology of stable structures.** Dynamics establishes that some stability requirement holds; it does not specify what shape (triangle, n-cycle, manifold) satisfies it. That is the topology experiment's work.
- **Specific dynamical laws** (Hamiltonian, Lagrangian, equations of motion). Those live downstream — likely in physics, importing dynamics + topology + math.
- **Continuous-time dynamics.** This experiment articulates discrete-iteration dynamics. Continuous extension is a downstream commitment.
