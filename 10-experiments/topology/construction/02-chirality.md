# 02. Chirality

> **The directed 3-cycle has intrinsic handedness: $A \to B \to C \to A$ is structurally distinct from $A \to C \to B \to A$. Chirality is forced by directedness, not added as a separate commitment.**

---

## Question

[Topic 01](01-the-triangle.md) established the directed 3-cycle as the minimum stable witnessing topology. The cycle is *directed* — each edge has a sense from one node to another. *Is the cycle's sense itself a structural feature, or arbitrary labeling?*

## Dependencies

- [01. The Triangle](01-the-triangle.md) — the directed 3-cycle.
- [Topology module — T1](../topology.md#commitments) — directedness is part of the substrate.
- [Polarity (weak form)](../../../03-the-grammar/02-polarity.md) — preserved structurally; chirality's polar partner forced in [Topic 03](03-the-double-triangle.md).

## Commitment

None. Chirality is forced by directedness applied to the 3-cycle.

## Construction

Consider the directed 3-cycle on nodes $\{A, B, C\}$. Two distinct directed cycles are possible:

- **Cycle $\alpha$:** $A \to B \to C \to A$
- **Cycle $\beta$:** $A \to C \to B \to A$

These are the only two directed cycles on three nodes that include all three nodes (the cycle must visit each node exactly once and return). They differ in the *order of traversal*.

Cycle $\alpha$ and cycle $\beta$ are related by **edge-reversal**: every edge in $\alpha$ has its reverse in $\beta$. There is no continuous deformation within the directed-graph substrate that converts one to the other without reversing edges.

This structural distinction is **chirality** (handedness). The two cycles are enantiomers — mirror images that cannot be superimposed by any operation preserving directedness.

Chirality is *intrinsic* to the directed 3-cycle:

1. **Forced by directedness.** Once T1 admits directed edges, a 3-cycle has two distinguishable senses. The choice of direction is not an additional commitment; the direction itself is part of what T1 articulates.
2. **Not additional structure.** Chirality is not a property *added* to the triangle. It is what directedness *is* when applied to the 3-cycle topology.
3. **Atomic.** The two chiralities are the irreducible distinct cycles on three directed nodes; no further decomposition produces additional chiralities at this level.

## All four standing properties (and Conservation) respected

- **Conservation ($\Sigma = 0$):** ✓ — chirality is a structural property of the cycle, not a contribution to the conservative sum.
- **Polarity:** chirality is itself polar — the two enantiomers $\alpha$ and $\beta$ are the polar pair. Their polar partnership is articulated in [Topic 03](03-the-double-triangle.md).
- **Closure:** ✓ — the two chiralities are internal to the directed-graph substrate; no external orientation is imposed.
- **Self-Reference:** ✓ — the cycle's sense is self-defined by its internal directedness; reading the cycle requires referencing its own structure.
- **Internality of Relations:** ✓ — the relation between the two chiralities (edge-reversal) is internal.

## Comparison

In knot theory, chirality distinguishes a knot from its mirror image. The trefoil knot is chiral — left-handed and right-handed trefoils are not isotopic. The framework's directed 3-cycle has the same structural form: handedness intrinsic to the directed structure.

In chemistry, chirality is foundational for asymmetric synthesis and stereoisomerism. Mirror-image molecules with the same constituents have different properties because of intrinsic handedness — structurally analogous to the triangle's two enantiomers.

## Transferability

**Engages:** Polarity + Self-Reference + directedness applied to the minimum cycle.

**Prediction:** Any lens with directed minimum-stable structures articulates two distinct enantiomers, related by edge-reversal but not equivalent.

- **Physics:** parity violation in weak interactions; left-handed neutrinos and right-handed antineutrinos. The chirality is structural, not arbitrary.
- **Chemistry:** stereoisomers with opposite handedness exist for any chiral molecule; biological molecules (amino acids, sugars) exhibit this asymmetry.
- **Biology:** the double helix of DNA is right-handed (B-form); its mirror image (Z-form, left-handed) exists structurally but is not the standard biological form.
- **Music:** ascending vs descending modes of the same triadic structure differ in tonal sense.

## What this enables

The directed 3-cycle has two chiralities. By Polarity, every non-trivial structure has a compensating contribution — chirality cannot exist alone without its polar partner. The anti-chiral twin is forced. That is [03. The Double Triangle](03-the-double-triangle.md).
