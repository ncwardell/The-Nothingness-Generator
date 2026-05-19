# Experiment: Mathematics

*The generator articulating itself through the lens of mathematics.*

---

## What this experiment is

This experiment unfolds the generator through mathematical articulation. Mathematics is composed of subdomains — arithmetic, geometry, algebra, analysis, topology, and so on — each requiring its own commitments. This experiment treats each subdomain as a separate articulation track.

## Methodological discipline

Every move in this experiment must respect **all** of the framework's structural rules:

**The postulates:**
- **Conservation** ($\Sigma = 0$): moves preserve the conservative sum.
- **Existence** ($\exists$): moves produce non-trivial structure.
- **Internality** (no outside): nothing introduced lives outside the totality.

**The four standing properties:**
- **[Closure](../../03-the-grammar/01-closure.md)**: new values and operations stay within the totality, or extend it *internally*.
- **[Polarity](../../03-the-grammar/02-polarity.md)**: every element has a polar complement; every operation has a polar partner.
- **[Self-Reference](../../03-the-grammar/03-self-reference.md)**: new structure is articulable from within.
- **[Internality of Relations](../../03-the-grammar/04-internality-of-relations.md)**: relations among new structures are themselves internal.

Three operating rules:

1. **Respect all four standing properties.** Each topic file checks the move against each.
2. **Atomicity.** Each topic file is one atomic move. No bundling.
3. **Forced over chosen.** Commitments minimized; consequences cascade through *all four* standing properties automatically.

A particular consequence: **Closure under operations forces self-referential generation.** When an operation produces a value not yet in the totality, the value cannot be externally posited (that violates Closure). It must emerge from within via a self-referential generative process. This is why integer generation uses Fibonacci+Zeckendorf rather than external successor.

## Subdomains

| Subdomain | Module file | Status | What it articulates |
|---|---|---|---|
| **Arithmetic** | [`arithmetic/arithmetic.md`](arithmetic/arithmetic.md) | Complete | Polar primitives, operations, integer generation via Fibonacci+Zeckendorf — the substrate |
| **Algebra** | [`algebra/algebra.md`](algebra/algebra.md) | Complete | Self-reference equation, eigenvalues, Vieta, the degenerate triple, the complex unit — and the bootstrap |
| **Geometry** | *(planned)* | Planned | Spatial structure on top of arithmetic+algebra |
| **Analysis** | *(planned)* | Planned | Limits, continuity, infinite processes |
| **Topology** | *(planned)* | Planned | Topological structure |
| **Abstract algebra** | *(planned)* | Planned | Groups, rings, fields, beyond the elementary arithmetic+algebra package |

Each subdomain is structured as a referenceable module:

- A **module file** at the subdomain root (named after the subdomain — e.g., `arithmetic.md`, not `README.md`). Lists dependencies, commitments, what is produced, and is the entry point for other subdomains importing it.
- Atomic topic files in a `construction/` subfolder, each self-isolated with dependencies linked. See [`../topic-template.md`](../topic-template.md) for the canonical topic file structure.

## Arithmetic and algebra: the foundational pair

**Arithmetic** is the substrate: specific values, specific operations, specific compositions (the integers via Fibonacci+Zeckendorf).

**Algebra** is the articulation language: variables, equations, abstract identities. Algebra builds on arithmetic and articulates the structural relations among arithmetic objects.

The framework's seed is *articulated* by algebra (the bootstrap happens there), not by arithmetic alone. Arithmetic provides the substrate; algebra speaks the framework's own articulation language. This is why the bootstrap lives in algebra: the framework's methodology is itself algebraic in character.

The combined **arithmetic+algebra package** is what bootstraps. Each subsequent subdomain imports both.

## Status

The arithmetic subdomain has Phases I, II, and III complete; Phase IV is in progress. See [`arithmetic/arithmetic.md`](arithmetic/arithmetic.md) for the detailed chain.

Substantial commitments beyond arithmetic — torus topology, breathing dynamics, a meeting-point lattice — belong in [`10-experiments/physics/`](../physics/), not here. The mathematical chain in this experiment provides the substrate that physics builds on.
