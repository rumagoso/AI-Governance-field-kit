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
- U.S. Government Accountability Office (GAO), review of 23 federal agency AI inventories (2025–2026) — primary source, not academic literature, but the essay's cold open; cite as a GAO report rather than a paper. Worth locating the exact GAO report number before publication for a precise citation.

---

*Compiled 10 August 2026. Several entries are arXiv preprints not yet through peer review — flag accordingly if used in a formal academic bibliography. A pass to confirm final journal placement (where "forthcoming") and to add DOIs where only arXiv IDs are currently available is worth doing closer to publication, since several of these are recent enough to still be in press.*
