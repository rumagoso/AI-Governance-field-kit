# Chapter 4: Naming Who Answers for the Seam

*Companion to "Nobody Owns the Seam"*

The essay's postmark-mcp incident worked precisely because a seam between two systems had no owner, fifteen clean releases had quietly become the reason nobody was still watching the sixteenth. This chapter is the record that makes "nobody" an unacceptable answer.

## Worked example

**Seam:** Internal agent calls third-party email-sending tool via MCP
**Direction:** Agent-to-tool
**Last reviewed:** 14 July 2026
**Named contact:** R. Aguiar, Platform Engineering
**Backup contact:** J. Mendes, Platform Engineering
**Trust basis:** Package has 40k weekly downloads, active maintainer, no incident history to date — not independently code-reviewed by us

That last field is doing the real work. "No incident history to date" is not the same claim as "safe." Writing it down as the actual reason this seam was left unmonitored is what makes it visible as an assumption instead of a fact.

## The inventory

One row per seam, every agent-to-agent and agent-to-tool boundary your systems actually depend on.

**Seam description**
Plain enough that someone unfamiliar with the integration can picture it: "our support agent queries a third-party knowledge base via API," not just a package name.

**Direction**
Agent-to-agent or agent-to-tool. The failure modes differ, and lumping them together hides which kind of seam you actually have the most of.

**Last reviewed**
The date someone actually looked at this seam's current behaviour and dependencies, not the date it was first set up.

**Named contact**
One person, not a team, not a rotating role. The person who gets paged first if this seam is the source of an incident.

**Backup contact**
A second named person, because the first one leaves, goes on leave, or is unreachable at 2am, and a seam whose only contact has left is functionally back to having no owner at all.

**Trust basis**
Why this seam was judged safe enough to leave unmonitored between reviews. "Vendor reputation," "long clean track record," "internal team wrote it," whatever's actually true. If the honest answer is "nobody ever formally decided, it just kept working," write that.

## Who fills this in, and when

Filled by whoever technically owns the integration, at the point it's built, not retrofitted across the whole stack in one sitting months later. A seam inventory built retroactively from memory will systematically miss the seams nobody thinks of as seams, the internal tool nobody considers "third party" because it's built by the team next door.

The failure mode specific to this chapter: a trust-basis field that never gets revisited. "Fifteen clean releases" was true right up until it wasn't. Set a review cadence tied to something other than a fixed calendar date, a major version bump, a change of maintainer, a new permission the integration starts requesting, any of which is a better trigger for re-reading this row than an annual reminder that arrives regardless of whether anything's actually changed.
