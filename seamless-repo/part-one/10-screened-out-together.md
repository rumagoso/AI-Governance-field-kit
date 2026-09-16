# Screened Out, Together

*A hundred rejected applications, several within the hour, some at hours no recruiter was reading them. A federal court is now deciding whether the vendor whose software rejected them can be held liable alongside every employer who used it.*

In July 2024, a federal court declined to accept that defence at face value, allowing the claims to proceed on the theory that Workday could be liable as an agent of the employers using its tools, a legal category built for one company acting on another's behalf, applied here to software making recommendations at a scale no individual employer's HR department was actually reviewing. In May 2025, the court went further, conditionally certifying the case as a nationwide collective action. Workday's own filings put the potential scope at over a billion rejected applications during the relevant window; the court noted the collective could run into the hundreds of millions. Discovery is ongoing as of mid-2026.

## A bias test built for the wrong number of defendants

The AI Act, alongside a growing list of national and municipal rules, requires bias testing for high-risk employment systems. The obligation is written for a straightforward picture: one organisation, one system, one set of applicants, test it, document the result, move on. Mobley v. Workday is what happens when that picture is wrong in a specific way. Workday's screening tools aren't one company's system. They're one vendor's system, deployed with local variations across hundreds of separate employers, each of whom can run a bias audit on their own hiring process and find nothing alarming in isolation, because the pattern Mobley alleges only becomes visible in aggregate, across a customer base no single employer can see into and no single employer's audit was ever designed to catch.

This is not quite the seam problem an earlier essay in this collection describes, where the gap sits in who explains an incident after it happens. Here the system is known, named, and heavily used; nobody's confused about what it is. The gap is upstream of any single incident: who is actually testing this pattern for bias, given that no party in the chain, not the individual employer, not the vendor insisting it merely sells software, has full visibility into the aggregate outcome their own compliance obligation is supposed to cover.

## The test that expires quietly

A second problem compounds the first. One commentator following the case put it plainly: an employer's AI may have passed a bias audit in 2025 while having produced discriminatory outcomes across 2021 to 2023, with no contemporaneous monitoring in between to have caught it. In litigation, that observation continued, that isn't a compliance gap. It's negligence. A bias test is a snapshot. The collective action's window in Mobley runs back to September 2020, five years of hiring decisions now sitting in an evidentiary pool that no annual or point-in-time audit was built to cover retroactively. This is the same evidence-decay problem an earlier essay in this book describes for AI inventories generally, applied here to fairness specifically, and arguably with sharper teeth, since the gap isn't discovered by an internal reviewer. It's discovered by opposing counsel.

## What the two-party structure actually demands

Neither "the vendor should test it" nor "the employer should test it" survives contact with how these systems are actually built and sold. The vendor controls the model and can see patterns across its full customer base that no individual employer ever could. The employer controls the specific configuration, the job criteria, the actual population of applicants being screened, details the vendor doesn't fully see either. A bias-testing obligation that assumes either party alone has the full picture will keep missing exactly the pattern Mobley alleges: one only visible in the aggregate, sitting in the space between a vendor's shared model and a thousand employers' individual, each individually clean, deployments.

The honest requirement isn't a single retest by a single party. It's a named allocation, decided in advance and in writing, of which aggregate-level testing the vendor is responsible for and which configuration-level testing sits with the deployer, reviewed on a cadence that doesn't let five years of drift accumulate silently in between. Nobody currently owns that allocation by default. A federal court is now the first place it's actually being drawn.


---

*The practical version of this problem, an explicit allocation naming which aggregate-level bias testing the vendor owns and which configuration-level testing the deployer owns, with the gap between them stated in writing rather than assumed away, is addressed in the field manual, Part Two, "Naming Who Tests for Bias, at Which Level."*

*See it filled in: Ondas Digital's Inês Duarte confronts what she can't test for, in Chapter 10.*
