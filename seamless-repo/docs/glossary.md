# Glossary

Plain-language definitions for the specific terms used across this book, in the order they first appear rather than alphabetically, since most readers will look one up mid-chapter rather than browse the whole list.

**Decommissioning** — Formally retiring an AI system: deciding what happens to its data, telling everyone who depended on it, and taking it off the active inventory. Distinct from a system simply being abandoned or forgotten.

**Human oversight (AI Act, Art. 14/26)** — The Act's requirement that a person be positioned to understand, monitor, and intervene in an AI system's operation. This book distinguishes *presence* (someone is there), *competence* (they're equipped to catch a specific failure), and *comprehension* (they actually understood what they signed off on), three different things the phrase "human oversight: yes" tends to collapse into one.

**AI literacy (AI Act, Art. 4)** — A requirement, active since 2 August 2025, that staff and anyone acting on a provider or deployer's behalf have sufficient understanding of AI to use it responsibly, given their role. No prescribed format; documentation is the primary evidence regulators look for.

**NIS2** — The EU's second Network and Information Security directive, setting incident-notification and risk-management obligations for essential and important entities.

**DORA** — The EU's Digital Operational Resilience Act, financial-sector-specific, extending obligations to a financial entity's ICT third-party providers, not just the financial entity itself. Its penalty structure can include a daily accrual on top of a fixed cap for critical providers.

**Authority Gap** — A term from ENISA's 2026 frontier-AI cybersecurity report describing the mismatch between how fast a modern incident moves and how fast a human approval process (a Change Advisory Board, for instance) can realistically respond.

**Seam** — Any point where two systems, two teams, or two organisations hand off to each other. This book's central term: seams are where accountability tends to disappear, because each side can plausibly point to the other.

**MAESTRO** — A seven-layer threat-modelling framework for agentic AI systems, published by the Cloud Security Alliance, running from L1 (foundation models) to L7 (the agent ecosystem). Used in this book to analyse how a single disabled control can silently remove protection across several layers at once.

**Provider vs. deployer (AI Act, Art. 3/25)** — A provider builds or substantially modifies an AI system and carries the Act's full compliance weight; a deployer merely uses one. Article 25 sets out when a deployer's own actions, rebranding, fine-tuning, repurposing, can reclassify them as a provider without anyone deciding that on purpose.

**Article 50 (AI Act)** — The Act's transparency provision: providers must mark generative AI output as artificial; deployers carry separate disclosure duties for deepfakes and certain AI-generated public-interest text.

**Draws strongly (GDPR Art. 22, CJEU SCHUFA ruling)** — The legal test, from a December 2023 CJEU ruling, for whether producing an automated score counts as the decision itself: if a downstream party relies heavily on the score to decide, generating it is automated decision-making, regardless of whether a human signs off afterward.

**Chain of custody (content labelling)** — Whether a label marking content as AI-generated survives every hop it travels through after creation, not just whether it was attached correctly at the start.

**CSA AICM** — The Cloud Security Alliance's AI Controls Matrix, a control framework with explicit requirements around AI governance, including documented acceptable-use definitions.

**ISO 27001 / ISO 42001** — International standards for information security management (27001) and AI management systems specifically (42001). 42001 goes further than 27001 by requiring evidence that policies are enforced, not merely documented.

**Silent AI coverage** — The industry term for the pre-2026 assumption that general commercial liability, cyber, or tech E&O insurance implicitly covered AI-related claims, an assumption new ISO exclusion forms (CG 40 47/48) explicitly ended.

**Compensating control** — A safeguard, often monitoring or a kill switch, that cuts across several parts of a system rather than belonging to just one. This book's argument is that disabling one control can silently remove a compensating control for several others at once, without anyone realising the two were ever connected.
