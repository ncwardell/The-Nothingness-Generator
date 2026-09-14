# Logical Audit

*Internal consistency review of the generator. Findings are ordered by severity.*

---

This document complements [`audit.md`](audit.md), which sorts the generator's content into factual / methodological / interpretive. This one asks a narrower question: **are there places where the framework's own documents contradict each other, or where a claimed forcing does not hold?**

Scope is the generator level only — postulates, grammar, process. Findings are stated against the framework's own standards (forced-vs-chosen, atomicity, Internality), not against external ones.

---

## Finding 1 — `02-polarity.md` contradicts itself on minimality ⚠ **substantive**

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

**Why it matters.** This is the framework's first substantive move. If paired polarity is forced, the arithmetic chain overstates its commitments and should be corrected. If it is chosen — as A, atoms.md, boundary.md and the chain all say — then Claim B is wrong and the final section of `02-polarity.md` should be withdrawn.

**Recommended:** delete or rewrite the final section of `02-polarity.md`. The rest of that file is among the most careful writing in the repository; the closing section undoes it.

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

**Recommended:** state the demarcation explicitly. A workable line: *productive tension holds between postulates, and between a structure and its own conditions; a contradiction between two assertions within a single derivation is a defect.* That keeps the founding tension intact while making the framework correctable — and being correctable is what makes the paraconsistency principled rather than protective.

---

## What the audit did not find

- **No broken derivation** in the grammar. The weak-polarity derivation is valid arithmetic; the self-reference derivation is valid given the stated reading of Existence; Closure follows from Internality trivially, as claimed.
- **No stealth import** in the arithmetic, algebra, or topology chains. Every construction examined uses only prior topics plus the postulates; external mathematics appears only in `## Comparison` sections, always in the form "in standard mathematics X; here it is generated as Y." The discipline is real and consistently applied.
- **No overclaiming in the experiment overviews.** The physics modules label their depth and particle assignments as **chosen hypotheses**, which is the correct status for them.

The generator's epistemic discipline is the strongest thing in the repository. Findings 1, 3 and 5 are all cases where the repo departs from its *own* standard, not from an external one.

---

## Summary

| # | Finding | Severity | Fix |
|---|---|---|---|
| 1 | `02-polarity.md` self-contradiction on minimality | substantive | delete/rewrite its final section |
| 2 | Self-bootstrap presupposes step 3 | substantive | name it; reframe as fixed point |
| 3 | `existence.md` vs `03-self-reference.md` on the two readings | substantive | name the strong reading as a commitment |
| 4 | "Four standing properties" overcounts | presentational | restate as one + three |
| 5 | Paraconsistency lacks a demarcation criterion | methodological | state where tension ends and error begins |
