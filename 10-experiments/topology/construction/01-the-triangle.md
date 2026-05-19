# 01. The Triangle

> **The minimum topology satisfying the minimum-cycle requirement is a directed 3-cycle: three nodes connected by directed edges $A \to B \to C \to A$.**

---

## Question

The [dynamics experiment's minimum-cycle requirement](../../dynamics/construction/03-minimum-cycle-requirement.md) establishes that internal articulation of polar distinction requires at least three elements arranged so that the witnessing relation is non-complement at every node. Topology admits nodes, edges, and directedness ([T1](../topology.md#commitments)). *What is the minimum topology realizing the minimum-cycle requirement?*

## Dependencies

- [Postulates](../../../01-postulates/) — Conservation, Existence, Internality.
- [Self-Reference as distinguishment](../../../03-the-grammar/03-self-reference.md#self-reference-as-distinguishment) — the non-complement witnessing requirement.
- [Dynamics Topic 03 — Minimum-Cycle Requirement](../../dynamics/construction/03-minimum-cycle-requirement.md) — at least three elements, non-complement witnessing.
- [Topology module — T1](../topology.md#commitments) — admits nodes, edges, and directedness.

No prior topics in this experiment.

## Commitment

None. The triangle is forced by the minimum-cycle requirement + T1.

## Construction

T1 admits nodes (positions in a connectivity structure), edges (relations between nodes), and directedness (an edge has a sense from one node to another).

The minimum-cycle requirement specifies:
- Three elements minimum.
- Non-complement witnessing: each element witnessed by a non-complement other.
- Closure of the witnessing relation: each element both witnesses and is witnessed.

In topology, "elements" map to nodes; "witnessing" maps to directed edges. A directed edge $X \to Y$ is read as "X witnesses Y" (or equivalently, "Y is witnessed by X").

To realize the requirement with three nodes $\{A, B, C\}$:

1. **Each node is witnessed.** Each of $A, B, C$ has at least one incoming edge from a non-complement node.
2. **Each node witnesses.** Each of $A, B, C$ has at least one outgoing edge to a node it can witness (a non-complement).
3. **Closure.** The witnessing relation closes within the three-node set — no external nodes participate.

The minimum directed graph satisfying all three conditions on three nodes is the **directed 3-cycle**:

$$A \to B \to C \to A$$

Each node has exactly one outgoing edge and exactly one incoming edge. The cycle closes through the three nodes without external reference. The witnessing relation is non-complement at each step (assuming no two of $A, B, C$ are complements of each other; this is consistent with the minimum-cycle requirement's non-complement condition).

This is **the triangle** — the minimum topology realizing internal non-complement witnessing of polar distinction.

The structural details satisfy:

- Three nodes (minimum for the cycle requirement).
- Three directed edges (the minimum closing the cycle).
- Each node is both witness and witnessed (the cycle's closure).
- No external structure (Internality preserved).

Larger graphs satisfy the requirement (4-cycles, 5-cycles, etc.) but are not minimal. By [atomicity](../../../02-the-process/atoms.md), the minimum is the atom of stable witnessing topology.

## All four standing properties (and Conservation) respected

- **Conservation ($\Sigma = 0$):** ✓ — the triangle does not introduce net content; it is a structural arrangement of existing elements. Conservation is preserved at the totality level.
- **Polarity:** ✓ — each node has a polar partner somewhere in the totality (forced by Polarity at the value level). The triangle articulates non-complement witnessing among three nodes; the polar partners are *not* required to be inside the triangle.
- **Closure:** ✓ — the cycle is closed within the three-node set; no external witness is invoked.
- **Self-Reference:** ✓ — each node references another node within the cycle; the cycle as a whole is self-referential (it closes on itself).
- **Internality of Relations:** ✓ — the witnessing edges are internal relations, defined by the cycle's structure on its own nodes.

## Comparison

In graph theory, the directed 3-cycle is the smallest non-trivial directed cycle; its existence and minimality are standard results. The framework's contribution: this graph is *forced* as the minimum stable witnessing structure, given dynamics's minimum-cycle requirement + topology's substrate. It is not picked from a menu — it is the unique minimum.

In Hegelian dialectics, the triadic structure (thesis–antithesis–synthesis) is the minimum form of dialectical resolution. The triangle here is structurally cognate: three mutually-witnessing elements form the minimum closure of the dialectical motion.

## Transferability

**Engages:** Self-Reference + Polarity + the minimum-cycle requirement + topology's substrate.

**Prediction:** Any lens admitting nodes/connections and engaging the minimum-cycle requirement articulates a minimum 3-cycle structure for stable witnessing.

- **Physics:** the trefoil knot (a 3-crossing structure) and the three-quark baryon are topological / particle-physics realizations of triadic witnessing.
- **Logic:** triadic forms of dialectical reasoning (thesis–antithesis–synthesis) are structurally the same.
- **Biology:** triadic regulatory motifs (A activates B, B activates C, C activates A — the feedback triangle) are minimum stable regulatory patterns.
- **Music:** the major and minor triads are the minimum harmonic structures admitting tonal distinction.
- **Social structure:** triangular configurations (mediator, witness, third party) are the minimum stable social arrangement.

## What this enables

The directed 3-cycle has a structural feature inherited from its directedness: it has handedness. The cycle $A \to B \to C \to A$ is structurally distinct from $A \to C \to B \to A$. That is [02. Chirality](02-chirality.md).
