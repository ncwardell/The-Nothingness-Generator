# Experiments

*The generator articulating itself through specific lenses.*

---

## What an experiment is

Each subfolder is an experiment: a particular lens through which the generator articulates its own structure. The "domain" of an experiment is a slice of the totality; the experiment is the totality articulating itself in the form that slice provides.

This reframe is not stylistic. By [Internality](../01-postulates/internality.md), there are no external objects to apply a tool to. By [Self-Reference](../03-the-grammar/03-self-reference.md), the generator's articulation through any domain is also the generator articulating itself. So an experiment is not "us using the framework on the domain." It is "the framework expressing its structure in the form the domain provides."

What this means in practice:

- A **hit** is the generator recognizing its own structure in the lens.
- A **miss** is the lens not admitting the form being attempted; the experiment must revise its commitments or assignments.
- A **silence** is the lens not engaging the structural feature being attempted.

Single experiments produce one self-portrait of the generator. [Cross-domain analysis](../15-cross-domain-analysis/) examines multiple self-portraits at once, to find what is invariant.

## Anatomy of an experiment

Every well-formed experiment is structured as:

- A **module file** at the experiment root (named after the lens, e.g., `arithmetic.md`). This lists dependencies, commitments, what the experiment produces, and is the entry point other experiments can reference when "importing" this one.
- A **construction subfolder** containing **atomic topic files** in numbered sequence. Each topic file is one atomic move in the chain.
- A **bootstrap topic** at the end of the chain that verifies the lens articulates the framework's seed in its own vocabulary (the success condition).

Each topic file follows the same structure (statement, question, dependencies, commitment, construction, four-property check, comparison, transferability, what-this-enables). See [`topic-template.md`](topic-template.md) for the canonical template and discipline checklist.

## The substrate / articulation requirement

