# Chapter 2: Building Your Own Merged Clock Table

*Companion to "Three Clocks, One Fire"*

The essay's matrix showed what happens when AI Act, NIS2, and GDPR notification clocks run on the same incident at once. It didn't show your matrix, because your matrix depends on which regimes actually bind you, which sector you're in, and which contracts layer on deadlines no regulation mentions at all. This chapter is that worksheet.

## Worked example

**Incident type:** Lead-scoring tool (from Chapter 5) misflags a batch of prospects, some contacted with an unauthorised loan offer
**Regimes that apply:** AI Act — unclear, Ondas never formally assessed whether this counts as high-risk; GDPR — yes, personal data and an automated flag driving contact decisions; DORA — possibly, Ondas may count as an ICT third-party service provider to the bank client, a category DORA extends obligations to even though Ondas itself isn't a financial entity; Client contract — yes, the bank's own contract requires 4-hour notice on anything touching customer data
**Shortest applicable deadline:** 4 hours (the bank's own contract, tighter than GDPR's 72 and far tighter than anyone at Ondas had prepared for)
**First-alert role:** Undecided at the time of the incident — this gap is what prompted building the table at all

One row, filled honestly after the fact rather than before, already surfaces what the essay warned about: the tightest clock wasn't a regulator's. It was a client's, buried in a contract nobody had cross-referenced against GDPR, let alone against DORA, which nobody at Ondas had realised might apply to them at all until this incident forced the question.

## The worksheet

One row per incident type your organisation could plausibly face.

**Incident type**
Named plainly enough that someone under pressure can match a real event to it in seconds, not a legal category, a description: "model gives wrong output affecting a customer decision," not "Annex III high-risk malfunction."

**Regimes that apply to you**
Tick AI Act, NIS2, GDPR, any sector-specific regime, and contractual clocks, for this incident type specifically. If you're in financial services, DORA belongs on this list explicitly, its ICT third-party risk pillar carries its own notification obligations and a penalty structure unlike the others, up to 2% of global turnover, with critical ICT providers facing a daily accrual on top of a fixed cap, a burn-rate penalty that changes how urgently this row needs answering. Most organisations are not in scope for all of them at once; the point of ticking rather than assuming is to stop treating the essay's three-clock example as universal when your actual exposure might be two clocks, or five.

**Shortest applicable deadline**
Not a list of every deadline, the shortest one, because that's the one that actually governs your first move. A 72-hour GDPR clock is irrelevant to your first hour if a contract gives you 24.

**First-alert role**
Named role, not "whoever's on call" written literally. If your organisation doesn't have a role for this yet, that gap is the worksheet's most useful output.

## Who fills this in, and when

This one is filled by whoever owns incident response, in a room with whoever owns your contracts, before either of them is dealing with an actual incident. That pairing matters: the compliance side of an organisation usually knows the regulatory deadlines cold and has never seen the client contracts; the commercial side knows the contracts and has never read Article 73. The worksheet doesn't work if it's filled by only one of them guessing at the other's numbers.

The failure mode specific to this chapter: filling it in once and treating it as permanent. Regulatory deadlines get amended. Contracts get renewed with different terms. A clock table built in year one and never revisited is exactly the kind of stale artefact the rest of this book warns about, review it whenever a contract renews or a regulation you're subject to changes, not on a fixed annual schedule that may not line up with either.

ENISA's 2026 report warns of a related, larger version of this problem at the national level: simultaneous incident surges now regularly exceed CSIRT capacity, multiple clocks (the AI Act, NIS2, the Cyber Resilience Act, and contractual deadlines alike) racing at once across an entire sector, not just inside one organisation. Your own worksheet is the small-scale version of a capacity problem regulators are now naming at the continental one.
