# Chapter 5: Building Your Own Label Chain of Custody

*Companion to "Every Hand That Touched It"*

The essay's argument was that a label attached once, at generation, is not the same claim as a label that survives to the point a viewer sees it. Screenshots, format conversions, and re-exports strip labels as a matter of routine, not malice. This chapter maps where that happens to your own content, before a regulator maps it for you.

## Worked example

```mermaid
flowchart TD
    A[Generation<br/>Marketing image, in-house SD fine-tune<br/>Label: embedded metadata] -->|survives| B[Internal asset library]
    B -->|LOST — CMS strips metadata| C[Website CMS]
    B -->|untested| D[Social scheduler]
    B -->|survives, watermark visible| E[Partner shares<br/>co-marketing kit]
    E -->|LOST — partner's own re-export tool<br/>crops watermark| F[Partner's social post]
    D -->|LOST — most platforms strip on upload| G[Public social post]
    C -->|survives, no further hops| H[End: website visitor]

    style C fill:#f88
    style F fill:#f88
    style G fill:#f88
    style H fill:#8f8
```

| Hop | Label survives by default? | Responsible | Last tested |
|---|---|---|---|
| Generation → Internal library | Yes (embedded metadata) | Marketing Ops | 03 Aug 2026 |
| Internal library → CMS | **No** — CMS strips metadata on optimisation | Web team | 03 Aug 2026 |
| Internal library → Social scheduler | **Untested** | Social media contractor | — |
| Internal library → Partner kit → Partner's post | **No** — partner's own re-export crops the watermark | *unassigned* | — |

One diagram, four rows, and the reader can already see what a linear checklist would have hidden: the same asset forks three ways from a single point, and each fork has an independent, different fate. The dead end with no name attached is the one worth acting on first.

## Building your own

**Map the hops.** Start at generation and follow every path your content actually takes, not the path your policy says it should take. Include the ones you're not proud of, the partner handoff nobody reviewed, the contractor's own tools.

**Test, don't assume.** A label surviving one hop is not evidence it survives the next. Each edge in the diagram gets its own answer: yes, no, or untested, and untested is the honest default until someone actually checks.

**Name a responsible party per hop, not per asset.** The person accountable for the label surviving the CMS upload is not automatically the person accountable for it surviving a partner's re-export. Different hop, different point of failure, different name.

## Who fills this in, and when

Filled jointly by whoever owns content generation and whoever owns each downstream distribution channel, redrawn whenever a new distribution path is added, a new partner, a new platform, a new re-posting workflow. A diagram drawn once at launch and never touched again will silently stop matching reality the first time marketing adds a channel nobody thought to loop back into this chapter.

The failure mode specific to this chapter: testing the easy hops and leaving the inconvenient ones marked "untested" indefinitely. An untested hop several steps removed from your own systems, the partner's re-export, the third-party scheduler, is usually the one most likely to be losing the label, precisely because it's furthest from anyone who'd notice.
