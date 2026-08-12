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
| Human participation tier(s) (see note) | ○ | — | ○ | ○ | — |
| Impact assessment reference (DPIA / FRIA) | ● (deployer) | ● | ○ | ○ | ○ |
| Public / releasable status | ○ | — | — | — | ● |
| Retraining / version-change log | ○ | ○ | ● | ● | ○ |

**Reading the table:** the AI Act and the US federal inventory regime are the two most prescriptive on *identity and status* fields — who, what, is it still running. GDPR is the strictest on *data category and accountable controller*, inherited whenever an AI system touches personal data regardless of AI-specific law. NIST's RMF and ISO 42001 are the two that actually ask for *lifecycle and change* fields — the ones everyone's inventory tends to go stale on first, per the earlier piece in this series on inventory decay.

A record missing the life-cycle-stage and version-change fields will satisfy the AI Act's registration on day one and fail the moment anyone asks whether the entry still describes what's actually running.


**Note on the human-participation-tier row:** none of the five regimes currently mandate this field by name, which is precisely the gap it exists to close. "Named accountable human" satisfies the letter of AI Act Article 14, ISO 42001, and GDPR's controller requirement while leaving open whether that person does any genuine evaluation at all. Recording which of five participation tiers applies, evaluative review, bounded review, procedural sign-off, no human touchpoint, or shared and ambiguous, and noting that a system can carry more than one, turns "human oversight: yes" from a box tick into an honest description of what actually happens.