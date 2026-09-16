# Naming Who Triggers the Migration

*Companion to "84 Days"*

## Worked example

**Vendor / product:** Third-party AI video-generation tool Sofia uses for client campaign content
**Export/portability tested:** Yes, tested 15 May 2026, the week after a smaller competing tool Ondas had also relied on announced its own shutdown with three weeks' notice, which is what prompted Sofia to check this one before it happened to her too. Full asset export took 25 minutes, confirmed usable elsewhere
**Estimated full migration time if this vendor discontinues:** 1–2 weeks, three active client campaigns depend on it at any given time
**Named migration-trigger owner:** Sofia Reis
**Trigger condition:** Any formal discontinuation notice, regardless of stated timeline, starts migration planning within 48 hours, not at the deadline

That last field exists because Ondas already lived the alternative once, with the smaller tool, where nobody had a plan and three weeks of notice turned into three weeks of scrambling. The trigger isn't "when the vendor shuts down." It's "when the vendor says it will," which, on Ondas's own recent evidence, can be barely a month.

## Building the register

**Vendor / product**
Every AI tool or API a real workflow depends on, not just the ones with the most spend attached, a free or cheap tool a team has quietly built a habit around carries the same discontinuation risk as an expensive one.

**Export/portability tested**
Not assumed, actually tried. A vendor's documentation claiming data export is possible is not the same as someone on your team having done it and confirmed the result is usable elsewhere.

**Estimated full migration time**
A real estimate, even a rough one, based on actual dependency, not a guess made under pressure during an actual shutdown notice.

**Named migration-trigger owner**
One person accountable for starting the migration process the moment a trigger condition is met, not for deciding whether to start it, that decision should already be made in this register.

**Trigger condition**
Defined precisely enough that a discontinuation announcement, however it arrives, is unambiguously recognised as the trigger. "We'll figure it out when it happens" is not a trigger condition.

## Who fills this in, and when

Built by whoever owns the workflow depending on the vendor, for every AI tool the business would genuinely struggle to lose without notice. Reviewed whenever a new critical dependency is adopted, and tested, the export step actually run, at least annually, since a vendor's export tooling can silently degrade or change between when it was last checked and when it's actually needed.

The failure mode specific to this chapter: treating a vendor's contract terms as equivalent to actual continuity protection. A termination-notice clause is a legal promise about warning, not a technical guarantee about how much of that warning translates into real, usable time, as the gap between OpenAI's public announcement and Disney's own notice period demonstrates even for a counterparty with real negotiating leverage.
