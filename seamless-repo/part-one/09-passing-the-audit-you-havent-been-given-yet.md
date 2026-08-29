# Passing the Audit You Haven't Been Given Yet

*Five out of twenty-three. That's the base rate among organisations built to be audited.*

When the US Government Accountability Office reviewed the AI inventories of twenty-three federal agencies — agencies with statutory reporting obligations, dedicated compliance staff, and years of advance notice that the requirement was coming — only five could provide comprehensive information for every use case they had reported. Three agencies had no AI use cases to report at all. Of the remaining twenty, the other fifteen had gaps: missing fields, inaccurate entries, systems that had gone stale between one reporting cycle and the next. Two inventories had listed something as an AI system that, on closer inspection, wasn't AI at all. GAO ended up issuing thirty-five recommendations to nineteen agencies just to get the inventories themselves into a defensible state. (GAO-24-105980, *Artificial Intelligence: Agencies Have Begun Implementation but Need to Complete Key Requirements*, 12 December 2023.)

Sit with that for a moment before moving on to the private sector, which faces the same question with none of the statutory obligation and considerably less practice. If the organisations built specifically to be audited can't reliably produce a clean account of their own AI use, the honest question for everyone else isn't whether they have an AI governance policy. It's whether they could survive being asked to prove it.

## Policy is not evidence

Most AI governance programmes are, at bottom, well-written descriptions of what should happen. A policy states that models are validated before deployment, that a named function signs off on high-risk use cases, that oversight is documented. All of that is worth having, and none of it answers the question an auditor, a regulator, an acquiring company's due-diligence team, or a plaintiff's lawyer will actually ask: for this specific decision, on this specific date, can you show me it happened as described?

The two are not the same artefact, and organisations reliably invest in the one that's easier to finish. A policy is a document; once written and approved, it is done, in the sense that matters to a project plan. Evidence is not a document. It is a habit — logged continuously, at the moment each decision is made, by a system built for exactly that purpose. Nobody gets to declare evidence "finished," because it accrues only as fast as the organisation keeps producing it, and stops the moment anyone looks away.

## What the chain actually looks like

Take one ordinary example: an AI system flags a loan application for manual review. Proving governance around that single event means being able to produce, for that one case, a specific chain — which model version made the flag, on what data, under what documented risk tier, routed to which named individual, who took what action and on what basis, with a timestamp on every link.

Most organisations, asked to produce this chain for a case from eight months ago, will have most of the links and be missing exactly the one that matters. The model version is usually recoverable from deployment records. The routing is usually recoverable from a ticketing system. The one link that tends not to survive is the last one — a specific person's documented reasoning for the decision they made, distinguishable from a rubber stamp applied because the queue was long. Everything upstream of the human is comparatively easy to log automatically. The human link is the one organisations assume will always be reconstructable from memory, and it's the one that isn't.

## Why the evidence rots faster than the policy

A policy stays true until someone deliberately rewrites it. Evidence decays on its own, continuously, without anyone having to do anything wrong.

Log retention defaults quietly delete the record after ninety days, because that was the storage setting someone chose for cost reasons long before anyone connected it to audit exposure. Model versions roll forward — a vendor ships an update, the behaviour behind a decision made in March is no longer the behaviour running in June, and nothing in most organisations' processes re-validates the earlier decision against the version that actually produced it. The named accountable individual for a decision made eight months ago may have changed teams, changed roles, or left the company, and the org chart that would have explained who they were reporting to no longer exists in the form it did on the day of the decision.

None of this is negligence in the way a missing control is negligence. It's closer to erosion — evidence audit-readiness isn't a project with a finish line, it's a rate an organisation either keeps up with or quietly falls behind on, one expired retention window at a time.

## The narrower, buildable ask

A comprehensive evidence programme covering every AI use case an organisation has, built and maintained indefinitely, is the kind of ask that sounds responsible and gets funded once, badly, and then abandoned. It restates the scale of the problem as though naming it were the solution.

The narrower version is more honest about what's actually achievable, and considerably more likely to survive contact with a real budget: identify the handful of decision types that would actually get asked about — the ones a regulator, an insurer, or a plaintiff's lawyer would plausibly want to trace — and for those specifically, make the full chain real, including the human link that usually goes missing. Depth on the few cases that matter beats shallow, decorative coverage across everything an organisation happens to be doing with a model. Five well-evidenced decision types survive an audit. A hundred loosely logged ones do not.

## Show me

The uncomfortable moment in any version of this story isn't the audit request itself. It's the moment, somewhere in the room, when someone realises the honest answer to "can you show me" was never going to be yes — not because anyone lied about their governance, but because nobody had built evidence at the same pace they'd built policy.

Twenty-three agencies had years of notice, statutory obligation, and dedicated staff. Eighteen still couldn't produce a clean account of their own AI use when asked. The question worth answering before that room exists is not whether your policy is well written. It's whether, for the handful of decisions that would actually get questioned, you could show your working tomorrow morning.

---

## Annex: AI Inventory Template — Mandatory Fields by Regime

A single inventory record, built once, can satisfy most of what the major regimes ask for separately — if it captures the fields below. Columns mark where each field is a genuine legal requirement (●), a de facto necessity for downstream obligations (○), or not applicable.

| Field | AI Act (Annex VIII / Art. 71) | GDPR (Art. 30 record) | NIST AI RMF (MAP function) | ISO/IEC 42001 (AI inventory) | US Federal (EO 13960 / OMB) |
|---|---|---|---|---|---|
| Unique system name / identifier | ● | ○ | ● | ● | ● |
| Purpose / intended use | ● | ● | ● | ● | ● |
| Provider identity & contact | ● | ● | ○ | ○ | — |
| Deployer identity & contact | ● (public deployers) | ● (controller) | ○ | ○ | ● |
| Risk classification / tier | ● (high-risk basis) | — | ● | ● | ○ |
| AI life-cycle stage (design / pilot / production / retired) | ○ | — | ● | ● | ● |
| Categories of data processed | ○ | ● | ● | ○ | ○ |
| Deployment status (on market, recalled, suspended) | ● | — | ○ | ○ | ○ |
| Conformity assessment / certification reference | ● | — | ○ | ● | — |
| Named accountable human / role | ○ | ● (controller) | ● | ● | ○ |
| Impact assessment reference (DPIA / FRIA) | ● (deployer) | ● | ○ | ○ | ○ |
| Public / releasable status | ○ | — | — | — | ● |
| Retraining / version-change log | ○ | ○ | ● | ● | ○ |

**Reading the table:** the AI Act and the US federal inventory regime are the two most prescriptive on *identity and status* fields — who, what, is it still running. GDPR is the strictest on *data category and accountable controller*, inherited whenever an AI system touches personal data regardless of AI-specific law. NIST's RMF and ISO 42001 are the two that actually ask for *lifecycle and change* fields — the ones every inventory tends to go stale on first.

A record missing the life-cycle-stage and version-change fields will satisfy the AI Act's registration on day one and fail the moment anyone asks whether the entry still describes what's actually running.

The gap between those two moments is not a technical oversight. It is the part of the record nobody was ever assigned to keep true.
