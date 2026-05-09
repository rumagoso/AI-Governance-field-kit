# AI Governance Field Kit

**Practitioner-grade tools for governing AI systems in the real world.**

---

## What this is

Regulators write rules. Vendors ship products. Auditors check boxes. Between them sits the gap where AI governance actually has to work — and that gap is largely empty of usable artefacts. This kit exists to close some of that gap.

A *field kit* is what you carry into the work, not what you read about the work. The artefacts here are designed to be auditable, citable, and usable inside ISMS, audit, and compliance practice. They are built from inside that practice, not from outside it. Every piece has been published or deployed; none are theoretical.

This repository is in early consolidation. Existing artefacts remain in their current homes; cross-links are added as each piece is integrated. Expect movement through 2026.

---

## The stack — four layers

The artefacts in this kit are not a loose collection. They sit in four interlocking layers, each addressing a different governance question:

**Layer 1 — Declaration.** What should an AI system disclose about itself? *Artefacts: WBSC.*

**Layer 2 — Detection.** How do we verify those declarations against actual behaviour? *Artefacts: WBSC-PL.*

**Layer 3 — Application.** How does an organisation use the framework in real assessment and assignment of responsibility? *Artefacts: AI Supplier Assessment Template, RACI Matrix for Agentic AI Governance.*

**Layer 4 — Accountability.** When something goes wrong, how is the action attributable, the chain of custody intact, the entity identifiable? *Artefacts: TRACE.*

The four layers are independent enough to use separately, and integrated enough that they reinforce each other when used together.

---

## Artefacts

**WBSC v1.1.0 — Worldview & Belief System Card.**
An open standard for AI transparency. Surfaces the worldview, belief system, and ethical posture embedded in an AI system, in a form that practitioners can read and auditors can cite. Published via Cloud Security Alliance Portugal, October 2025. License: CC BY 4.0.
→ [github.com/rumagoso/worldview-belief-system-card](https://github.com/rumagoso/worldview-belief-system-card)

**WBSC-PL v1.1.0 — WBSC Probe Library.**
A structured library of prompts for behaviourally sensing AI systems. Probes are versioned, classified by type (direct, indirect, stress, meta), and mapped to specific WBSC fields. Used to test whether a system's stated posture matches its observed behaviour under controlled conditions. License: CC0.
→ [github.com/rumagoso/wbsc-probe-library](https://github.com/rumagoso/wbsc-probe-library)

**AI Supplier Assessment Template v0.1.**
A ten-question template for evaluating AI vendors. Designed to slot into existing supplier-security workflows without rebuilding them. Covers training-data provenance, data-handling commitments, audit rights, subprocessor disclosure, and incident notification. License: CC BY 4.0.
→ Public Gist (linked from this repository when integrated)

**RACI Matrix for Agentic AI Governance v0.1.**
A responsibility-assignment matrix for agentic AI deployments inside an organisation. Portuguese-language original; English translation in progress. Maps roles across deployment, monitoring, incident response, and decommissioning. License: CC BY 4.0.

**TRACE v0.2 — Trusted Registry for Autonomous Connected Entities.**
A position paper proposing a runtime identity and accountability layer for AI agents acting across organisational boundaries. Submitted as public comment to the NIST NCCoE concept paper on software and AI agent identity (April 2026). Solo work; collaborators welcome. Further development planned for 2026–2027. License: CC BY 4.0.

**90-Day Runbook (spine).** *Drafting.*
A practitioner-facing guide for organisations standing up AI governance from a near-zero baseline in ninety days. Three blocks: Diagnose (weeks 1–4), Verify (weeks 5–8), Govern (weeks 9–12). First vertical: NIS2 (Portuguese context). Second vertical: DORA. Portuguese skeleton exists; integration into this kit scheduled for autumn 2026.

---

## Landed articles

The published trail behind the kit, in chronological order:

| Date | Venue | Title |
|---|---|---|
| Oct 2025 | CSA Portugal | WBSC: a practitioner framework for AI transparency |
| Mar 2026 | Substack — Meanderthal #1 | Civis |
| Mar 2026 | Substack — Meanderthal #2 | Eerie |
| Mar 2026 | LinkedIn | TRACE: the manifest we forgot to write |
| Mar 2026 | Substack — Meanderthal #3 | The Manifest We Forgot to Write |
| Apr 2026 | NIST NCCoE | Public comment on AI agent identity (TRACE submission) |
| May 2026 | LinkedIn | The Auditable Surface Just Multiplied. Our Frameworks Have Not. |

More writing at [rumagoso.substack.com](https://rumagoso.substack.com).

---

## New directions

The kit is not finished. The following work is in flight:

**Empirical research.** WBSC-PL v1.2 is a cross-vendor study of CVP-gating effects on belief-stress probes, to be pre-registered on the Open Science Framework. A cross-vendor typology paper is planned for an academic venue in autumn 2026.

**Practitioner adoption.** The 90-day runbook (above) is the primary adoption surface; NIS2 first, DORA second. A follow-up CSA Portugal article extending the prompt-as-instrument argument is scheduled for May 2026.

**Conferences and venues.** Submissions under consideration: BSides Portugal 2026, hack.lu, Black Hat Europe, AI Village, FIRST Conference, ENISA AI Cybersecurity Conference. Status updated here as decisions land.

The directions are public so the trajectory is legible. Treat them as commitments to track, not promises to deliver on a fixed date.

---

## Principles

The discipline that holds the kit together:

- Build in the open. Default licence for new material is CC BY 4.0; specific artefacts may use CC0 or MIT.
- Versioned, datable, hash-verifiable run records.
- The rater is never the system under test.
- Findings are published regardless of outcome — null results count.
- Practitioners are the primary audience. Academics and policymakers are welcome; they are not the design centre.

---

## How to use this kit

**As an ISMS practitioner evaluating an AI vendor.** Start with the AI Supplier Assessment Template. Where the vendor's answers leave gaps, run the relevant WBSC-PL probes against the system. Use the WBSC structure to record what was claimed, what was observed, and where the two diverged. Bring that record into your supplier risk file.

**As an auditor producing evidence for ISO 42001 Clause 8.** WBSC gives you a declaration artefact. WBSC-PL gives you a verification method. The combination produces an audit trail that is reproducible, dated, and citable. The Assessment Template plus RACI close the loop on organisational responsibility.

**As a researcher reproducing or extending findings.** WBSC-PL is CC0 and versioned. Run records are published with each release. Pre-registration for v1.2 is on OSF. Cross-vendor methodology is documented in the design doc accompanying each release. Forking, extending, or contesting is welcome.

---

## Contributing

Feedback, issues, and pull requests are welcome. For now:

- Issues on the relevant artefact repository (each piece has its own home; see Artefacts above).
- Direct contact: see Author below.
- A consolidated contribution guide will follow once the kit's structural decisions land (target: late May 2026).

---

## Author

**Rui Soares.** ISMS Manager (CISSP), Invited Lecturer at NOVA IMS, member of CSA Portugal and the Portuguese ISO technical committee. Author of WBSC, WBSC-PL, and TRACE.

Newsletter: [Meanderthal](https://rumagoso.substack.com).
Contact: rui.msoares@gmail.com.

---

## License

Each artefact carries its own licence (CC0, CC BY 4.0, or MIT depending on the piece, as noted in Artefacts above). Default for new material in this repository is **CC BY 4.0** unless otherwise stated.