By the [Universal Bootstrap Principle](../02-the-process/self-bootstrap.md#the-universal-bootstrap-principle), every experiment must contain two layers:

- **Substrate** — the lens's specific objects, values, primitives.
- **Articulation** — the language for expressing structural relations among them.

The bootstrap happens in the articulation, not the substrate. Without an articulation language, a lens cannot bootstrap.

For the mathematics experiment, the substrate is *arithmetic* (specific values, operations, integer generation) and the articulation is *algebra* (variables, equations, structural identities). The bootstrap lives in algebra.

For every other experiment, both layers must be identified explicitly:

- Physics: substrate of observables; articulation of equations / dynamical laws.
- Language: substrate of vocabulary; articulation of grammar / syntax.
- Biology: substrate of molecules and structures; articulation of interactions / metabolic relations.

The substrate and articulation may live in separate subdomains (as arithmetic and algebra do within mathematics), or be developed together. Either way, both must exist, and the bootstrap must live in the articulation.

## The algebraic package as canonical template

The arithmetic+algebra package is the framework's first bootstrap-verified lens. It is therefore the **canonical structural template** for every other lens. Numbers and operations in the package are not exclusively mathematical objects — they are structural positions that any lens fills with its own content.

When generating a new experiment, don't start from scratch. Use the algebraic package as the template: identify what fills each position (polar pair, unit of distinction, zero, addition, iteration, Fibonacci-analog, self-reference equation, eigenvalues, bootstrap) in your lens. The shape is universal; the content is lens-specific.

See [`15-cross-domain-analysis/transferability.md`](../15-cross-domain-analysis/transferability.md#the-algebraic-package-as-canonical-structural-template) for the full template and how to apply it.

**Specific assignments are revisable hypotheses.** If a guess turns out wrong, the experiment is revised. The strict [grammar](../03-the-grammar/) and the [generator's method](../02-the-process/) stand independently of any specific experiment.

## Foundational lenses vs. test lenses

Lenses divide into two kinds (full treatment in [`mutual-reinforcement.md`](../15-cross-domain-analysis/mutual-reinforcement.md)):

**Foundational lenses** — essential to the framework's operation. Without them, something the framework needs is unarticulated.

- **Mathematics (algebra)** — the framework's methodology is itself algebraic; without algebraic articulation, the framework cannot describe how it operates.
- **Language (narrative)** — the framework needs to be communicable; without narrative articulation, it cannot be transmitted or grasped beyond pure structure.
- **Logic** — currently articulated implicitly in [`00-orientation/logical-foundation.md`](../00-orientation/logical-foundation.md); could become an explicit experiment.
- **Awareness / phenomenology** — currently articulated implicitly in [`02-the-process/the-empathic-mode.md`](../02-the-process/the-empathic-mode.md); could become an explicit experiment.

**Test lenses** — domains the framework can be applied to as empirical tests. Each successful test-lens bootstrap is empirical evidence of the framework's reach.

- Physics, biology, music, ethics, social structure, etc.

The framework's individual bootstrap doesn't *require* any specific test lens to verify. The foundational lenses cover what the framework *needs* to operate. The test lenses cover where the framework can be *applied* and tested.

## Current and planned experiments

| Experiment | Module file | Type | Status |
|---|---|---|---|
| **mathematics** | [`mathematics.md`](mathematics/mathematics.md) | Foundational | Bootstrap-verified |
| **language** | [`language.md`](language/language.md) | Foundational | Bootstrap-verified |
| **dynamics** | [`dynamics.md`](dynamics/dynamics.md) | Foundational | Phase I complete (Topics 01–03) |
| **topology** | [`topology.md`](topology/topology.md) | Foundational | Bootstrap-verified (Topics 01–08) |
| **physics** | [`physics.md`](physics/physics.md) | Test | Initial port — Phase I in progress |
| biology | *(planned)* | Test | Planned |

**Mathematics:** arithmetic ([`arithmetic.md`](mathematics/arithmetic/arithmetic.md)) as substrate, algebra ([`algebra.md`](mathematics/algebra/algebra.md)) as articulation. The bootstrap lives in algebra. The combined package is the canonical structural template.

**Language:** vocabulary (Loshi) as substrate, narrative composition as articulation. The bootstrap takes the form of a creation narrative.

**Dynamics** *(Phase I complete):* states + transitions as substrate, persistence relations as articulation. Phase I articulates collapse pressure (Topic 01), two-node instability (Topic 02), and the minimum-cycle requirement (Topic 03) for stable witnessing structure. Provides the stability requirement that the topology experiment imports. Phases II (fixed-point analyses) and III (bootstrap) are planned.

**Topology** *(bootstrap-verified):* nodes + edges + directedness as substrate, cycles + witnessing graphs as articulation. Phases I-III complete: triangle (minimum stable structure), chirality, double triangle, polarity at node level (forcing 6 elements), static prism (configuration), dynamic twisted strand (iteration trajectory), bisection (algebraic assignment), and bootstrap (verification with cross-lens convergence). The four-structure $\{\phi, \psi, 1, -1\}$ is produced by topology's bisection path AND by math's Vieta path — the framework's first substantive cross-domain convergence.

**Physics:** observables (particle masses, fundamental constants) as substrate, dynamical laws and depth/coupling formulas as articulation. Imports the math+algebra package and (when articulated) the topology experiment's torus structures. Adds physics-specific commitments: torus topology, breathing dynamics, meeting-point lattice, depth/coupling structure for particles. The first scientific test of the [strong hypothesis](../15-cross-domain-analysis/the-strong-hypothesis.md).

**Biology** *(planned):* molecules and structures as substrate, interactions / metabolic relations as articulation. Builds on the mathematics package and possibly imports Loshi vocabulary.

Each experiment lives in its own subfolder with its own module file and atomic topic chain.

## How experiments relate

Experiments are *not* required to share commitments. Different lenses may need different additional commitments. Where experiments share commitments, the shared structure is a candidate for promotion to framework-level (see [`15-cross-domain-analysis/`](../15-cross-domain-analysis/)). Where they diverge, the divergence is informative — it indicates which commitments are lens-specific.

The framework's broadest claim is that the *generator* is universal; specific commitments and assignments are not. Productivity across multiple experiments using related but not identical commitments is the strongest form of evidence.

## Adding a new experiment

1. Create a subfolder named for the lens.
2. Write a README following the anatomy above.
3. Make commitments and assignments explicit before tracing any consequences.
4. Maintain forced-vs-chosen discipline throughout.
5. Document hits, misses, and silences honestly.

The experiment is the unit of empirical work. The framework earns credibility through consistent generative success across diverse lenses. Single experiments are anecdotal; patterns across experiments — examined in [`15-cross-domain-analysis/`](../15-cross-domain-analysis/) — are evidence.
