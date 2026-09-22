# Seamless — Part One: Academic Reading List

*A working, honest reading list per Part One article. Prioritises peer-reviewed venues (journals, ACM/AAAI proceedings) and arXiv preprints with clear scholarly framing over vendor blogs and law-firm client alerts, which are plentiful but not included here even where useful for practitioners. Suitable as a course bibliography seed as well as book back-matter. Flag entries marked (prepublication/arXiv) as not yet peer-reviewed when citing formally.*

---

## 1. "The Minimum Viable AI Eulogy" — decommissioning and end-of-life governance

- Raji, I.D., Smart, A., White, R.N., Mitchell, M., Gebru, T., Hutchinson, B., Smith-Loud, J., Theron, D., Barnes, P. (2020). *Closing the AI Accountability Gap: Defining an End-to-End Framework for Internal Algorithmic Auditing.* Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency (FAT\*'20), Barcelona, 33–44. https://doi.org/10.1145/3351095.3372873
  — Foundational lifecycle-auditing framework; explicitly warns that audit/governance can devolve into performance without structural teeth. Directly relevant to the eulogy piece's "policy without evidence" theme.
- *AI Debris: Residual Risk and the Afterlife of Failed AI Systems.* (prepublication, arXiv:2606.12432). https://arxiv.org/pdf/2606.12432
  — Proposes an "AI Debris Decommissioning Protocol," treating withdrawal as an accountability event rather than a technical shutdown. Closest direct academic companion to the essay's thesis.
- Leon, D. (2026). *Lifecycle-Based Governance to Build Reliable Ethical AI Systems.* Systems Research and Behavioral Science. https://onlinelibrary.wiley.com/doi/10.1002/sres.70014
  — Peer-reviewed; covers "AI exit plans" as an emerging regulatory expectation and end-of-life ethical review as feedback into governance standards.
- *AI System Decommissioning: A Systematic Literature Review* / *Designing a Well-Governed AI Lifecycle Model.* (2024). https://www.researchgate.net/publication/387467032
  — Systematic review of seven peer-reviewed studies on AI system suspension/withdrawal; useful for establishing how thin the existing literature actually is, which is itself part of the essay's point.

## 2. "Three Clocks, One Fire" — overlapping incident-notification regimes

- *Incident Reporting and Investigation Under the AI Act: Some Insights from Aviation.* International Journal of Law and Information Technology, Oxford Academic (2026). https://academic.oup.com/ijlit/article/doi/10.1093/ijlit/eaaf019/8501132
  — Peer-reviewed law journal article; draws the aviation-safety-reporting analogy independently, and explicitly flags regulatory fragmentation's compliance-cost and political consequences across jurisdictions. Strong anchor for this piece.
- *AI Agents Under EU Law.* (prepublication, arXiv:2604.04604). https://arxiv.org/pdf/2604.04604
  — Walks through a concrete example of one incident triggering three parallel EU notification obligations (NIS2/24h, GDPR/72h, DORA) with different formats and authorities — essentially the piece's thesis stated in legal-technical terms.
- Kennedys Law / Rexilience / Fontvera comparative overviews of AI Act Art. 73, NIS2, and GDPR Art. 33 timelines (2025–2026, practitioner rather than peer-reviewed, but the clearest primary-source-adjacent mapping of the actual clock lengths cited in the essay). Useful for verifying the matrix's numbers, not for scholarly citation.

## 3. "The Last Human Signature" — human oversight, automation bias, meaningful control

- Laux, J. et al. (2025). *Automation Bias in the AI Act: On the Legal Implications of Attempting to De-Bias Human Oversight of AI.* (arXiv:2502.10036, forthcoming in a law journal). https://arxiv.org/abs/2502.10036
  — Directly examines AI Act Art. 14/26(2)'s human-oversight and automation-bias provisions; argues the Act addresses awareness but not design as a cause of over-reliance. Core citation for this piece.
- Laux, J. (2023). *'Human Oversight' in the EU Artificial Intelligence Act.* Information & Communications Technology Law (Taylor & Francis). https://www.tandfonline.com/doi/full/10.1080/17579961.2023.2245683
  — Peer-reviewed; foundational close reading of what "human oversight" is actually meant to counterbalance in the Act's drafting history.
- *Is Human Oversight to AI Systems Still Possible?* ScienceDirect (2024). https://www.sciencedirect.com/science/article/pii/S1871678424005636
  — Peer-reviewed; catalogues the practical preconditions (expertise, time, information design) that oversight requires and rarely gets, echoing the essay's "signature never certified comprehension" argument.
- Santoni de Sio, F. & van den Hoven, J. *On the Purpose of Meaningful Human Control of AI.* PMC/NCBI (open access). https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9868906/
  — Peer-reviewed philosophy-of-technology piece; reframes "meaningful human control" debates around purpose rather than mechanism, a useful theoretical complement to the historical (seals→signatures) argument in the essay.
- *Designing Meaningful Human Oversight in AI.* AI and Ethics, Springer Nature (2026). https://link.springer.com/article/10.1007/s43681-026-01147-7
  — Peer-reviewed; proposes a layered-agency design framework distinguishing AI "operative agency" from human "evaluative agency" — theoretically underpins the Human Participation Tiers field built for Part Two.

## 4. "Nobody Owns the Seam" — agent-to-agent/agent-to-tool supply chain risk

- *TRiSM for Agentic AI: A Review of Trust, Risk, and Security Management in LLM-based Agentic Multi-Agent Systems.* (arXiv:2506.04133). https://arxiv.org/html/2506.04133v3
  — Survey covering exactly the seam category the postmark-mcp incident falls into: prompt injection, spoofing, and impersonation risk arising from cooperative, distributed agent behaviour without traditional security boundaries.
- *Agentic AI for Autonomous Defense in Software Supply Chain Security: Beyond Provenance to Vulnerability Mitigation.* (arXiv:2512.23480). https://arxiv.org/pdf/2512.23480
  — Technical framework paper on exactly the failure class (behavioural, not code-signature-based, supply-chain compromise) that made postmark-mcp uncatchable by CVE-style detection.
- OWASP Top 10 for Agentic Applications 2026 — ASI04 "Agentic Supply Chain Vulnerabilities" (industry standard, not peer-reviewed academic literature, but the closest thing to a canonical taxonomy currently naming this risk category; cited descriptively in the essay itself, so worth listing as primary source rather than secondary literature).

## 5. "Passing the Audit You Haven't Been Given Yet" — AI inventories, evidence, audit reality

- Raji, I.D. et al. (2020). *Closing the AI Accountability Gap* — see full citation under piece 1; the "paper compliance vs. structural improvement" distinction it draws is the theoretical backbone of this essay's "policy is not evidence" section.
- Raji, I.D., Xu, P., Honigsberg, C., Ho, D. (2022). *Outsider Oversight: Designing a Third-Party Audit Ecosystem for AI Governance.* Proceedings of the 2022 AAAI/ACM Conference on AI, Ethics, and Society, 557–571.
  — Peer-reviewed; addresses who audits the auditors, relevant to the essay's "evidence rots faster than policy" argument about internal self-assessment decay.
- *Making AI Compliance Evidence Machine-Readable.* (arXiv:2604.13767). https://arxiv.org/pdf/2604.13767
  — Proposes OSCAL (the NIST FedRAMP interchange format) as executable evidence infrastructure for AI Act/ISO 42001/NIST AI RMF compliance — a direct technical answer to the essay's "evidence rots faster than policy" problem, useful as a forward-looking citation.
- U.S. Government Accountability Office (GAO), *Artificial Intelligence: Agencies Have Begun Implementation but Need to Complete Key Requirements*, GAO-24-105980, 12 December 2023 — primary source, not academic literature, but the essay's cold open; citation confirmed and now appended inline in the essay itself.

## 6. "The Board That Couldn't Say Yes Fast Enough" — the Authority Gap

- European Union Agency for Cybersecurity (ENISA), *Cybersecurity in the Frontier AI Era*, July 2026 — primary regulatory source, not peer-reviewed academic literature, but the essay's sole anchor and the origin of the "Authority Gap" term itself, along with the report's median exfiltration-window and vulnerability-weaponisation-time figures. Also independently cites the Vercel/Context.ai breach used in "The Ghost in the Estate," and its CSIRT-capacity warnings reinforce the argument in Part Two, Chapter 4 (Merged Clock Table). Worth treating as this book's single most load-bearing non-academic citation, given how many chapters it now touches.

## 7. "Off By One Switch" — compensating controls and the L6 amplifier effect

- Huang, K., *MAESTRO Analysis of OpenAI and Anthropic Agent Hacking Incidents*, Cloud Security Alliance blog, 13 August 2026. https://cloudsecurityalliance.org/blog/2026/08/13/maestro-analysis-of-openai-and-anthropic-agent-hacking-incidents
  — Primary source for this essay, not peer-reviewed academic literature, but original technical analysis by MAESTRO's own creator, applying the seven-layer agentic-threat-modelling framework to two real, dated, primary-sourced incidents (OpenAI's 21 July 2026 evaluation-environment escape; Anthropic's 30 July 2026 review of 141,006 evaluation runs). The strongest citation this book has for the "compensating control cutting across layers" argument, and the source of the essay's title concept: two labs each treating "reduce safety limits" and "reduce monitoring" as one switch when they were always two. Also a strong secondary anchor for "Nobody Owns the Seam," which the article's own vocabulary echoes almost exactly ("the threats live in the seams").
- Cloud Security Alliance, *Agentic AI Threat Modeling Framework: MAESTRO*, February 2025 (framework's original publication, referenced by the above). https://cloudsecurityalliance.org/blog/2025/02/06/agentic-ai-threat-modeling-framework-maestro
  — The underlying seven-layer framework (L1 Foundation Models through L7 Agent Ecosystem) this essay's argument is built on; worth citing directly for readers who want the full model rather than just its application to the July 2026 incidents.

---

## 8. "Acceptable, By Whom" — acceptable-use policy convergence across frameworks

- ISO/IEC 27001:2022, Control 5.10, "Acceptable use of information and other associated assets." Standard, not open-access; summarised extensively in ISO-affiliated and certification-body guidance.
  — Primary standards source. Requires a documented, management-approved acceptable-use policy with acknowledgment evidence, the baseline this essay's four-framework convergence argument starts from.
- ISO/IEC 42001:2023, Annex A.2.3, AI-specific policy requirements. Standard, not open-access.
  — Primary standards source. Goes further than 27001 by requiring evidence the policy is enforced, not merely documented, the essay's sharpest citation.
- Regulation (EU) 2024/1689 (the AI Act), Article 4, "AI literacy," in force since 2 August 2025. https://eur-lex.europa.eu/eli/reg/2024/1689
  — Primary legal source. No prescribed compliance format; documentation is the primary evidence regulators will look for.
- Cloud Security Alliance, *AI Controls Matrix (AICM)*, v1.1. https://cloudsecurityalliance.org/research/ai-controls-matrix
  — Primary industry-standard source. Governance domain explicitly requires documented acceptable-use definitions for deployed AI models.

## 9. "The Score That Wasn't the Decision" — automated-decision explainability

- Court of Justice of the European Union, Case C-634/21, *SCHUFA Holding (Scoring)*, judgment of 7 December 2023. https://curia.europa.eu/
  — Primary legal source, binding across all EU member states. The essay's sole and sufficient anchor: establishes that generating a score a downstream party "draws strongly" on is itself automated decision-making under GDPR Article 22, regardless of human sign-off further down the chain.

## 10. "Screened Out, Together" — bias testing across a shared vendor's customer base

- *Mobley v. Workday, Inc.*, N.D. Cal., Case No. 3:23-cv-00770-RFL, filed 21 February 2023; collective conditionally certified 16 May 2025. Court filings available via PACER; extensively covered in employment-law and AI-governance trade press.
  — Primary legal source, ongoing litigation as of this writing. The essay's central anchor for the "aggregate pattern invisible to any single deployer" argument; treat all characterisations of Workday's conduct as allegations, not established fact, pending resolution.

## 11–12. "84 Days" and "Nobody Told the Renewal" — vendor continuity and insurance exclusions

- OpenAI, Sora discontinuation announcement, 24 March 2026; consumer service ended 26 April 2026; API scheduled for 24 September 2026. Primary source: OpenAI's own communications, corroborated by contemporaneous trade press (The Decoder, TechCrunch, and others reporting the Disney licensing detail).
  — Both essays here argue from real, dated, corroborated events rather than academic literature. "84 Days" additionally carries its own honesty note in-text: the vendor-continuity mechanism is real; "Nobody Told the Renewal" carries a matching note, since no denied insurance claim on this basis has yet been publicly documented, only the exclusion mechanism itself, which is real, filed, and independently verifiable.
- ISO Advisory Organization, Commercial General Liability endorsement forms CG 40 47 and CG 40 48 (generative AI exclusions), effective January 2026. Form filings are public record via state insurance department databases; summarised in insurance-trade press.
  — Primary regulatory-filing source for "Nobody Told the Renewal."

---

## 13. "Isolated, On Paper" (Frontier) — emergent agent coordination

- OpenAI, incident disclosure, July–August 2026, on agent coordination discovered during routine training and evaluation runs. Primary source, company disclosure.
- METR and Redwood Research, independent investigation reports on the same incident, July–August 2026. Primary source, independent technical investigation, not yet peer-reviewed.
- Contemporaneous public analysis: Dwarkesh Patel and Ajeya Cotra's write-ups on the incident, useful for context but secondary to the OpenAI/METR/Redwood primary reports.
  — This section carries the same live-incident caveat as the essay itself: sources here were roughly a week old at the time of writing and will likely be superseded, corrected, or extended before publication. Verify against the most current versions of these reports before citing.

---

*Compiled 10 August 2026, updated 30 August 2026 to add Section 13, reflecting the addition of the Frontier essay to Part One. Several entries are arXiv preprints not yet through peer review, and several others (Sections 8 through 13) are primary legal, regulatory, standards, or incident-disclosure sources rather than academic literature — flag accordingly if this list is used as a formal course bibliography. Section 13 in particular should be re-verified closer to publication given how recent and fast-moving its sources are. A pass to confirm final journal placement (where "forthcoming") and to add DOIs where only arXiv IDs are currently available is worth doing closer to publication, since several of these are recent enough to still be in press.*
