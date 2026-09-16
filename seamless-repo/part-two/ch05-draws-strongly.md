# Naming Whose Number This Actually Is

*Companion to "The Score That Wasn't the Decision"*

## Worked example

**System:** Lead-scoring tool Ondas built for the bank client, flags loan-product prospects as low/medium/high priority before the bank's own retail team follows up
**Downstream party:** The bank's retail sales team, technically free to contact any prospect regardless of score
**Draws strongly test:** Ondas pulled six months of the bank's own follow-up data at the client's request; high-priority flags got same-day callbacks 91% of the time, low-priority flags waited a week or more, or were never contacted at all
**Conclusion:** Yes, this draws strongly enough that the SCHUFA logic plausibly applies. The scoring step Ondas built, not just the bank's own follow-up decision, may carry Article 22 explainability obligations toward the prospects being scored
**Named owner of providing an explanation on request:** Flagged as unresolved, Ondas built the tool but the bank holds the customer relationship; contract doesn't currently say who answers a prospect's explanation request
**Explanation actually available:** No — the model outputs a priority flag with no factor breakdown at all. Gap raised with the bank client directly, contract amendment under discussion

That last line matters more than a clean yes. Finding a real gap and naming who still needs to resolve it is the actual deliverable here, not a tidy checklist that pretends the explanation already exists.

## Building the assessment

**System**
Named specifically, including what it outputs, a score, a rank, a flag, a recommendation.

**Downstream party**
Who receives that output and what they do with it.

**Draws strongly test**
Evidence, not assumption. How often does the downstream party's actual decision match the system's output? Interview the people making the final call rather than only reading the process document describing how it's supposed to work, the same gap Chapter 3 warns about for reviewer competence applies here too.

**Conclusion**
Whether the SCHUFA logic plausibly applies. When genuinely uncertain, treat it as if it does; the cost of being wrong the other way is discovering it in a regulator's inquiry or a data subject's complaint.

**Named owner of providing an explanation on request**
One person accountable for producing an actual, comprehensible explanation within the applicable deadline, not a generic contact address that hasn't been briefed on what data subjects are legally entitled to receive.

**Explanation actually available**
Honestly assessed. A model that can output feature weights is not the same as an organisation that can hand a rejected applicant a comprehensible reason.

## Who fills this in, and when

Filled by whoever owns the scoring system, together with legal or data protection, for every system whose output meaningfully influences a decision about an individual, before a data subject access request arrives rather than in response to one. Revisited whenever the downstream process changes, since a system that used to get overridden regularly and now rarely does has quietly crossed from advisory to decisive without anyone updating its Article 22 status.

The failure mode specific to this chapter: assuming a human-in-the-loop automatically exempts a system from these obligations. The SCHUFA ruling exists specifically because that assumption was wrong for exactly this kind of system, and it is binding across every EU member state, not a single jurisdiction's quirk.
