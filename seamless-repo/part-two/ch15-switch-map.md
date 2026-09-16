# Chapter 11: Naming What One Switch Actually Turns Off

*Companion to "Off By One Switch"*

## Worked example

**Control being disabled:** Content-safety filtering on the bank client's chatbot, for a stress test Bruno ran to see how it handled hostile or off-topic questions
**Intended effect:** Let the model respond to deliberately awkward test prompts instead of refusing them, so Bruno could evaluate whether the refusals were too aggressive
**Other things bundled with this flag, discovered on inspection:** The same setting that disabled content filtering also disabled the conversation-logging Bruno had built for the bank's own compliance review, because he'd wired both to the same debug flag eighteen months earlier and never revisited it
**Verified still active before the run:** No — Bruno assumed logging was separate, the same assumption the essay describes at two frontier labs, at a much smaller scale
**Action taken:** Logging separated into its own flag; the stress-test run itself flagged as unverified and quietly re-run properly the following week

One five-minute inspection, done before the run rather than after, would have caught this. Bruno hadn't done anything unusual or careless by the standards of how Ondas built things generally. That's exactly the problem this chapter exists to fix.

## The switch map

For every control your organisation can disable, temporarily or permanently, for testing, debugging, or research:

**Control being disabled**
Named specifically. "Safety settings off" is not specific enough to audit; "content-safety filtering, environment flag SAFETY_MODE" is.

**Intended effect**
What the person flipping the switch actually wants to happen, in one sentence.

**Other things bundled with this flag**
The part that takes actual investigation: what else, in the code, the infrastructure, or the process, changes when this flag changes, whether or not anyone intended it to. This is usually discovered by reading the actual implementation, not by asking whoever built it what they remember it doing.

**Verified still active before the run**
Whether someone actually checked, this time, that the things not meant to change stayed unchanged. "It worked last time" is not verification.

## Who fills this in, and when

Filled by whoever has technical access to actually disable the control, before the first time it's used, not after something goes wrong while it's active. Revisited any time the underlying system the flag lives in gets refactored, since bundling that didn't exist at build time can be introduced later by an unrelated change.

The failure mode specific to this chapter: treating this as a one-time audit rather than a standing check run every time the switch gets used. A flag that was cleanly separated from other controls in January can become silently bundled again after a refactor in June, and nobody re-checks a control that already passed once.
