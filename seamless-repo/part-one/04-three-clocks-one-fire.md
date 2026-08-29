# Three Clocks, One Fire

*Three regulations start three different incident clocks the moment something goes wrong, and no incident response plan names who's supposed to read all three at once.*

03:14. Something in the pipeline is clearly wrong. Nobody has confirmed what, yet, or how bad, or whether anyone outside the room needs to know.

Three clocks have already started. Nobody pressed a button. Nobody chose to start them.

One fire. Three clocks.

## The Clocks

**AI Act, Article 73.** If a high-risk system caused it, the provider reports to market surveillance. Fifteen days, as a rule. Ten, if someone may have died. Two, if it's widespread or critical infrastructure took a serious, irreversible hit. And if you're the deployer, not the provider — Article 26(5) — you don't even get fifteen days to think about it. Twenty-four hours to tell the provider. Then the clock is theirs, but you're already in the chain.

**NIS2.** In Portugal, the cascade runs tighter than the "24/72" everyone quotes from memory. Initial notification within 24 hours. An update at 72. End-of-impact notification within 24 hours of resolution. A final report within 30 working days. Four deadlines, not two.

**GDPR.** Seventy-two hours to the supervisory authority, if personal data moved. A different 72 hours than NIS2's. Nobody tells you that on day one.

Three clocks. Different starts. Different owners. Same fire.

## Why They Don't Line Up

An AI Act "serious incident" and a NIS2 "significant incident" and a GDPR "personal data breach" are not the same event wearing three names. They're three different tests, applied to the same facts, sometimes returning three different answers. Your system might clear the NIS2 bar and miss the AI Act one. Or trip GDPR without coming close to either.

Which means someone has to run all three tests, at 03:14, before any of them can start ticking honestly.

Here's a smaller asymmetry that's easy to miss until you draw the three side by side: the AI Act has a fast lane if someone may have died — ten days instead of fifteen. NIS2's cascade has no equivalent. Its four deadlines are keyed to severity of impact on the service, not to whether a person was harmed. The regulation built specifically around AI harm has a human-injury clock. The regulation built around critical infrastructure and essential services doesn't. Not a gap in anyone's implementation — a genuine difference in what the two laws were built to notice.

Who runs them?

In most organisations — mine included, and I doubt we're unusual — the honest answer is: whoever's awake decides, and the decision about who that should be was never actually made. Not written down. Not assigned. Not tested. A single incident response plan tends to name an incident commander. It rarely names who owns the *classification* — the person whose job it is to say, out loud, at minute one, "this trips wire two and wire three, not wire one."

That's not a technicality. Get the classification wrong and you're not late by minutes. You're late by a clock you never started.

## The Unresolved Thing

Nobody has built the merged matrix. Not us, not — as far as I can tell — most of the organisations racing toward the same August deadlines.

What happens instead: the matrix gets built live, during the incident, by whoever's in the room, under the worst possible conditions for careful cross-referencing three regulations against fact patterns nobody has fully confirmed yet.

That's the actual risk. Not the incident. The incident was always going to happen eventually — that's what incident response is for. The risk is discovering, at 03:20, that your only classification tool is a tired person's memory of three different regulations they half-read months ago.

## The Merged Matrix

One table. Built once, before the fire, not during it.

| Trigger | AI Act 73 | NIS2 (PT) | GDPR | Who classifies |
|---|---|---|---|---|
| High-risk AI system malfunction, no personal data, no critical infra | 15 days (provider) / 24h to provider (deployer) | — unless it meets significant-incident criteria | — | Named role, not "whoever's on call" |
| Same, plus personal data exposed | 15 days | Maybe | 72h | Named role |
| Death or serious injury plausibly linked | 10 days | 24h initial | 72h if personal data | Named role |
| Widespread / critical infrastructure disruption | 2 days | 24h initial, 72h update, 24h end-of-impact, 30 working days final | 72h if personal data | Named role |

The columns aren't the hard part. Regulations publish their own deadlines; anyone can look them up at 3pm on a Tuesday. The hard part, the part worth actually building before you need it, is the last column. Not the clocks. Who reads them.

Three clocks started tonight, and none of them asked permission.

The only real question left is whether anyone was ever named to hold the watch.

---

*The merged matrix above is the seed of a living document, the field manual, Part Two, "Building Your Own Merged Clock Table," walks through adapting it to your own regulatory footprint and naming the classification role before you need one.*