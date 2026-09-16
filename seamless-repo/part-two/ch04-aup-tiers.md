# Naming What "Acceptable" Actually Means Here

*Companion to "Acceptable, By Whom"*

## Worked example

**Tool:** Public ChatGPT (personal accounts, not managed by Ondas)
**Tier:** Conditional
**Data permitted:** Public information only, no client names, no unreleased campaign material, no client data of any kind
**Evidence of actual training:** 40-minute session, 3 March 2027, run by the CTO-as-a-service consultant after a client security questionnaire revealed staff had been using personal AI accounts unmanaged; walked through what Ondas's own client contracts actually restrict, quiz with an 80% pass threshold, not just an acknowledgment click
**Last reviewed:** 3 March 2027, tied to the client questionnaire that surfaced the gap
**Escalation for anything outside this tier:** Tiago Vento, response within one business day

**Tool:** Team-licensed Claude account (contracted, Ondas's own subscription)
**Tier:** Approved
**Data permitted:** Internal and client campaign material, excluding the bank client's data specifically, per that client's own contract terms
**Evidence of actual training:** Same 40-minute session, plus a second walkthrough of exactly what the bank client's contract does and doesn't allow
**Last reviewed:** 3 March 2027

Two tools, same underlying model family in one case, two different tiers, because the terms attached to each one are different. A single "AI is allowed" or "AI is banned" policy, which is what Ondas had before this exercise, meaning nothing written down at all, can't hold that distinction. A tiered one can.

## Building the tier list

**Tool**
Named specifically, including whether it's the consumer or enterprise version, since those frequently carry different data-handling terms under the same brand name.

**Tier**
Approved, Conditional, or Prohibited. Prohibited tools get a stated reason and, where relevant, a technical block, not just a line in a document nobody reads.

**Data permitted**
Specific enough that an employee could apply it to a real decision without asking someone first. "Use good judgment" is not a data classification.

**Evidence of actual training**
Not a click-through timestamp. A dated session, a walkthrough of real examples, ideally something with a pass/fail component. If this field can only point to an acknowledgment checkbox, the tool doesn't yet have real training behind it, regardless of what the tier says.

**Last reviewed**
Tied to an event, a vendor terms-of-service change, a new data-handling agreement, not a fixed calendar date that may not line up with either.

**Escalation contact**
Named person, for anything a tool or situation doesn't clearly fit.

## Who fills this in, and when

Built jointly by whoever owns AI governance and whoever owns IT security, before a new tool is approved for use, not after someone's already been using it for six months. Reviewed every time a new tool is requested or an existing tool's data-handling terms change, which, per Chapter 11 of this manual, happens more often than most inventories assume.

The failure mode specific to this chapter: treating the acknowledgment click as equivalent to the training-evidence field. They are not the same thing, and conflating them is the exact gap this essay's companion piece is about. An AUP tier list where every "evidence of training" field just says "signed policy on file" hasn't actually closed the gap; it's documented it.
