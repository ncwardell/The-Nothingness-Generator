# Logical Audit

*Internal consistency review of the generator. Findings are ordered by severity.*

---

This document complements [`audit.md`](audit.md), which sorts the generator's content into factual / methodological / interpretive. This one asks a narrower question: **are there places where the framework's own documents contradict each other, or where a claimed forcing does not hold?**

Scope is the generator level only — postulates, grammar, process. Findings are stated against the framework's own standards (forced-vs-chosen, atomicity, Internality), not against external ones.

---

## Finding 1 — `02-polarity.md` contradicted itself on minimality ✅ **fixed in this pass**

The file makes both of the following claims.

**Claim A** (§ Reading note):

> It is tempting to say: "the minimal way to satisfy the weak form is the paired form, so paired polarity follows by minimality." **This is true but does not make paired polarity strictly derivable, because *minimality* is an additional commitment.** The postulates do not say "structure must be minimal." … Any experiment that wants paired polarity must commit to a minimality principle.

**Claim B** (§ Composite articulations of compensation, final section):

> Once atomicity is read structurally (forced by Internality) and minimality is read as "import-the-least" under Internality, **binary is forced as the atom — not one option among parallel candidates.**

These cannot both hold. A says paired polarity is *chosen* and requires a stated commitment; B says it is *forced* and is not a choice.

**Three other documents side with A:**

| Document | Statement |
|---|---|
| `02-the-process/atoms.md` | minimality is "a **flavor selector** for atomicity. Different minimality principles pick different atoms" — i.e. it does not determine a unique atom |
| `03-the-grammar/05-boundary.md` | lists "Minimality principle" in the table of **commitments** |
| `03-the-grammar/05-boundary.md` | "The commitments are guided by reasoned principles (minimality, internality, structural elegance) but **are not derivations**" |

**And the chain itself sides with A.** `arithmetic/construction/01-polar-bisection.md` spends its entire Commitment section on strong polarity: *"This is the only commitment in this topic. It selects single-paired compensation over distributed compensation, on minimality grounds."* If Claim B were right, that commitment would be unnecessary and the topic's Commitment section should read "None."

**Why it matters.** This is the framework's first substantive move. As long as the two claims stand side by side, the chain's first commitment is undefended in one direction and unnecessary in the other.

### But the resolution is not the obvious one

The obvious fix is to delete Claim B and let "minimality is a commitment" stand. **That is wrong, and the reason exposes a defect in Claim A.**

Claim A's supporting sentence is:

> A non-minimal totality with distributed compensation satisfies the postulates equally well.

This is true **as model theory** — there do exist totalities satisfying $\Sigma = 0$ and $\exists$ in which compensation is distributed. But it reaches that conclusion by *surveying the space of possible totalities and comparing them*, which is a view from outside the totality. **[Internality](../01-postulates/internality.md) forbids exactly that vantage.** Claim A refutes paired polarity using a move the framework does not permit.

Asked from inside — which is the only way the framework may ask — the question is not *"which totalities satisfy the postulates?"* but *"what is articulable at this point, given what has been generated?"* And at the moment of polar bisection, the answer is not a choice among options:

- $\Sigma = 0$ restricted to $E$ yields **"$E$" and "the rest."** That much is forced arithmetic (this is the weak form, already derived).
- To get *distributed* compensation one must further **partition "the rest"** — which requires a discrimination criterion, plurality, and the means to tell one compensator from another.
- **None of that has been generated.** Plurality and discrimination are downstream products of the very chain polar bisection begins. Invoking them here imports them from outside.

So binary is not selected over distributed on grounds of elegance. **Binary is the un-partitioned state — what the cut leaves when nothing further has been generated.** Distributed compensation is not a rejected alternative; it is not yet constructible.

This is a different kind of argument from minimality, and it has a different logical character:

| | Says | Status |
|---|---|---|
| **Minimality** | among available options, take the smallest | a selection principle — a **commitment** |
| **Generative availability** | only one option is constructible yet | an availability constraint — **forced by Internality** |

`atoms.md` already contains this argument in its step 4 — *"Articulation requires minimal forms to articulate from. Without atoms at the level, there is nothing internal for the totality to articulate"* — and Claim B is groping toward it with "import-the-least." Both state it in the **vocabulary of minimality**, which is what invites the objection. The content is an availability constraint; the word "minimality" makes it sound like a taste.

