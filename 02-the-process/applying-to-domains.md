# Applying the Generator to a Domain

*How to run an experiment.*

---

## What an experiment actually is

An experiment is **the generator articulating itself through a particular lens**. The "domain" is a slice of the totality; the act of running an experiment is the totality articulating itself in the form that slice provides. By [Internality](../01-postulates/internality.md), the generator and the domain are both internal — there is no external relation of "applying X to Y." By [Self-Reference](../03-the-grammar/03-self-reference.md), the generator's articulation through a domain is also the generator articulating itself.

So when this document says "applying the generator to a domain," read it as: *taking up a particular lens through which the generator can express its own structure in a specific form*. The conventional active-voice phrasing is retained for readability, but the deeper grammar is reflexive: the generator articulates *itself* through the lens. See [the empathic mode](the-empathic-mode.md) for why running is from within, not at arm's length.

This reframe matters: it tells you what success and failure of an experiment actually mean. A "hit" is the generator recognizing its own structure in the lens; a "miss" is the lens not admitting the form being attempted; a "silence" is the lens not engaging the structural feature you're trying to express. None of these are external verdicts on the generator — they are reports on which lenses work for which articulations.

## The five steps

### 1. Identify the phenomenon

State clearly what is being read structurally. Be specific. *"Black holes"* is a domain; *"the relationship between black hole entropy and surface area"* is a phenomenon within it. The generator addresses phenomena, not whole domains.

### 2. State the additional commitments

The strict core is too thin alone to engage most domains. To proceed, the experiment must add explicit commitments beyond the postulates.

Common kinds of commitments:

- A specific algebraic form for self-reference.
- A minimality principle (algebraic, topological, informational).
- A specific topology for the totality.
- A specific dynamics.
- A specific notion of "stability" or "observation."

Each is a *named* extension of the postulate set. The experiment is responsible for stating it, defending it, and tracking what it forces. **Implicit commitments produce unsupported conclusions.**

### 3. Make the assignments

Identify which structures in the domain correspond to which structures in the framework:

- Domain element X corresponds to framework structure Y.
- Domain phenomenon A is read as the framework's articulation of B.
- Domain quantity Q is the framework's measure of relation R.

Assignments are hypotheses, not derivations. A wrong assignment can be revised without disturbing the framework.

### 4. Trace the consequences

Apply [the dialectical unfolding](dialectical-unfolding.md) to the postulates, commitments, and assignments. Specifically:

