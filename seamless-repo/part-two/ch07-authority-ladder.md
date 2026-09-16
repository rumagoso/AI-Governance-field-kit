# Chapter 10: Naming Who Can Say Yes at 2am

*Companion to "The Board That Couldn't Say Yes Fast Enough"*

## Worked example

When the lead-scoring incident (Chapter 6) happened, at 9pm on a Thursday, nobody at Ondas was authorised to pause the tool without reaching Mariana, who was on a flight and uncontactable for six hours. Tiago Vento, who spotted the misflagged batch, had the technical access to disable the integration in minutes. He didn't have the authority, and no one had ever written down whether he should.

Ondas built this ladder the following month. It pre-authorises Tiago to disable any client-facing AI integration immediately if it's producing incorrect customer-facing output, logged and reported to Mariana within the hour, no advance sign-off needed for that specific action. Separately, it names "any incident touching the bank client's customer data" as a trigger that skips the ladder entirely and goes straight to Mariana, regardless of the hour, because that one crosses into the 4-hour contractual clock Chapter 6 surfaced.

Same company, same kind of incident, and a second one wouldn't cost six hours of nobody being allowed to act.

## The pre-authorised action ladder

For each class of routine response, name in advance:
- The specific, bounded action (not "respond to incident" — "isolate hosts matching X," "revoke credentials of type Y")
- Who is authorised to execute it without further approval
- Who signed off on the authorisation, and when
- What must be logged once it's used

If an action isn't on this list, it isn't pre-authorised — it goes up the ladder instead.

## The escalation triggers

A short, named set of conditions that skip the ladder entirely and go straight to whoever holds real authority in your organisation:

- **Critical business function down**
- **Critical customer impact**
- **Existential threat** — to the organisation, or to something beyond it
- **Personal data breach**
- **Other regulatory breach**

For each trigger, work out your own threshold with these questions, rather than borrowing someone else's numbers:

- *Critical business function* — which functions, specifically, would you say this about out loud to a customer within the hour? What's the revenue or contractual threshold that makes something "critical" here, not just "annoying"?
- *Critical customer* — do you have named accounts with contractual notification clocks? What tier of customer, by revenue or by contract terms, triggers this versus a standard incident ticket?
- *Existential threat* — what would have to be true for this to threaten the organisation's continued operation? Is there a scenario, given what you build or operate, where the threat extends beyond your own walls — and who in your structure is responsible for recognising that scenario if it appears?
- *Personal data breach* — which regulation's clock applies to you (GDPR's 72 hours, a sector-specific variant, a client contract's shorter one)? Who is the named person that starts that clock the moment they know, not the moment it's confirmed?
- *Other regulatory breach* — which regimes actually apply to your sector and jurisdiction (NIS2 scope, CRA obligations, others)? Have you checked this in the last year, or is the list inherited from whenever it was last written?

Each trigger needs a named recogniser — someone whose job includes noticing the trigger has fired, not just a Board member who reacts once someone else finally calls.

## Who fills this in, and when

The ladder and the triggers are set jointly by whoever holds operational authority (CTO, security lead) and whoever holds organisational authority (CEO, Board) — not by the incident responder alone, and not retrofitted after an incident. Reviewed on a fixed cadence and after any incident that didn't fit cleanly into either bucket.

The failure mode specific to this chapter: triggers written vague enough that everything qualifies, or specific enough that nothing ever does. "Significant impact" is not a trigger. If your on-call responder can't tell, from the wording alone, which bucket a live incident belongs in, the wording isn't done yet.