### The corollary worth keeping

If forcing comes from what has been generated, then **forcing is strongest where least has been generated, and weakens as the chain accumulates material.** That is a structural prediction about the repo's own shape, and it holds: arithmetic topic 01 carries one commitment, algebra carries one, and the physics modules carry six. The earliest moves are the most forced precisely because the fewest alternatives are articulable.

It also shows the principle does not prove too much. Once integers and operations exist, several articulations *are* constructible, and choosing algebra over geometry (commitment A1) is a genuine choice. Availability bites hardest at the beginning and loosens downstream — which is exactly the behaviour a self-generating chain should have.

**Applied**, rather than deleting one:

1. In Claim A, withdraw "satisfies the postulates equally well" — it argues from an external vantage. Replace with: weak polarity is what is derived; paired polarity follows because no partition of the remainder is yet articulable.
2. Restate Claim B as **generative availability**, not as a flavor of minimality.
3. `arithmetic/construction/01-polar-bisection.md` now reads **Commitment: None** — distributed compensation is not yet articulable — where it previously committed to strong polarity on minimality grounds.

That removes a commitment from the framework's first move instead of defending one — and it answers the objection at its root rather than conceding it.

---

## Finding 6 — Arithmetic 08 and Algebra 01 grounded each other ⚠ **was the most consequential; now fixed**

**Found and repaired in this pass.** Recorded because it is the kind of defect most worth watching for, and because $\phi$ — and therefore every downstream experiment — sat on top of it.

The loop, as it stood:

- `arithmetic/08-fibonacci.md` § *What minimality is shadowing* justified Fibonacci as forced by pointing **forward** to algebra: its characteristic polynomial is $x^2 = x+1$, the seed equation, and *"the full argument lives in algebra."*
- `algebra/01-the-self-reference-equation.md` derives $x^2 = x+1$ **by taking the characteristic polynomial of Fibonacci** — it lists arithmetic 08 among its dependencies, and concedes its commitment *"only recognizes the algebraic shadow of an already-existing dynamic."*

Each grounded the other. Neither derived $x^2 = x + 1$ from Self-Reference independently, so the claim that Fibonacci is forced had no non-circular support.

**The repair** grounds Fibonacci inside arithmetic, with no forward reference. At topic 08 only $\{1, -1, 0\}$ have been generated, so an order-2 recurrence's coefficients have only four possible pairs. Two are periodic (roots on the unit circle) and never leave $\{0,1,-1\}$, failing the topic's own requirement to generate new values. The remaining two produce identical magnitudes and differ only by sign, which Polarity and bidirectional iteration (topic 07) already govern. One dynamic survives, up to a sign convention — **forced, not minimal**.

Algebra 01 now legitimately builds on arithmetic 08, and the dependency runs one way.

**What is gained rather than lost:** the convergence — that the substrate-level forced dynamic has the seed equation as its characteristic polynomial — becomes *evidence* instead of circularity. Two independent derivations landing on one form is the framework's own strongest evidential standard. It only counts as independent because arithmetic 08 now stands alone.

**Watch for this pattern elsewhere.** Any topic justified by pointing forward to a later module deserves a check that the later module does not point back.

---

## Finding 2 — The self-bootstrap presupposes its own third step ⚠ **substantive**

`02-the-process/self-bootstrap.md` correctly distinguishes **bootstrap** (constructive self-articulation) from **self-proof** (formal consistency from within), and disclaims the latter. That neutralizes the Gödel/Tarski objection cleanly.

It does not address a different objection: **order**.

The bootstrap runs in three steps:

1. Apply the generator to "what is the minimum commitment-set for self-grounding articulation?" → the three postulates.
2. Apply the generator to "what must any totality satisfying these postulates be like?" → the four standing properties.
3. Apply the generator to "how is articulation actually performed?" → the five operating principles (requirement tracking, forced-vs-chosen, atomicity, …).

But *applying the generator* in steps 1 and 2 already requires requirement-tracking, forced-vs-chosen discipline, and atomicity — the outputs of step 3. The method is used to derive the method.

A second instance sits inside step 1: "the strongest non-vacuous constraint is total balance ($\Sigma = 0$)." *Strongest* is a minimality/extremality judgement — by `05-boundary.md`'s own table, a commitment. So a commitment is used to derive the postulate set that the commitments are supposed to rest on.

