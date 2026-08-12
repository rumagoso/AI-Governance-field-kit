# Chapter 7: Finding the Ghosts in Your Own Estate

*Companion to "The Ghost in the Estate"*

Vercel's breach didn't come from a weak control. It came from a tool nobody had counted, connected by one employee's personal login, invisible to every control downstream because none of them knew there was anything there to control. A checklist that just says "inventory your AI tools" is useless against that; the tools worth worrying about are, by definition, the ones evading the normal ways you'd notice them. This chapter is a routine, not a form.

## Worked example

**Run date:** 4 August 2026
**Method used:** OAuth/SSO grant review
**Finding:** Three "Sign in with Google Workspace" grants to AI writing tools, none matching the approved-vendor list, granted by three different employees between February and June
**Action:** Two tools removed from access within 48 hours; one escalated for a proper vendor review after the team explained it had become part of their actual workflow

The point isn't that ghosts got found. It's that the routine turned "someone might be using something we don't know about" into three named tools with dates, which is the only form that gap can actually be acted on.

## The routine

**OAuth/SSO grant review.** What's connected to your Google or Microsoft workspace via "sign in with," sorted by app name. Flag anything AI-related nobody explicitly approved.

**Browser extension audit.** Via endpoint management if you have it, via a short honest staff survey if you don't. Extensions are one of the quietest ways an AI tool enters a workflow.

**Expense and procurement scan.** Small recurring charges to AI vendors that never went through a security review. Shadow AI is frequently paid for on a personal card and expensed quietly, under the radar of any procurement process built for larger purchases.

**DNS or network egress check.** Traffic to known AI API domains not accounted for in your approved tool list. Needs technical means to run, but is the hardest of the four to fool, since it catches usage even when nobody signed in with anything traceable.

Each method needs an owner, a frequency, and, critically, a defined next step. A ghost found and left un-actioned is worse than one never looked for, it turns "we didn't know" into "we knew and didn't do anything," which is a materially worse position in almost every regulatory framework this book touches.

## Who fills this in, and when

Run by whoever owns IT security or asset management, on a cadence, not a one-off. A single clean sweep tells you what existed on that day. New ghosts appear continuously, someone signs up for something new the week after your last review, so the routine only earns its keep if it repeats.

The failure mode specific to this chapter: running the easy methods, OAuth review is quick, and skipping the harder ones indefinitely because they take more effort to set up. The DNS check is usually the one that gets skipped, and it's also usually the one most likely to catch what the other three miss.