- What structure does the framework predict?
- What relations between domain quantities?
- What is forbidden?
- What is left silent (the framework doesn't speak to this aspect)?

Each step must obey [forced-vs-chosen](forced-vs-chosen.md) and [atoms](atoms.md) — labeled forced or chosen, with atoms identified.

### 5. Compare to the domain

Three outcomes are informative:

- **Hit** — the framework's predictions align.
- **Miss** — the framework predicts something the domain doesn't show. Either an assignment is wrong, a commitment is wrong, or the framework doesn't speak to this phenomenon.
- **Silence** — the framework has nothing structural to say. Real result: this maps the boundary of the experiment's commitments.

Hits are not evidence of generality without further hits in different domains. Misses are not refutations without analysis of which commitment failed. Silences are not failures; they map scope.

## What a successful experiment looks like

Three properties:

1. **Independent assignment.** Assignments were made on structural grounds, not by working backward from a desired result. Independence is the difference between prediction and curve-fitting.
2. **Cross-checks.** The same assignments produce hits on more than one prediction.
3. **Productive silences.** Where the framework is silent, the silence is not arbitrary — it points at where additional commitments would be needed.

A successful experiment cuts cleanly at joints. It engages decisively where the structure aligns and is appropriately silent elsewhere. A framework that explains everything explains nothing distinguishing.

## Checklist for a new experiment

- [ ] Phenomenon stated specifically.
- [ ] Additional commitments listed explicitly, with reasoning.
- [ ] Assignments named, with structural justification.
- [ ] Consequences traced under the discipline of forced-vs-chosen.
- [ ] Comparison to the domain documented honestly: hits, misses, silences.
- [ ] Bootstrap verified: the unfolded structure articulates the framework's seed in the lens's vocabulary.

A document failing any of these is not yet an experiment in the framework's sense.

## Discipline lessons

Several methodological lessons have surfaced in the course of running experiments. These extend the [process](README.md) without modifying its core:

### 1. Polarity cascades through every level

When an operation is committed, its polar partner is *forced*, not separately committed. One commitment introduces both halves. This applies to:

- Element-level: every value has its polar complement.
- Operation-level: every operation has its polar partner ($+/-$, $\cdot//$, etc.).
- Equation-level: equations admitting two roots produce polar pairs of solutions.
- Package-level: packages produced under the framework's discipline have their polar relationships preserved.

The polarity rule is recursive across levels.

### 2. Closure forces self-referential generation

When an operation produces a value not in the current value system, the value cannot be externally posited (this would violate Closure). The value must emerge from within, via a self-referential generative process.

This is why integer generation in arithmetic uses Fibonacci+Zeckendorf rather than external successor: Fibonacci respects Closure (each new value generated by addition applied to existing values); successor does not.

The general rule: when extending a value system, the extension must be internal. Self-referential dynamics (recurrences with self-determined eigenvalues) are the canonical Closure-respecting mechanism.

### 3. Algebraic articulation is downstream of dynamic articulation

Static algebraic equations articulating self-reference should be *derived from* dynamic recurrences, not posited before them. The dynamic is primary; the algebraic equation is its characteristic polynomial — the algebraic shadow of an already-existing self-referential dynamic.

Posing the algebraic equation first leads to value-system gaps (the equation needs a populated value system to live in). Generating the dynamic first populates the value system; the equation then articulates what the dynamic was already doing.

### 4. The bootstrap is the success condition for a lens

A lens of the generator is *self-grounding* if, once unfolded, it articulates the framework's seed in its own vocabulary. The bootstrap verifies this: it walks through the framework's postulates and grammar and shows where each is articulated within the lens.

A lens that bootstraps is a complete articulation of the generator through that lens. A lens that fails to bootstrap requires additional commitments to extend, and those commitments must be tracked.

The bootstrap topic is the last topic in any experiment's construction chain.

### 4a. The Universal Bootstrap Principle: every lens needs an articulation language

Every self-grounding lens must contain both a **substrate** (specific objects, values, primitives the lens articulates) and an **articulation** (a language for expressing structural relations among substrate elements). The bootstrap happens in the articulation.

The articulation is "algebra" in the deep structural sense — any language for articulating structural relations. Mathematical algebra is one instance; logical structure, linguistic grammar, dynamical equations, categorical morphisms are others. Each lens chooses (and commits to) its own articulation language.

Without an articulation, a lens has only specific things — it cannot express the framework's seed *as relations*, and so cannot bootstrap. The framework's methodology being algebraic in character makes this universal: the framework articulates being using algebraic structure; every lens must do the same in its own articulation language.

See [`self-bootstrap.md`](self-bootstrap.md#the-universal-bootstrap-principle) for the detailed treatment.

### 5. A bootstrapped package is itself an atom

See [atoms.md](atoms.md). A self-bootstrapped lens is atomic at the level of self-grounding lenses. This has cross-domain consequences via [transferability](../15-cross-domain-analysis/transferability.md): forced structures within a bootstrapped lens are forced structures of the *generator*, articulated through that lens.

### 6. Each topic file should follow the standard template

Every topic file in any experiment's construction chain should use the template at [`../10-experiments/topic-template.md`](../10-experiments/topic-template.md). Following the template keeps the discipline visible: dependencies, commitments, four-property check, comparison, transferability, what-this-enables.
