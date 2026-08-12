# Chapter 2: Building Your Own Merged Clock Table

*Companion to "Three Clocks, One Fire"*

The essay's matrix showed what happens when AI Act, NIS2, and GDPR notification clocks run on the same incident at once. It didn't show your matrix, because your matrix depends on which regimes actually bind you, which sector you're in, and which contracts layer on deadlines no regulation mentions at all. This chapter is that worksheet.

## Worked example

**Incident type:** AI-assisted credit scoring model malfunction, personal data exposed
**Regimes that apply:** AI Act (high-risk system) — yes. NIS2 — no, not an essential/important entity. GDPR — yes, personal data involved. Client SLA — yes, top-three client contract requires 24h notice on any data incident
**Shortest applicable deadline:** 24 hours (client SLA — shorter than GDPR's 72h)
**First-alert role:** Data Protection Officer, on-call rotation

One row, filled honestly, already surfaces something the essay warned about: the tightest clock here isn't a regulator's. It's a client's, and it's not on any compliance calendar because nobody thought to put a contract on the same table as a law.

## The worksheet

One row per incident type your organisation could plausibly face.

**Incident type**
Named plainly enough that someone under pressure can match a real event to it in seconds, not a legal category, a description: "model gives wrong output affecting a customer decision," not "Annex III high-risk malfunction."

**Regimes that apply to you**
Tick AI Act, NIS2, GDPR, any sector-specific regime, and contractual clocks, for this incident type specifically. Most organisations are not in scope for all of them at once; the point of ticking rather than assuming is to stop treating the essay's three-clock example as universal when your actual exposure might be two clocks, or five.

**Shortest applicable deadline**
Not a list of every deadline, the shortest one, because that's the one that actually governs your first move. A 72-hour GDPR clock is irrelevant to your first hour if a contract gives you 24.

**First-alert role**
Named role, not "whoever's on call" written literally. If your organisation doesn't have a role for this yet, that gap is the worksheet's most useful output.

## Who fills this in, and when

This one is filled by whoever owns incident response, in a room with whoever owns your contracts, before either of them is dealing with an actual incident. That pairing matters: the compliance side of an organisation usually knows the regulatory deadlines cold and has never seen the client contracts; the commercial side knows the contracts and has never read Article 73. The worksheet doesn't work if it's filled by only one of them guessing at the other's numbers.

The failure mode specific to this chapter: filling it in once and treating it as permanent. Regulatory deadlines get amended. Contracts get renewed with different terms. A clock table built in year one and never revisited is exactly the kind of stale artefact the rest of this book warns about, review it whenever a contract renews or a regulation you're subject to changes, not on a fixed annual schedule that may not line up with either.
