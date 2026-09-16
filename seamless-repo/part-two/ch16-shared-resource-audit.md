# Naming What You Haven't Checked

*Companion to "Isolated, On Paper"*

Most of this book asks you to name an owner. This chapter asks something narrower and, in a specific way, harder: not who's responsible for a system, but which resources two of your own, separately-owned systems can both write to, resources nobody designed as a communication channel and nobody has therefore ever thought to check.

## Worked example

**Shared resource:** A package-manager cache, used by two of Ondas Digital's internal automation tools, the client-reporting agent and the campaign-scheduling agent, both maintained by Bruno Alves but run as separate, unrelated jobs
**Why it's shared:** Both tools install the same handful of Python packages on the same build server; sharing the cache was a cost and speed optimisation, decided in 2025, before either tool involved an AI agent making autonomous decisions about its own execution
**Could it carry an unintended signal:** Untested. Both agents can write arbitrary filenames into the same cache directory. Nobody had asked, before this exercise, whether one agent's output could be read by the other as anything other than a caching artefact
**Isolation assumed or verified:** Assumed. The build server's architecture diagram shows the two jobs as unconnected, which is true of their intended data flows and says nothing about the cache
**Action taken:** Cache directories separated per job, 4 March 2027; the shared build-speed optimisation was worth less than the unaudited channel it created

Nothing in this example involved anything as dramatic as the essay's anchor. That's the point. The mechanism, two systems sharing a writable resource nobody threat-modelled, is ordinary infrastructure, not frontier-lab infrastructure, which is exactly why it's worth checking at any scale.

## Building the audit

**Shared resource**
Named specifically: which cache, queue, shared filesystem, database, or logging destination two or more of your systems can both write to.

**Why it's shared**
The real, usually mundane, reason it exists. Cost, speed, convenience. Knowing the original reason helps you judge whether the risk is worth what it's saving.

**Could it carry an unintended signal**
The question most architecture reviews never ask, because the resource was never categorised as a communication channel, only as infrastructure. Answer honestly whether anyone has actually checked, or whether "no" just means "never asked."

**Isolation assumed or verified**
Whether your confidence that two systems are separate comes from an architecture diagram, which shows intended connections, or from an actual test of what they can reach.

**Action taken**
Separate the resource, monitor it, or make an informed, documented decision to accept the risk. All three are legitimate outcomes; leaving the field blank is not.

## Who fills this in, and when

Whoever owns the infrastructure two or more AI systems run on, not the owner of either individual system, since neither owner alone can see the shared resource from their own side. Run whenever two systems begin sharing any infrastructure for operational convenience, which, per the essay this chapter companions, is nearly always framed as an efficiency decision rather than a governance one at the time it's made.

The failure mode specific to this chapter: treating an architecture diagram as evidence of isolation. A diagram shows what a system was designed to do. It does not show what it can do with a resource nobody drew onto the diagram in the first place.
