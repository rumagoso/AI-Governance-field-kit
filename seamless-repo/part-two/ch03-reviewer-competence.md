# Chapter 6: Naming What Your Reviewers Need to Know

*Companion to "Qualified to Disagree"*

Steven Schwartz reviewed his own brief before filing it. He was qualified to practise law and unqualified to catch a fabricated citation, because nothing in twenty years of legal training had ever needed to teach him that a well-formatted case reference might not exist. This chapter names, per system, the specific thing a reviewer needs to have been shown before their sign-off means anything.

## Worked example

**System:** AI-drafted contract summaries (LEGAL-AI-003)
**Named reviewer:** T. Vieira, Senior Associate
**Known failure mode:** Model occasionally invents a clause reference that reads as plausible but does not appear in the source document
**Evidence reviewer was shown this failure mode:** Walked through two real examples flagged by QA, 9 June 2026, before this reviewer was assigned to the workflow
**Last caught incident:** 3 July 2026 — reviewer flagged an invented indemnity clause reference before the summary went to the client

That last field earning a real date is what makes this record worth more than a training certificate. A reviewer who can point to something they actually caught has demonstrated the competence this chapter is trying to verify. A reviewer with no entry there yet isn't necessarily failing, but the blank is worth knowing about before an incident makes it visible.

## The record

One per AI system that has a human reviewer in its workflow.

**System and use**
What the system does and where its output goes, enough context to know what's actually at stake if the reviewer misses something.

**Named reviewer(s)**
Not a role, a role rotates without anyone updating this record. The actual person or people currently doing the review.

**Known failure mode**
Not "AI can be wrong," the specific pattern this system is known or expected to produce: fabricated citations, confidently wrong numbers that look right, miscategorised items, whatever applies. General AI literacy does not transfer to catching a specific tool's specific way of failing, and this field exists to stop pretending it does.

**Evidence reviewer was shown this failure mode**
A training session, a worked example, a real incident walkthrough, dated, before the reviewer started signing off on this system's output. "They're experienced" is not evidence. A specific session with a specific date is.

**Last caught incident**
The most recent time this reviewer actually caught something wrong, or an honest blank if there isn't one. Leave it blank rather than filling it with something vague; the blank is the finding.

## Who fills this in, and when

Filled by whoever manages the reviewer, updated the first time the reviewer is assigned to this specific system, and again the first time they catch, or clearly miss, something. This record decays the same way an inventory does: a reviewer trained on a system's failure modes eighteen months ago, on a system that's since been updated by its vendor, may no longer be trained on what the system currently does wrong.

The failure mode specific to this chapter: treating a strong reviewer's general reputation as evidence for this specific record. Seniority is not competence in a failure mode nobody taught anyone to expect. If the "evidence shown" field can't point to an actual dated session, the honest tier is "not yet demonstrated," regardless of how senior the name attached to it is.