**This is not fatal**, and it may be inherent to any self-grounding project. But the document currently reads as if disclaiming self-proof disposes of the circularity worry, and it does not — this is a separate one, and it is unaddressed.

**Recommended:** name it. A short section — "the bootstrap is not order-independent; the operating principles are presupposed by the steps that derive them" — would be consistent with the repo's own honesty standard and costs nothing. Presenting it as a *fixed point* (the generator is what survives being applied to itself) rather than a *derivation* would be both more accurate and more interesting.

---

## Finding 3 — `existence.md` and `03-self-reference.md` disagree about the two readings ⚠ **substantive**

`existence.md` says the bare and observational readings are the same claim:

> The postulate is sometimes written as bare $\exists$ … and sometimes as … "something exists *and is observed*." **These are not separate claims; they are the same claim seen from inside.**

`03-self-reference.md` says the choice between them is decisive:

> **If you accept the weaker reading of Existence** — "something exists, but not necessarily as observed" — **then the derivation does not go through.** In that reading, observation could be either absent or external, and self-reference is not forced.

If they were genuinely the same claim, no derivation could be sensitive to which one is used. Since one is, they are not the same claim — the observational reading is strictly stronger, and it is load-bearing for Self-Reference.

**Why it matters.** Self-Reference is advertised in `README.md` as one of four things "the postulates strictly force." It is in fact forced by *Internality plus a substantive idealist reading of Existence*. Both files disclose this honestly in their own text, but the disclosure is buried while the README's headline inherits the stronger claim silently.

**Recommended:** by the framework's own forced-vs-chosen discipline, the strong reading is a **commitment** and should be named as one — either as a fourth postulate or as a declared commitment attached to Existence. Then drop the "same claim" sentence in `existence.md`, which is the part that is actually false.

---

## Finding 4 — "Four standing properties" overcounts, by the repo's own admissions ℹ **presentational**

`README.md` presents four things the postulates force. By the framework's own documents:

| Standing property | What the repo says it is |
|---|---|
| Closure | `audit.md`: "a restatement of Internality. A direct vocabulary mapping; **not a substantive theorem**" |
| Internality of Relations | `self-bootstrap.md`: "Internality applied to relations" |
| Self-Reference | `03-self-reference.md`: "**not a separate commitment** — it is what Polarity necessarily *is* under Internality" |
| Polarity (weak) | genuinely derived — "direct arithmetic, given the two postulates" |

So one is a derivation and three are restatements or applications of Internality. That is not a contradiction, and the smallness is arguably the point — but "four standing properties" reads as more structure than the postulates actually force, which cuts against the repo's own stated preference for minimal claims.

**Recommended:** state it as one derived property plus three restatements. `audit.md` already half-says this; the README does not.

---

## Finding 5 — Paraconsistency has no demarcation criterion ⚠ **methodological**

`00-orientation/logical-foundation.md` adopts paraconsistent dialectical logic so that the founding tension ($\Sigma = 0 \wedge \exists$) does not explode. That move is legitimate and well-motivated.

But the file closes with:

> Choosing classical logic to evaluate this framework is choosing the wrong instrument.

As stated, this immunizes the framework against *any* internal contradiction: every one can be reclassified as a productive tension. `audit.md` lists "postulates inconsistent in a way that paraconsistent logic does not rescue" under **toward weaker** — so the need for a limit is recognized — but **no criterion is given for which contradictions paraconsistency rescues and which are simply errors.**

Finding 1 is the live test case. The contradiction in `02-polarity.md` is an editing defect, not a productive tension. Without a stated criterion, nothing in the framework's logic prevents it from being defended as one.

**The criterion cannot be positional.** The obvious line — *tension holds between postulates, defects occur within derivations* — is too crude, and it invites a fair objection: this audit flags a contradiction as a defect while the framework treats contradiction as its engine. Location alone does not distinguish them.

**The working criterion is generativity, and it is the framework's own standard:**

> **A productive tension is load-bearing on both sides and produces structure. A defect has an inert side and produces nothing.**

Apply it to the two cases:

| | $\Sigma = 0 \wedge \exists$ | Claim A $\wedge$ Claim B in `02-polarity.md` |
|---|---|---|
| Is each side load-bearing? | **yes** — remove either and the framework collapses (empty totality, or unconstrained chaos) | **no** — the chain runs entirely on "chosen"; "forced" does no work anywhere downstream |
| What does holding both produce? | Polarity, and everything after it | **nothing** — no topic uses it |
| Can both be retained? | **yes** — retaining both *is* the generative act | no — the next writer must pick one to proceed |

