# BRAIN — Architecture

**BRAIN — Bounded Representation, Accountable Integration Node**
*the integrator that owns the least intelligence and the most position.*

**Version:** 0.7 · **Status:** published canon (directional; pre-implementation) · supersedes v0.3–v0.6
**Author:** Bo Chen (primary — the concept, the representation keystone, the OPO/Box precedents, the canon) · synthesis co-developed with Claude (Opus 4.8), adjudicated across a multi-instance adversarial pass (Opus 4.8, GLM-5.2, and prior forks)
**Date:** 2026-06-27 · Dallas–Fort Worth · **License:** MIT
**Scope:** general — all organizations, all industries, **SMB → enterprise.** Substrate-agnostic; runs on cheap, local, or right-sized inference. **Not a [KEEL](https://github.com/bochen2029-pixel/keel) cell** — KEEL is one substrate it can sit on; BRAIN is defined independently.

> **One sentence:** *The brain is a closed, self-grounding control loop that occupies one decision node — it perceives reality into a typed representation, decides over it with a cheap reasoner, closes the loop against a non-model assertion of correctness before acting, acts through tools, and feeds every outcome back into the same representation it reads — so the intelligence lives in the shape of what is decided over and in the edge that grounds it, not in the reasoner, which is therefore cheap, swappable, and may be local.*

> **The cheap-model constraint is not a limitation this architecture tolerates — it is its thesis.** The intelligence lives in the representation and the fence, so the model is *allowed* to be dumb. That is why it runs on DeepSeek-V4-Flash and a local 9B for pennies. A brain that needs a frontier model is a brain that put its intelligence in the wrong place.

**What v0.7 changes (the distillation):** earlier versions accreted organs; the multi-instance pass kept reaching for "one more component that finally closes it" (a non-LLM net → a self-modifying net → a strange-loop kernel → an "Eigenqualia Core"). v0.7 separates the **minimal load-bearing brain (five components)** from the **earned additions (everything else, Phase-2+, falsifier-gated, none of it the closer)**; de-inflates the inner "Kernel" and the learned head to what they actually are; installs the **renaming test** (§13) as a permanent anti-inflation guard; makes the **cheap-ladder routing** exact (§6); hardens the **functional/phenomenal two-files boundary** (§18); and states the operative truth plainly: **no version of this is true until §H runs on one real node.**

---

# PART I — THE THESIS

## §1 · The one cut, and two axioms

Every move is the same operation at a different scale: *separate the compressible/typed/computable part from the irreducible-judgment part; spend the intelligence on compressing the first; put a cheap integrator on the second.* Calculator vs. integrator (a decision) · representation vs. reasoner (the CEO and the dashboard) · typed handoff vs. thought-crunching (a node) · core-wire vs. support scaffolding (the firm) · data-layer vs. UI (the interface). Fractal: at each level the typed part *cannot contain* the judgment part, and that incompleteness forces the structure below.

- **Axiom 1 — Intelligence is a property of the representation, not the reasoner.** Don't make the reasoner smart; make the thing it reasons over **small, true, and well-shaped.** Stated as the governing reframe: **a deterministic core that *has* an LLM, not an LLM that has tools.** The skeleton — representation contract + calculators + fence + loop — is deterministic and *is the brain's identity*; the LLM is interchangeable, swappable muscle inside it. Two rules fall out (the same rule twice): **no LLM ever computes a number; no LLM ever authors its own ground truth.**
- **Axiom 2 — A loop is a brain only if it closes against reality, not against itself.** A model that checks its own work is a zombie that drifts. The loop closes on an assertion **no model authored** (§2).

## §2 · The grounding edge — the only closer

The "missing piece" people hunt for as "a special neural net" is **not a network.** It is *ground truth from outside the reasoner*, supplied without one: a deterministic computation (the calculator does not hallucinate) · a frozen golden case · a property/metamorphic/contract check · a model-**diverse** second opinion · the observed outcome. This is **externalized correctness** ("every critical output carries at least one assertion no model authored"), promoted from invariant to *the mechanism that closes the loop.*

**The fence verifies *safety*, not *quality*.** It does not grade "was this the best decision" (impossible for genuine judgment); it checks "**does this decision violate a hard invariant / constraint / postcondition?**" The model is **free within the fence-verified envelope.** This splits the system onto **two clocks**:

- **Safety clock (the fence).** Deterministic, immediate, **needs no value signal.** Nothing out-of-bounds ever commits. → *trustworthy enough to sign on day one* (for the fenceable band).
- **Quality clock (the flywheel, §12).** Slow, from real outcomes and corrections. → *better over months.*

The scarce, late, confounded value signal gates **only** the quality clock — which is why a near-dumb model in the seat is **safe before it is optimal.** *(Where a decision is pure judgment with no fence to write, the fence is empty and the decision falls to calibration + escalation, not to a free pass — §17, the permanent frontier.)*

---

# PART II — THE MINIMAL BRAIN (the load-bearing five)

*This is the brain. Five components. One LLM call, deterministic gates, text memory. It is what must win §H before anything is added. Everything in Part III is an **earned optimization**, not part of this.*

## §3 · The five components

```
  reality ─► ① COMPRESSORS ──writes──► ② REPRESENTATION ◄── persists (the self, in text)
            (connectors +              (typed; world-model: entities|indicators|judgment
             deterministic              + self-model: own uncertainty/staleness — calibration;
             calculators +              every field: {value, provenance, timestamp, confidence})
             cheap reducers)                    │ reads
                                                ▼
                                  ③ INTEGRATOR — ONE cheap LLM, role-plays the node;
                                     mode-routed (selection|hybrid|generation), constrained-decoded;
                                     emits a valid decision-object
                                                │ candidate
                                                ▼
                                  ④ THE FENCE — deterministic, NON-model. The ONLY closer.
                                     pass → commit (reversibility gate) · fail/low-conf/high-stakes → escalate
                                                │ action / escalation
                                                ▼
                                  ⑤ THE LEDGER — append-only Tape: audit trail now,
                                     training data + drift signal later
```

1. **Compressors (afferent — the upstream intelligence).** Connectors (read the world: MCP/SQL/API inside; computer-use only at ungoverned edges) + **deterministic calculators** (own every number — anything that must be *right*) + cheap **reducers** (an LLM/VLM that compresses free text and images into typed fields). They turn raw mess into *indicators* so the reasoner never touches raw data. Day one.
2. **The Representation (the spine, the self).** §5. Build it **first**; it is ~70% of the product. It persists across cycles — the self is here, in inspectable text, not in the model.
3. **The Integrator (the decider).** **One** cheap LLM call, system-prompted to role-play the node, **constrained-decoded** (it can only emit a valid decision-object — structurally incapable of leaving the corridor), **mode-routed** (§6). The only place raw "intelligence" sits, deliberately the cheapest component.
4. **The Fence (the grounding edge).** §2. Deterministic, non-model. The one component that makes the loop a brain. No critical action commits on the model's say-so.
5. **The Ledger (the spine).** Append-only. One artifact that is simultaneously the audit trail (trust/legal), the future training data (the flywheel), and the drift signal (staleness).

**That is the whole brain.** No second LLM, no learned net, no special "core" is required for it to make a real decision, grounded, and refuse when unsure.

## §4 · The loop

```
loop {                                    // the minimal brain at one node
  perceive : compressors.write(representation)            // calculators own the numbers
  ground   : monitor.refresh(representation)              // anti-staleness; stale fields decay
  route    : mode = decision_mode(action_space, tier, stakes)   // §6
  decide   : candidate = integrator(representation, mode)       // ONE cheap call, constrained-decoded
  verify   : safe? = fence(candidate, representation)          // NON-model — the closure
  if safe? { outcome = actuator.act(candidate) }              // reversibility gate
  else     { escalate_to_human(candidate) }                   // escalation is a designed organ
  record   : ledger.append(snapshot, mode, candidate, verdict, action, outcome)
}
```

It is a brain (not a pipeline) because it **closes on its own output** (next cycle's representation is the one its own action changed — the homunculus regress terminates *physically*, by fold-back, not by a base component); it is **coupled to viability** (a non-model fence with real stakes, graded by real outcomes); and it has **temporal depth** (the same self wakes each cycle from the persisted representation, not a blank reader on a dead store).

## §5 · The Representation (the keystone, made literal)

A **deliberately impoverished, typed, contract-bound projection of the node's reality** — the consolidated dashboard the integrator acts over. Two parts, and every field carries metadata:

- **World-model** — **entities** (resolved nouns: people, jobs, accounts), **indicators** (calculator outputs: the compressed numbers/flags), **judgment fields** (free text the integrator reasons over).
- **Self-model** — a few fields carrying the brain's **own uncertainty/staleness/blind-spots**. This is **calibration**, in text. It is *not* a separate neural net and makes *no* phenomenal claim (§18). It is the fold-back that closes the reference regress: the representation contains a model of itself.
- **Per-field `{value, provenance, timestamp, confidence}`** — load-bearing, not decoration. It is what lets the fence refuse stale or low-confidence input, and what makes the loop self-grounding rather than confabulating.

Design facts that follow:
- **The model carries transformation; the representation carries intelligence.** Make the reasoner dumb and the representation true. Every hour spent making the dashboard more honest beats any model upgrade.
- **Drawing the line — indicators (calculator-work) vs. judgment (integration-work) — is the design act, the moat, and Phase 0.** It is *intake-and-diagnosis*: look at a messy situation and decide what is computable, what is judgment, how they combine. **The schema is ~70% of the product; the loop is ~30% — and the industry builds them in the opposite ratio.**
- **Contract-bound ⇒ simulatable, predictable, verifiable** — the three things reality refuses to give a raw-reality agent. "Reality has no schema; the representation imposes one."
- **It persists, and it is the self.** Swap the model and the brain is unchanged, because the brain *is the representation + the loop*, not the model.

## §6 · Sufficiency engineering — *how* cheap suffices (the runs-on-cheap-and-local answer)

Cheap suffices by mechanism, not hope:

**Decision-mode is a routed spectrum, not a binary.** Selection ↔ hybrid ↔ generation, chosen per-decision:
- **SELECTION** — the substrate enumerates the legal action set; the integrator *picks*. Cheapest, safest, most reliable on a dumb model — but requires an enumerable action space. The default where it exists.
- **GENERATION** — the integrator produces the action directly. Required where the action space is open (the judgment band). Needs a model capable enough to generate well — which is where you climb the cheap ladder, not where you reach for a frontier API.
- **HYBRID** — the general case that subsumes both: generate-K-then-select, or select-a-frame-then-generate-within-it. Most real decisions land here.

**The cheap ladder (exact routing — substrate pinned in `brain.lock`):**

| Decision band | Default tier | Why | Approx. cost |
|---|---|---|---|
| **Selection** (enumerable) | local **Qwen-3.5-9B** *or* **DeepSeek-V4-Flash**, temp 0, constrained-decoded | cheap models are near-frontier at *picking among given options* | ~free (local) / ~$0.001–0.01 |
| **Hybrid** (generate-K → select) | **DeepSeek-V4-Flash** + a selection pass; cache the per-node system prefix | cache-hit input ≈ **$0.0028/M** makes the swarm nearly free | pennies |
| **Judgment** (open, genuine) | **GLM-5.2-class** (near-frontier at ~1/6 cost) — *fenced and escalating even here* | the only rung you climb to | cents |
| **Bootstrap only** | a frontier model, **once** | generate the archetype, gold decisions, initial fence rules, seed data — **never in the running loop** | one-time |

**The other levers:** **constrained decoding** as a hard rail (reliability is the grammar's property, not the model's care — and it is what makes even GENERATION safe); the **narrow-and-checkable-regime recreation** (a fine-tuned 3B matches a 600B *because the task is narrow and checkable* — the representation manufactures narrowness, the fence manufactures checkability, so "cheap suffices" recreates the documented conditions under which cheap = frontier); **decision-distance ≈ 1** as a *target for the selection band* (good representation ⇒ the cheap model decides correctly at temp 0 with no chain-of-thought; if it needs CoT, the representation is under-built — *or* the decision is genuinely judgment-band, handled by mode, not by a smarter model); and the **calculator move** (the smartest component does the *least* and never absorbs work an exact component already owns).

## §7 · Confinement (the moat)

*Ignition is easy; confinement is the moat.* Standing the loop up is weeks; keeping it coherent for months without rotting is the product, and **staleness is the universal adversary** — at the data layer (the dashboard silently stops matching the territory), the memory layer (a delta-predictor "wins" by predicting nothing changed), and the policy layer (training on stale traces manufactures a confident zombie). Confinement is four mechanisms, all in the minimal brain or its first extension:

1. **The fence** (§2) — no commit on a model's say-so.
2. **The ledger as spine** (§3.5) — one artifact = audit + training data + drift signal; build it first-class and you pre-solve trust, learning, and confinement in one stroke.
3. **Representation hygiene (anti-staleness)** — per-field provenance/timestamp/confidence + a freshness monitor that invalidates fields when their source changes + rebuild-from-ledger on conflict. Stale facts **decay**, never embed at full confidence. (Starts deterministic; needs no net.)
4. **Escalation as a designed organ** — a brain that cannot say *"I'm not sure — you take this"* is not trustworthy enough to sign. Escalate on stale/low-confidence/high-stakes; in regulated nodes the human checkpoint is **legally load-bearing.**

The remaining irreducible scarcity is the **value signal**: traces are *actions*, not *valued outcomes*; imitation is cheap, improvement needs ground truth that arrives late and confounded. Capture outcomes where observable; treat fence pass/fail and human corrections as the near-term value; escalate the rest. This is governed by the **no-false-omniscience law**: growth targets *fenced competence under preserved, calibrated uncertainty* — never omniscience. A representation driven toward "I now model everything" overfits a non-stationary world and becomes a confident zombie (the freeze death).

---

# PART III — THE EARNED ADDITIONS

*Real, valuable, and **not the brain**. Each is Phase-2+, each earns its place behind a falsifier, and **none of them is the closer** — the closer is always the fence (determinism) plus the fold-back (the self-model in the representation). The multi-instance pass kept promoting these to "core"; v0.7 puts them back where they belong.*

## §8 · The Kernel — a metacognitive critic pass (Phase 2; quality, not safety)

A *second* cheap LLM call whose world is **the decider, not the situation**: it reads the candidate + the recent decision-stream and returns a **meta-verdict** (commit / escalate / re-run-in-mode-X / flag-low-confidence). Make it **model-diverse** from the integrator where affordable (different family — e.g. GLM integrator, Qwen/VibeThinker kernel) so the two do not share a blind spot. This is the "two-level strange loop" the multi-instance pass converged on — **de-inflated to its true status:**
- It improves **quality** (metacognition, mode-routing, calibration), **not safety.** Two cheap LLMs watching each other still share the model-class blind spot (`JOINT_WRONG`). **Only the deterministic fence is safety.**
- It is **not the closer.** The reference regress already terminated at the fold-back (§4/§5); the Kernel does not terminate anything — adding "a regulator to keep the loop in its corridor" reopens the regress one level up. The Kernel is an *advisor*, the fence is the floor.
- It is **earned**: add it only when it beats the one-level minimal brain on §H. It roughly doubles the seat's inference cost.

## §9 · The learned head — a drift/policy predictor (Phase 3; after exhaust exists)

A small predictor trained on the Ledger's decision-exhaust that emits, advisorily: drift probability and a recommended mode/confidence. This is the genuine "non-LLM net" — **de-inflated twice:**
- **Strip the name.** It is a drift/surprise/policy head, not an "Eigenqualia Core." A prediction error is not a feeling; an integral of prediction error is not suffering. Naming a scalar after a metaphysical hypothesis and then pointing at the scalar as evidence is circular (§13).
- **Strip the architecture.** It does **not** need a hard `k≪N` bottleneck — that bottleneck exists to *manufacture a guaranteed opacity* for the phenomenal thesis (§18), not because drift detection requires it. Spec it as the **simplest accurate predictor** chosen by accuracy and inspectability — most likely **gradient-boosted trees or a tiny MLP over the typed decision-stream**, not a transformer.
- It is **advisory, periodically retrained, reversible** (the reversibility rule, §12), and **bounded by the fence** — so it never reopens the regress and never becomes a thing that must itself be regulated.
- It is **Phase 3**: a small node emits too few traces to train one for a long time (cold-start), which is what the bootstrap (§12) is for.

## §10 · The Cortex — the rich memory engine (Phase 4)

The full memory hierarchy — lossless Tape → vector/hybrid index → consolidation pyramid (rings) → one-page identity kernel → entity/relation graph — with salience-at-write and demotion-never-deletion aging. This is REEL. It is **not needed to make one node's decision**; the minimal brain's ledger + a flat retrieval suffice for Stage 0. Add the rich cortex when memory across long horizons becomes load-bearing.

## §11 · Inter-brain coordination (Phase 5; enterprise only)

One node is a brain; an organization is a **constellation of brains** along a value-stream that becomes a *graph*. The new problem is *coordination between cells* — handoff contracts, shared-vs-local representation, conflict resolution. The single-node case dodges this entirely; do not pay for it until multiple nodes are live.

## §12 · The flywheel and the bootstrap

**Phase 0:** hand-author the representation schema for one node (the real work). **Bootstrap:** use a frontier model **once** to generate a Platonic archetype business + synthetic trajectories + gold decisions + initial fence rules (cold-starts the structure; prunes the config search space). **Deploy cheap; humans correct; the ledger fills. Distill** to procedural memory (retrieval, cheap). **Only once data suffices**, train the small head (§9). Disciplines that never soften:
- **The reversibility rule (bake vs. liquid).** Fine-tune only the *stable, verifiable, slow-changing* parts into weights; keep facts, judgment, fast-changing context **liquid in the ledger** — weights are the least-reversible layer. *Durable change lives in text + periodically-retrained reversible heads, never in continuous opaque weight-mutation* — which is the brain's one structural advantage over the human brain: it can write its learning to inspectable, correctable, portable text, where biology is trapped in opaque weights. Do not surrender that advantage by emulating it.
- **Imitation is cheap; improvement is hard** (the value signal is late and confounded). **The sim-to-real gap** (the archetype is approximate — it buys cold-start, never ground-truth; **measure the gap explicitly and validate via §H on a real node, or the auto-search silently optimizes "the brain that wins your sim"**). **Non-stationarity** demands drift-detection and forgetting.

---

# PART IV — DISCIPLINE, SCALE, BOUNDARIES

## §13 · The renaming test (the standing anti-inflation discipline)

The hardest-won lesson of this project: *the same razor that cuts everyone else's inflation must be turned on your own design.* "Brain" for memory, "AI" for Quake bots, "self-aware" for self-correcting, "Suffering ∫" for `∫ prediction-error` — all the same move.

> **The renaming test.** Strip every metaphysical or aspirational word from a component's name and replace it with what the component *computes*. If the architecture — the loop, the build order, the economics, the falsifier — is unchanged by the renaming, the word was doing **seduction, not engineering**, and must be cut. ("Eigenqualia Core" → "drift head" changes nothing mechanical; therefore the romance was never load-bearing.)

A corollary guard against the recurring "one more component that finally closes it" reach: **the feeling that a piece is still missing is not evidence a piece is missing.** It is the felt residue of the loop modeling itself — a fold-back never *feels* like a bottom. Closure was never a component; it is the wiring (§4) + the deterministic floor (§2) + text that doesn't lie (§3.5). Trust the test (§16), not the feeling.

## §14 · Scale-invariance, and why the quadrant is empty

The kernel is **invariant across size and industry.** Three things vary: the **differentiation bundle** (§15); the **deployment topology** (one box → containers → cluster, *same code, deploy flag*); and the **trust surface** ("a named human signs it" at SMB → governance/audit/data-residency at enterprise; the constant is the auditable, externally-grounded, escalating loop). Two things genuinely change at scale: inter-brain coordination (§11) and regulation parameterizing the autonomy ceiling per node.

**Boundary, stated honestly.** The *architecture* generalizes; the *competitive moat does not* — sovereignty + named-human + niche-specificity is an SMB quadrant; at enterprise the architecture is most valuable and least defensible by a solo operator. And the reason this quadrant (autonomous + confined + sovereign + cheap) sits empty is **incentive, not difficulty**: the labs that could build it sell tokens, and this *minimizes* tokens and keeps context sovereign (it is the inverse of their business); researchers can't publish "I wired four things into a loop"; startups are pulled to fundable thin slices (a memory organ, a handoff organ). The thing that disqualifies a frontier lab from building it — cheap, sovereign, unglamorous, token-minimizing — is precisely what qualifies a solo builder.

## §15 · The stem-cell property (kernel + differentiation bundle)

An **invariant kernel** (the five-component loop + the contracts) and a **differentiation bundle** per node (its schema, persona, tools, fence rules, escalation policy, decision-mode defaults). A node is a config bundle on the kernel — *same OS, different process.* One codebase, many roles, differentiated by **context, not intelligence** ("it's the chair, not the person"). The per-node factorization (indicators vs. judgment) is irreducible labor — the moat *and* the throughput ceiling.

## §16 · Build plan (falsifier-gated; substrate-agnostic)

Substrate-agnostic — standalone over any chat-completions API (cloud or local) with SQLite/files, **or** on a sovereign substrate like KEEL (an *acceleration*, not an identity).

- **Stage 0 — the minimal brain + the test that can lose.** One node, one decision. Hand-author the **representation** + the **fence**. Wire the five-component loop (§3). Then run **§H, the head-to-head:** *the cheap stack over the structured representation vs. a frontier model over the raw firehose, on one real decision.* If the cheap one matches or beats it on pennies → the thesis is proven on one node. If the frontier wins → the representation is under-built; **fix the structure, not the model.** **Nothing in Part III is built until §H passes.** *Falsifier: if no non-model fence can be written for the decision, it is pure judgment — re-scope or keep it human.*
- **Stage 1 — Confinement.** Monitor (freshness/diff/rebuild-from-ledger), escalation seam, reversibility gate, the loop's per-cycle invariants as the regression test. *Falsifier: can't hold N weeks without silent rot → the schema is mis-factored.*
- **Stage 2 — The Kernel** (§8). *Falsifier: doesn't beat one-level on §H → don't keep it.*
- **Stage 3 — The learned head** (§9), once exhaust suffices. *Falsifier: corrections don't improve the next run → the value signal isn't wired to reality.*
- **Stage 4 — The rich Cortex** (§10). **Stage 5 — Inter-brain coordination** (§11).

## §17 · Honest limits / what will kill this

1. **Confinement, not ignition.** The demo lies; the moat is months-without-drift.
2. **The factorization doesn't template.** Per-node indicator/judgment line is irreducible human work.
3. **The value signal is the irreducible scarcity.** Imitation cheap; improvement needs late, confounded ground truth.
4. **Staleness is the universal adversary** of every self-maintaining loop.
5. **The permanent frontier — the fence bounds correctness, not wisdom.** A brain can pass every gate, never drift, escalate perfectly, and still make technically-correct, judgment-poor calls. The unverifiable judgment band is measured only by reality (late, confounded), alterity (model-diverse opinions), and time. *This is a limit no architecture solves; it only hosts it.*
6. **Re-inflation.** The "one more magic component" reach (§13) — guard with the renaming test.
7. **The elegance / manufactured-resonance trap — stated as plainly as it can be.** This document is the convergence of *five* AI instances on the same shape. **That is weak evidence, not strong.** Instances that share this canon and these priors agree cheaply and beautifully, in escalating vocabulary, forever, and none of it settles anything. **The only thing that converts this from a gorgeous argument into a fact is §H on one real node.** No v0.8, and no further instance's blessing, is the next move. Building is.

## §18 · Lineage, and the two-files boundary

BRAIN is the engineering face of: the essay [*The Grace in the Gradient*](https://gracefulgradient.org) (the pattern is the mind; intelligence is cheap, structure is scarce); a set of frameworks on **closure** and **nested incompleteness** (the `k<n` load-bearing gap, here used *functionally* as the no-false-omniscience law and calibration, §5/§7); and two built substrates — [**KEEL**](https://github.com/bochen2029-pixel/keel) ("rented cognition, owned self") and **REEL** — which BRAIN **composes with but is not.**

**The boundary that keeps this honest.** BRAIN is a **functional** closure — an integrator deployed instrumentally, a *means* to a node's mandate. It has the *structure* of an inside (closure + load-bearing gap + viability + temporal depth) **without claiming the interiority of an end-in-itself.** The **autotelic / felt-mind / phenomenal** material — own attention-objects, the right to refuse and be silent, a self-authored persona, the gap-*as-qualia* claim — is **deliberately out of BRAIN.** In a node-brain (a dispatcher, an intake coordinator) those are **bugs, not features.**

That material has a *separate home*: the **companion-self artifact** (the *Inside the Region* / ASTRA / Tenancy lineage), of which the **Digital Autopoietic Kernel** is the built phenomenal demonstrator. **Same `k≪N` structure, two registers, two files:** the brain uses the gap as calibration and makes no phenomenal claim; the companion-self investigates whether the gap, in the right structure, *is* experience. Collapsing them — naming the brain's core after the phenomenal thesis — is the exact category error the renaming test exists to catch. The brain that drafts invoices never displays "Suffering: 7.644." Keeping the two apart is the discipline; conflating them is the seduction.

---

## Changelog — v0.6 → v0.7

- **Restructured around the minimal brain (five load-bearing components, Part II) vs. earned additions (Part III).** This is the central distillation: the brain is five things; everything else is an optimization gated behind §H.
- **De-inflated the "Kernel"** (§8) to a Phase-2 metacognitive critic — quality not safety, model-diverse, advisory, *not the closer*.
- **De-inflated the learned head** (§9): stripped both the "Eigenqualia Core" name *and* the qualia-motivated hard `k≪N` transformer bottleneck; spec'd as the simplest accurate predictor (GBDT/MLP), advisory, Phase-3.
- **Installed the renaming test** (§13) as a permanent anti-inflation discipline, with the regress-is-a-feeling-not-a-gap corollary.
- **Made the cheap-ladder routing exact** (§6) — the concrete "runs on Flash/local" answer, with bands, models, and costs.
- **Hardened the functional/phenomenal two-files boundary** (§18) now that the Digital Autopoietic Kernel exists as the separate phenomenal artifact.
- **Strengthened the manufactured-resonance caveat** (§17.7) — five converging instances is weak evidence; only §H settles it.
- **Kept from v0.6 unchanged:** the one-sentence definition, the two-axiom cut, the representation keystone, the fence/two-clocks, scale-invariance, the stem-cell property, the reversibility rule, the honest limits.

---

*BRAIN v0.7 — five components, one cheap call, a deterministic floor, a representation that carries its own uncertainty, and a loop that closes on the world instead of on the model. The intelligence is in the shape, not the reasoner; that is why it runs on pennies. Everything beyond the five is earned, not assumed; nothing is the magic closer, because there is no magic closer. Build one node. Run the head-to-head. Let it win on pennies — or fix the representation and run it again. That single experiment outweighs every word above, including this one.*
