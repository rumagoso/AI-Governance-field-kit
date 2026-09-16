# The Board That Couldn't Say Yes Fast Enough

*Every framework assumes a moment where a human reviews and approves. This is what happens when the moment is smaller than the approval process.*

In July 2026, ENISA gave the gap a name. Its report on cybersecurity in the frontier AI era described what it called the Authority Gap: the inability of human Change Advisory Boards to authorise an intervention inside the few minutes an autonomous exploit actually leaves them. The report cited industry research putting the median time from initial access to data exfiltration at seventy-two minutes. A CAB that meets weekly, or even one that can convene an emergency call in an hour, is not slow by any normal measure. It is simply answering a question the incident stopped asking twenty minutes ago.

The instinct is to read this as a tooling problem — faster dashboards, better automation, an AI copilot summarising the incident for the committee. That helps, but it doesn't touch the actual failure. The failure is structural: almost every governance framework, from internal change management to the AI Act's human-oversight provisions, assumes there is a moment. A point where a person looks at a proposed action and says yes or no before it happens. That assumption held for decades because the moment was always bigger than the decision. Now, for a meaningful share of incidents, it isn't.

The fix is not to make committees faster. It's to stop routing everything through the committee.

Most incidents don't need a Board-level decision at all. They need a pre-authorised action — a specific, bounded response that someone has already agreed, in writing, can happen without a meeting: isolate this class of host, revoke this category of credential, roll back this kind of deployment. The authorisation happened in advance, during a calm afternoon, by someone with the standing to give it. What executes at 2am is not a judgment call. It's the execution of a judgment call made weeks earlier.

But some incidents genuinely need the opposite: not faster execution, but faster escalation. The failure mode here isn't a committee moving too slowly on something small — it's an organisation moving too slowly to notice something large. The essay's real subject is naming, in advance, which incidents belong in which bucket, because doing that math during the incident is how both buckets get the wrong incident.

A short, named set of triggers that skip the normal ladder and go straight to whoever holds real authority — Board, CEO, whoever that is in your structure — tends to cover most of what actually matters:

- **Critical business function down** — a revenue-generating or contractually SLA'd service, not "something looks slow."
- **Critical customer impact** — named accounts, contractual notification clocks already running.
- **Existential threat** — to the company, or, and this is the trigger most frameworks quietly omit, to something larger than the company. ENISA's own report is explicit that frontier-AI-scale incidents can carry systemic risk beyond any single organisation.
- **Personal data breach** — the moment that starts GDPR's seventy-two-hour clock, the same clock a Clock Table exercise should already have surfaced.
- **Other regulatory breach** — NIS2, CRA, or whatever sector-specific obligation applies to you.

None of these triggers work if they're written vaguely enough that everything qualifies, or specifically enough that nothing ever does. "Significant impact" is not a trigger. A named threshold, tied to a named person who can recognise it in the moment — not just a Board member who reacts once someone finally tells them — is.

And the thresholds themselves won't travel unchanged across borders or sectors. A "critical customer" in a five-person consultancy is not a critical customer in a national payments processor. A "regulatory breach" trigger in financial services pulls in obligations that don't exist for a small manufacturer, and vice versa for CRA product-security duties. Rather than hand you fixed numbers, the worksheet asks the questions that produce them for your own context — what counts as critical here, decided once, by someone with the standing to decide it, not improvised at 2am by whoever picked up the phone.

The Authority Gap is not going away. Frontier AI didn't create the problem of committees being slower than incidents — it just shortened the incident until the mismatch became impossible to ignore. The organisations that will hold up are not the ones with the fastest committee. They're the ones that worked out, ahead of time, which decisions never needed a committee at all, and which ones needed to reach the people who could actually decide — fast, and by name — the moment it mattered.

---

*The practical version of this problem, a pre-authorised action ladder and a named escalation-trigger set, is addressed in the field manual, Part Two, "Naming Who Can Say Yes at 2am."*


*See it filled in: Ondas Digital's own six-hour gap becomes an authority ladder in Chapter 7.*