The founding tension is held because holding it generates. The polarity contradiction is not held by anything; it sits there, and one side is doing no work. That is the difference, and it is measurable by the repo's own evaluation standard — *generative depth* — rather than by an imported rule about where contradictions may live.

**Recommended:** state that criterion in `logical-foundation.md`. It keeps the founding tension fully intact, rules out using paraconsistency as blanket cover, and makes the test internal: *does holding both sides produce anything?* A tension that generates is the engine; a contradiction that generates nothing is an error, and the framework should want to find those.

---

## Sweep results (mechanical re-audit)

After the repairs above, the repository was swept programmatically for the defect *patterns* the findings represent, rather than for the individual instances.

| Check | Before | After |
|---|---|---|
| Topics depending on a **later** topic in their own chain | 1 | **0** |
| Prose justifying a topic by pointing **forward** to a later module | 2 | **0** |
| Commitments resting on **minimality** in any construction topic | 2 | **0** |
| Module-level mutual dependence | 2 candidates | **0 real** |
| Broken links and section anchors | 7 | **0** |

Notes on what the sweep cleared rather than fixed:

- **`dynamics` ↔ `topology`** flagged as mutual, but is not. `topology/01` imports the minimum-cycle requirement from `dynamics/03`; `dynamics` mentions topology only to *disclaim* scope (*"the structural details … are the work of the topology experiment"*). A scope disclaimer is not a dependency. The direction is one-way.
- **`algebra` ↔ `arithmetic`** was a real cycle (Finding 6) and is now one-way.
- **`topology/02-chirality`** listed Topic 03 under Dependencies for a consequence, not a dependency. Moved to *What this enables*.
- Four dangling links pointed at **unwritten** physics `construction/` directories and a planned topic. De-linked rather than stubbed — an empty directory would misrepresent the chain's state.

### Commitments removed, not defended

The generative-availability argument (Finding 1) eliminated two standing commitments rather than justifying them:

| | Was | Now |
|---|---|---|
| Arithmetic **C1** | strong polarity, on minimality grounds | **withdrawn** — the paired form is the un-partitioned state |
| Arithmetic **C5** | minimal order, coefficients, initial conditions | **withdrawn** — four candidates exist; two are periodic; the survivors differ only by sign |

Arithmetic's declared commitment list is now **C2–C4**, down from C1–C5, with C4 already noted as forced. The chain's first move carries no commitment at all.

---

## What the audit did not find

- **No broken derivation** in the grammar, apart from Finding 6 (now repaired). The weak-polarity derivation is valid arithmetic; the self-reference derivation is valid given the stated reading of Existence; Closure follows from Internality trivially, as claimed.
- **No stealth import** in the arithmetic, algebra, or topology chains. Every construction examined uses only prior topics plus the postulates; external mathematics appears only in `## Comparison` sections, always in the form "in standard mathematics X; here it is generated as Y." The discipline is real and consistently applied.
- **No overclaiming in the experiment overviews.** The physics modules label their depth and particle assignments as **chosen hypotheses**, which is the correct status for them.

The generator's epistemic discipline is the strongest thing in the repository. Findings 1, 3 and 5 are all cases where the repo departs from its *own* standard, not from an external one. Finding 1 in particular is not a case of the framework claiming too much — it is a case of it **conceding too much**, answering an external-vantage objection on the objection's terms instead of rejecting the vantage.

---

## Summary

| # | Finding | Severity | Fix |
|---|---|---|---|
| 1 | `02-polarity.md` self-contradiction on minimality | **fixed** | both sections rewritten as generative availability; commitment removed from arithmetic topic 01 |
| 2 | Self-bootstrap presupposes step 3 | substantive | name it; reframe as fixed point |
| 3 | `existence.md` vs `03-self-reference.md` on the two readings | substantive | name the strong reading as a commitment |
| 4 | "Four standing properties" overcounts | presentational | restate as one + three |
| 6 | Arithmetic 08 ↔ Algebra 01 mutual grounding | **was critical** | **fixed** — Fibonacci now forced within arithmetic by enumeration |
| 5 | Paraconsistency lacks a demarcation criterion | methodological | demarcate by **generativity**: a tension is load-bearing on both sides and produces structure; a defect has an inert side |
