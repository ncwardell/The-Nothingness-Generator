# 05. The Static Prism

> **The static configuration of the 6-element double triangle is the triangular prism: two anti-chiral 3-cycles on disjoint node sets, connected by 3 polar matching relations.**

---

## Question

[Topic 04](04-polarity-at-node-level.md) established that Polarity at the node level forces 6 elements (3 nodes + 3 anti-nodes), with each cycle witnessing internally and polar relations connecting them as Conservation balance. *What is the static spatial configuration of these 6 elements as a structural graph?*

## Dependencies

- [01. The Triangle](01-the-triangle.md) — directed 3-cycle structure.
- [02. Chirality](02-chirality.md) — directed cycles have intrinsic handedness.
- [03. The Double Triangle](03-the-double-triangle.md) — both chiralities are present.
- [04. Polarity at the Node Level](04-polarity-at-node-level.md) — 6 elements forced; cycles on disjoint node sets; polar relations connect them as Conservation balance, not witnessing.

## Commitment

None. The static prism is forced by Topic 04's structure articulated as a graph.

## Construction

The 6 elements from [Topic 04](04-polarity-at-node-level.md) are $\{A, B, C, -A, -B, -C\}$. The relations:

- **Triangle $\alpha$** on $\{A, B, C\}$: directed 3-cycle, say $A \to B \to C \to A$ (one chirality).
- **Anti-triangle $\beta$** on $\{-A, -B, -C\}$: directed 3-cycle of the *opposite* chirality (forced by [Topic 03](03-the-double-triangle.md)). Say $-A \to -C \to -B \to -A$.
- **Polar matching** between corresponding nodes: $A \leftrightarrow -A$, $B \leftrightarrow -B$, $C \leftrightarrow -C$. Three relations, structural balance only — *not* witnessing edges.

Drawn as a graph:

| Element | Within-cycle edges | Polar relation |
|---|---|---|
| $A$ | $A \to B$ (out), $C \to A$ (in) | $A \leftrightarrow -A$ |
| $B$ | $B \to C$ (out), $A \to B$ (in) | $B \leftrightarrow -B$ |
| $C$ | $C \to A$ (out), $B \to C$ (in) | $C \leftrightarrow -C$ |
| $-A$ | $-A \to -C$ (out), $-B \to -A$ (in) | $A \leftrightarrow -A$ |
| $-B$ | $-B \to -A$ (out), $-C \to -B$ (in) | $B \leftrightarrow -B$ |
| $-C$ | $-C \to -B$ (out), $-A \to -C$ (in) | $C \leftrightarrow -C$ |

Counts:
- 6 nodes
- 6 directed cycle edges (3 per triangle)
- 3 polar relations (undirected, or equivalently 6 directed with both directions, since polar is bidirectional structural balance)
- Treating polar relations as undirected: **9 undirected edges total**, each vertex degree 3.

This is the **triangular prism graph** $Y_3$ — a well-known 3-regular graph on 6 vertices, planar, with girth 3 (the two original triangles).

### The cogs metaphor

Visualize the prism in 3D: two parallel triangles aligned on a common axis, with corresponding vertices connected by polar matching "rungs." Each triangle is a "cog" (a closed cycle). The polar matching is the set of contact points between the cogs.

The two cogs are **anti-chiral**: if $\alpha$ traverses $A \to B \to C \to A$ in one rotational sense, $\beta$ traverses $-A \to -C \to -B \to -A$ in the opposite rotational sense. The polar matching connects each $\alpha$-tooth to its corresponding $\beta$-tooth (the negation partner).

This is the **static configuration**: the spatial arrangement of the 6 elements as a structural graph at a single "moment." It does not yet articulate what the structure does over iteration — that is the work of [Topic 06](06-the-dynamic-twisted-strand.md).

### T2 satisfied via polar matching

The two cycles share no nodes. By [T2](../topology.md#commitments) (no internally-disjoint substructures), they must connect at the element level. The polar matching provides the connection: each $X$ is internally related to $-X$ by Polarity. T2 is satisfied through structural relations (Conservation balance), not through shared witnessing edges.

## All four standing properties (and Conservation) respected

- **Conservation ($\Sigma = 0$):** ✓ — the polar matching is the structural articulation of Conservation across the two cycles. The 6 elements sum to zero (3 polar pairs each summing to zero).
- **Polarity:** ✓ — both at node level (each $X$ paired with $-X$) and at chirality level (the two cycles anti-chiral).
- **Closure:** ✓ — the prism is internally complete; all witnessing happens within cycles, all polar relations are internal Conservation balances.
- **Self-Reference:** ✓ — each cycle is self-referential (closes on itself); each element is witnessed within its cycle.
- **Internality of Relations:** ✓ — both within-cycle witnessing relations and cross-cycle polar relations are internal to the totality.

## Comparison

In graph theory, the triangular prism $Y_3$ is the simplest non-trivial prism graph and one of the most studied 3-regular structures. It is also the 1-skeleton of the triangular prism polyhedron. The framework's contribution: this graph is *forced* as the static configuration of the 6-element double triangle, with specific roles for each edge type (within-cycle = witnessing; polar matching = Conservation balance).

In knot theory, two parallel oriented cycles connected by a perfect matching is a basic building block — a "ladder" or "prism link." The framework's structure is the directed-graph analog.

## Transferability

**Engages:** the full Phase I cascade + Polarity at node level + cycle structure.

**Prediction:** Any lens with the 6-element double-triangle structure articulates a prism-like static configuration: two anti-chiral cycles connected by polar matching.

- **Chemistry:** stereoisomeric pairs (left/right enantiomers) within a molecule's structure form prism-like configurations when their atomic positions are mirror-paired across a plane.
- **Music:** parallel modal pairs (e.g., major/minor on the same root) share certain pitch elements in mirror positions, forming a prism-like harmonic configuration.
- **Physics:** matter and antimatter cosmologies, when articulated topologically, would have prism-like configurations with corresponding particle-antiparticle pairs as the polar matching.

## What this enables

The static prism articulates the configuration. But the topology lens depends on iteration to persist (collapse pressure). The next topic articulates what the structure *does* under iteration: [06. The Dynamic Twisted Strand](06-the-dynamic-twisted-strand.md). Static prism and dynamic strand are framework-wise polar partners — configuration ↔ process.
