# 03. Minimum Cycle Requirement

> **Internal articulation of polar distinction requires at least three elements, arranged so that the witnessing relation is non-complement at every node.**

---

## Question

[Topic 01](01-collapse-pressure.md) established that polar pairs require non-complement internal witnessing for distinction. [Topic 02](02-two-node-instability.md) established that two elements alone fail — mutual reference between complements has no distinction-bearing fixed point. *What is the minimum number of elements in a system that admits internal articulation of polar distinction?*

## Dependencies

- [01. Collapse Pressure](01-collapse-pressure.md) — non-complement witness required for distinction.
- [02. Two-Node Instability](02-two-node-instability.md) — two elements alone fail.
- [Polarity (weak form)](../../../03-the-grammar/02-polarity.md) — every non-zero element has compensating contribution.
- [Self-Reference as distinguishment](../../../03-the-grammar/03-self-reference.md#self-reference-as-distinguishment) — the non-complement witnessing requirement.

## Commitment

None. The minimum-cycle requirement is forced by Topics 01 and 02 + Self-Reference as distinguishment.

## Construction

Consider candidate systems of $n$ elements admitting internal polar distinction:

**$n = 1$.** A single element $A$ does not satisfy Polarity, which requires a compensating contribution somewhere. Without the polar-pair structure, there is no distinction to articulate at all. Excluded.

**$n = 2$.** A polar pair $\{A, -A\}$ is the minimum satisfying Polarity. By [Topic 02](02-two-node-instability.md), mutual reference between the pair fails to articulate distinction — the only fixed point of the restricted negation map is zero. Excluded.

**$n = 3$.** Consider a system $\{A, B, C\}$ where the elements are so arranged that no element is the complement of another *within the system's witnessing relation*. Each element has at least one non-complement other available as witness.

For the three-element system to admit internal polar distinction:

1. **Conservation at the system level.** The contributions sum to zero (Polarity at the totality level — the three-element subsystem's net contribution is balanced by the rest of the totality, or the three are themselves the relevant slice and sum to zero internally).
2. **Non-complement witnessing.** No witnessing relation pairs an element with its own complement. Each element is witnessed by a non-complement other.
3. **Closure of the witnessing relation.** Each element witnesses another; the relation closes within the three-element set.

The minimum configuration satisfying all three is achievable with $n = 3$: a three-element system where the witnessing relation pairs each element with a non-complement third. The structural details (whether the relation is a directed 3-cycle, an undirected triangle, or another arrangement; how the elements relate algebraically) are the work of the [topology experiment](../../topology/topology.md), which imports this requirement.

For $n \geq 3$ with appropriate structure, internal polar distinction is admissible. **Three is the lower bound.**

The **minimum-cycle requirement**: internal articulation of polar distinction requires at least three elements arranged so that the witnessing relation is non-complement at every node.

## All four standing properties (and Conservation) respected

- **Conservation ($\Sigma = 0$):** ✓ — the requirement is consistent with Conservation. The three-element system's contributions are balanced (either internally or in conjunction with the larger totality, depending on the experiment that instantiates the requirement).
- **Polarity:** ✓ — the requirement is articulated relative to polar pairs and their need for distinction-bearing witnessing.
- **Closure:** ✓ — the requirement is internal; the witnessing relation is among the system's own elements, no external scaffolding.
- **Self-Reference:** ✓ — directly engages Self-Reference as distinguishment; the requirement *is* the distinguishment requirement at minimum cardinality.
- **Internality of Relations:** ✓ — the witnessing relation is internal to the three-element system.

## Comparison

In graph theory, the smallest non-trivial directed cycle has three nodes ($A \to B \to C \to A$). The framework's contribution: the 3-element minimum is *forced* by Self-Reference as distinguishment + Polarity + the failure of one-element and two-element systems. The triangle in graph theory matches the structural requirement; the [topology experiment](../../topology/topology.md) articulates the directed-cycle structure as the canonical satisfier.

## Transferability

**Engages:** Polarity + Self-Reference + the failure modes of one-element and two-element systems.

**Prediction:** Any lens engaging polar pairs and internal witnessing has a minimum-cardinality requirement of three for stable distinction. Lens-specific articulations:

- **Physics:** the smallest stable bound states involve three constituents (three-quark baryons; matter requires more than a particle-antiparticle pair to persist as distinct).
- **Logic:** classical bivalent logic ($\{T, F\}$ alone) cannot ground itself; meta-logical structure or a third value is required.
- **Biology:** stable biological signaling involves at least three roles (transmitter, signal, receiver); two-role systems of mutual-recognition between complements do not constitute stable signaling.
- **Social structure:** dyadic mutual-reference relations between roles defined as opposites lack the internal witnessing for sustained distinction; triangular configurations (with a non-complement third) are the minimum.

## What this enables

The minimum-cycle requirement establishes the structural lower bound for polar distinction. This requirement is the dependency that the [topology experiment](../../topology/topology.md) imports to argue that the directed 3-cycle (the triangle) is the minimum stable witnessing structure.

This concludes **Phase I of the dynamics experiment** — the persistence-and-collapse layer is articulated:

- Polar pairs without witnesses are undifferentiated (Topic 01).
- Two-element mutual complement-reference fails to witness (Topic 02).
- Minimum cardinality for internal polar distinction is three (Topic 03).

Phase II (planned) will articulate fixed-point analyses for self-referential maps, with reference to the [math experiment's algebra subdomain](../../mathematics/algebra/) where the self-reference equation $x^2 = x + 1$ has eigenvalues $\phi, \psi$. Phase III (planned) will articulate the bootstrap — that the unwitnessed limit $\Sigma = 0$ is the seed regenerated in dynamics' own vocabulary.
