# If You Can Only Do This Much This Quarter

Sixteen chapters, all real, none of them urgent in the same way. This page ranks them by a simple test: how likely is the gap, and how bad is it when it bites. Not a substitute for judgement about your own situation, a starting order for a company that hasn't done any of this yet.

## Tier 1 — do these first, they're cheap and the gap is common

- **Ch.4, AUP Tiers.** Almost every company already has this exposure right now, staff using AI tools with no policy at all, and it costs an afternoon to fix the first pass.
- **Ch.8, Seam Inventory.** If you have any AI system calling a third-party tool or agent, this gap already exists and is usually invisible until an incident forces it into view.
- **Ch.14, Finding the Ghosts.** You cannot govern what you haven't counted. This is the precondition for most of the other chapters actually working.
- **Ch.1, Decommission Record.** Cheap to start applying going forward; the retroactive version (finding what's already been abandoned) is worth doing once, early.

## Tier 2 — do these once Tier 1 is running, higher stakes, more setup

- **Ch.6, Merged Clock Table.** Not urgent until the day it's extremely urgent. Worth having answered before an incident, not during one.
- **Ch.7, Authority Ladder.** Pairs naturally with Ch.6; both are about being ready before the clock starts, not during.
- **Ch.11, Provider Status Check.** Run this on every AI system you've built on top of a third-party model, especially anything fine-tuned or rebranded. The cost of getting this wrong compounds the longer it goes unchecked.
- **Ch.13, Insurance Coverage Check.** One conversation with your broker. Rare to need it urgently, expensive to discover the gap after a claim.

## Tier 3 — genuinely important, but only if the specific exposure applies to you

- **Ch.10, Bias Testing Allocation.** Essential if you use or sell AI systems that screen, rank, or score people. Skippable, honestly, if you don't.
- **Ch.5, Draws Strongly Test.** Same logic, only relevant if an automated score of yours meaningfully drives someone else's decision about an individual.
- **Ch.9, Label Chain of Custody.** Matters if you generate AI content that leaves your organisation. Low relevance if you don't.
- **Ch.12, Vendor Continuity Register.** Worth doing for whichever single AI tool your business would genuinely struggle to lose without warning. Not worth doing exhaustively for every minor tool.

## Tier 4 — do these once the above are stable

- **Ch.2, Human Participation Tiers** and **Ch.3, Reviewer Competence.** Both assume you already know which systems have humans reviewing them; worth doing properly once your inventory (Tier 1) is trustworthy.
- **Ch.15, Switch Map.** Relevant mainly if you're actively testing or red-teaming your own AI systems. Most SMEs aren't yet.
- **Ch.16, Reading the System.** The synthesis only works once several other chapters have something in them to synthesise. Doing it early just produces a page of "not started."

The pattern underneath this ranking, if you want it: start with the chapters that find out what you don't know (4, 8, 14), then the ones that get you ready before an incident (6, 7, 11, 13), then the ones that only apply if a specific kind of system is in play (5, 9, 10, 12), then the ones that assume the rest is already working (2, 3, 15, 16).
