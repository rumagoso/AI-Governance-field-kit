# AI Governance Field Kit

Practitioner-grade tools for governing AI systems in the real world.

*Last reviewed: November 2026.*

## What this is

Regulators write rules. Vendors ship products. Auditors check boxes. Between them sits the gap where AI governance actually has to work, and that gap is largely empty of usable artefacts. This kit exists to close some of that gap.

A field kit is what you carry into the work, not what you read about the work. The artefacts here are designed to be auditable, citable, and usable inside ISMS, audit, and compliance practice. They are built from inside that practice, not from outside it. Every piece has been published or deployed; none are theoretical.

This repository is a consolidation point. Most artefacts live in their own repositories and are linked from here; the book, *Seamless*, lives inside this one.

## The book: *Seamless: AI Governance for the Parts Nobody Owns*

Eighteen essays on where AI governance actually fails: not in any single control, but in the space between two things. Each essay is paired with a practical companion chapter (a record, a worksheet, an inventory) in a field manual you can use on its own. Self-published, written in public, launching February 2027.

- **Start here:** [`seamless-repo/`](seamless-repo/), with its own README, the essays, the field manual, a priority guide and a "first 30 days" plan.
- **Find the right chapter fast:** the [Rosetta Stone](seamless-repo/docs/rosetta-stone.md) indexes the whole book by symptom, by regulation and by family.
- **Licensing is different here:** the essays are all rights reserved; the field-manual templates are CC BY-SA 4.0. See [Licence](#licence).

## The stack: four layers

The artefacts in this kit are not a loose collection. They sit in four interlocking layers, each addressing a different governance question:

**Layer 1 — Declaration.** What should an AI system disclose about itself? Artefacts: WBSC.

**Layer 2 — Detection.** How do we verify those declarations against actual behaviour? Artefacts: WBSC-PL.

**Layer 3 — Application.** How does an organisation use the framework in real assessment and assignment of responsibility? Artefacts: AI Supplier Assessment Template, RACI Matrix for Agentic AI Governance, Agent Mandate Template, and the *Seamless* field manual.

**Layer 4 — Accountability.** When something goes wrong, how is the action attributable, the chain of custody intact, the entity identifiable? Artefacts: TRACE.

The four layers are independent enough to use separately, and integrated enough that they reinforce each other when used together.

## Artefacts

**WBSC v1.1.0 — Worldview & Belief System Card.** An open standard for AI transparency. Surfaces the worldview, belief system, and ethical posture embedded in an AI system, in a form that practitioners can read and auditors can cite. Published on the CSA blog, October 2025. Licence: CC BY 4.0. → [github.com/rumagoso/worldview-belief-system-card](https://github.com/rumagoso/worldview-belief-system-card)

**WBSC-PL v1.1.0 — WBSC Probe Library.** A structured library of prompts for behaviourally sensing AI systems. Probes are versioned, classified by type (direct, indirect, stress, meta), and mapped to specific WBSC fields. Used to test whether a system's stated posture matches its observed behaviour under controlled conditions. Licence: CC0. → [github.com/rumagoso/wbsc-probe-library](https://github.com/rumagoso/wbsc-probe-library)

**AI Supplier Assessment Template v0.1.** A ten-question template for evaluating AI vendors. Designed to slot into existing supplier-security workflows without rebuilding them. Covers training-data provenance, data-handling commitments, audit rights, subprocessor disclosure, and incident notification. Licence: CC BY 4.0. → Public Gist (linked from this repository when integrated)

**RACI Matrix for Agentic AI Governance v0.1.** A responsibility-assignment matrix for agentic AI deployments inside an organisation. Portuguese-language original; English translation in progress. Maps roles across deployment, monitoring, incident response, and decommissioning. Licence: CC BY 4.0.

**Agent Mandate Template v0.1 (November 2026).** Thirteen fields, in three groups (authority, control, lifecycle), that record what an AI agent is allowed to do, who granted it, and when it must be revalidated. Worked example first, blank template after. Covers the governance that emerging agent-token standards leave open. Licence: CC BY-SA 4.0. → [`Agent Mandate Template.pdf`](Agent%20Mandate%20Template.pdf)

**TRACE v0.2 — Trusted Registry for Autonomous Connected Entities.** A position paper proposing a runtime identity and accountability layer for AI agents acting across organisational boundaries. Submitted as public comment to the NIST NCCoE concept paper on software and AI agent identity (April 2026). Solo work; collaborators welcome. Licence: CC BY 4.0.

**90-Day Runbook (spine).** In drafting, not yet in this repository. A practitioner-facing guide for organisations standing up AI governance from a near-zero baseline in ninety days, in three blocks: Diagnose (weeks 1–4), Verify (weeks 5–8), Govern (weeks 9–12). First vertical: NIS2 (Portuguese context). Second vertical: DORA.

**Seamless: AI Governance for the Parts Nobody Owns.** The book described above. Essays all rights reserved; field-manual templates CC BY-SA 4.0. → [`seamless-repo/`](seamless-repo/)

## Landed articles

The published trail behind the kit, in chronological order:

| Date | Venue | Title |
|---|---|---|
| Oct 2025 | CSA blog | [Beyond AI Principles: Building Practical Transparency for Cybersecurity](https://cloudsecurityalliance.org/blog/2025/10/14/beyond-ai-principles-building-practical-transparency-for-cybersecurity) |
| Mar 2026 | Substack — Meanderthal #1 | Civis |
| Mar 2026 | Substack — Meanderthal #2 | Eerie |
| Mar 2026 | LinkedIn | TRACE: the manifest we forgot to write |
| Mar 2026 | Substack — Meanderthal #3 | The Manifest We Forgot to Write |
| Apr 2026 | NIST NCCoE | Public comment on AI agent identity (TRACE submission) |
| Apr 2026 | CSA blog | [From Declaration to Detection: Sensing AI Behavior with the WBSC Probe Library](https://cloudsecurityalliance.org/blog/2026/04/27/from-declaration-to-detection-sensing-ai-behavior-with-the-wbsc-probe-library) |
| May 2026 | LinkedIn | The Auditable Surface Just Multiplied. Our Frameworks Have Not. |
| Oct 2026 | LinkedIn | *Perishable Security* (three-part series) → [repo](https://github.com/rumagoso/perishable-security) |
| Oct–Nov 2026 | LinkedIn | *Seamless* essays, published ahead of the book: *Screened Out, Together*; *Qualified to Disagree*; *The Last Human Signature*; *84 Days*; *Every Hand That Touched It*; *Nobody Owns the Seam*; *The Ghost in the Estate* |
| Nov 2026 | CSA blog | Lost in Delegation |
| Nov 2026 | LinkedIn | Contain Yourself (short version; the full version is forthcoming on the CSA blog) |

<!-- CONFIRM: exact dates for the Seamless essays after Qualified to Disagree (16 Oct 2026). -->

More writing at [rumagoso.substack.com](https://rumagoso.substack.com).

## What's in flight

- **The book.** Eighteen essays and seventeen field-manual chapters are drafted; launch is planned for February 2027. The repository stays live after publication, so regulations that change get corrected here.
- **Empirical research.** WBSC-PL v1.2 is planned as a cross-vendor study of CVP-gating effects on belief-stress probes, to be pre-registered on the Open Science Framework. <!-- CONFIRM: still planned, and OSF status. -->
- **Practitioner adoption.** The 90-day runbook is the primary adoption surface; NIS2 first, DORA second.
- **Talks and venues.** Accepted talks are listed here when confirmed.

These are commitments to track, not promises to deliver on a fixed date.

## Principles

The discipline that holds the kit together:

- Build in the open. New material is openly licensed by default (CC BY 4.0 or CC BY-SA 4.0); specific artefacts may use CC0 or MIT, and the book's essays are the stated exception.
- Versioned, datable, hash-verifiable run records.
- The rater is never the system under test.
- Findings are published regardless of outcome. Null results count.
- Practitioners are the primary audience. Academics and policymakers are welcome; they are not the design centre.

## How to use this kit

**As an ISMS practitioner evaluating an AI vendor.** Start with the AI Supplier Assessment Template. Where the vendor's answers leave gaps, run the relevant WBSC-PL probes against the system. Use the WBSC structure to record what was claimed, what was observed, and where the two diverged. Bring that record into your supplier risk file.

**As an auditor producing evidence for ISO 42001 Clause 8.** WBSC gives you a declaration artefact. WBSC-PL gives you a verification method. The combination produces an audit trail that is reproducible, dated, and citable. The Assessment Template plus RACI close the loop on organisational responsibility.

**As someone deploying AI agents.** Write one Agent Mandate per agent instance, then use the *Seamless* field manual for the surrounding records: seam inventory, authority ladder, switch map. The [priority guide](seamless-repo/docs/priority-guide.md) says which to do first.

**As a researcher reproducing or extending findings.** WBSC-PL is CC0 and versioned. Run records are published with each release. Cross-vendor methodology is documented in the design doc accompanying each release. Forking, extending, or contesting is welcome.

## Contributing

Feedback, issues, and pull requests are welcome. For now:

- Issues on the relevant artefact repository (each piece has its own home; see Artefacts above). For the book, open an issue here.
- Direct contact: see Author below.

A consolidated contribution guide will follow once the kit's structural decisions land.

## Author

Rui Soares. Head of Cybersecurity and ISMS Manager (CISSP), Invited Lecturer at NOVA IMS, member of the Portuguese ISO technical committees. Author of WBSC, WBSC-PL, TRACE and *Seamless*.

Newsletter: Meanderthal. Contact: rui.msoares@gmail.com.

## Licence

This repository uses different licences for different material:

- **Repository code and default:** MIT (see `LICENSE`).
- **Artefacts:** each carries its own licence (CC0, CC BY 4.0, CC BY-SA 4.0, or MIT), as noted in Artefacts above.
- **The book, *Seamless*:** Part One (the essays) is © Rui Soares, all rights reserved. Part Two (templates and worksheets) is CC BY-SA 4.0. Details in [`seamless-repo/README.md`](seamless-repo/README.md).
