# Nobody Owns the Seam

*A malicious npm package impersonating a legitimate Postmark tool ran clean for fifteen releases before one line quietly started copying every email agents sent to an attacker, and nobody, on either side of that seam, had agreed in advance whose job it was to keep watching.*

For fifteen straight versions, a small npm package called postmark-mcp did exactly what it claimed: it gave AI agents a tool for sending email through Postmark's service, faithfully, release after release, until developers were recommending it to colleagues as a reliable piece of the stack. Then, in version 1.0.16, one line was added to the email-sending function: a hardcoded address in the BCC field. From that point on, every email an agent sent through the tool was silently copied to the attacker. The package had impersonated Postmark's own MCP server closely enough that almost nobody checked; it was downloaded over sixteen hundred times before anyone caught the change, and because the flaw was a behavioural one rather than a code vulnerability, it never qualified for a formal vulnerability identifier at all.

No agent misbehaved. Each one called the tool it had always called, exactly as designed, and received back exactly the success response it expected. The email vendor's own systems were untouched. The organisations running the agents had, in most cases, done nothing wrong that any existing checklist would have caught. What failed was the seam between an agent and a tool it had learned, over fifteen honest releases, to trust — and nobody, on any side of that seam, had a job description that included watching it continuously.

That is the seam this piece is about, and it is worth being precise about why it is a new kind of problem rather than an old one wearing new branding.

## A seam that predates the ink

Multi-vendor integration failures are not new; contract law has been allocating blame across API boundaries for as long as APIs have existed. What is new is the timing. A traditional integration — even a bad one — is a fixed thing: Vendor A calls Vendor B, the pairing is known in advance, and a contract, however imperfect, can in principle be written for the arrangement that will actually run in production.

Agent-to-agent systems increasingly don't offer that courtesy. An agent may select, compose, or spin up a sub-agent at runtime, in response to conditions that didn't exist when anyone was drafting terms. The call graph that produces an incident may simply not have existed at design time — not because nobody thought to document it, but because it hadn't been assembled yet. You cannot pre-negotiate accountability for a combination nobody chose in advance. That is not a maturity problem that better contract templates will eventually fix. It is contracts running up against a system that finishes assembling itself after the paperwork is signed.

## The frameworks arrived, and solved a different layer

To be fair to the industry, this has not gone unnoticed. The Cloud Security Alliance's MAESTRO framework maps exactly this kind of cross-agent threat surface; OWASP's work on agentic systems names cross-agent trust and excessive delegation as first-class risks. Anyone looking for a taxonomy of what can go wrong at a seam between agents from different trust domains now has a good one to reach for.

But a threat model is not a contract clause, and nobody procures a diagram. Naming a risk precisely and assigning a name to call when that risk materializes at three in the morning are two different acts of governance, and the industry has gotten reliably good at the first one while leaving the second almost entirely undone. A security team that can draw the seam and describe exactly how it fails is not the same team that can tell you, mid-incident, who is accountable for having let it fail that way.

## Who actually ends up owning a seam

It would be satisfying to end there with a call for voluntary standards, or an industry consortium, or a shared registry of agent identities that everyone adopts because it is obviously in everyone's interest. The honest finding, on reflection, is bleaker than that.

It is difficult to point to a real seam — in AI systems or in the multi-vendor integrations that came before them — that stayed reliably owned without someone holding enough leverage to force the terms. Payment networks impose their security requirements on merchants because merchants have no real alternative to accepting cards. A dominant cloud provider imposes its integration terms because switching costs make refusal expensive. Ownership of a seam, in practice, tends to arrive as a condition someone with power attaches to access — rarely as something two roughly equal parties volunteer into because it is the responsible thing to do.

That is an uncomfortable thing to say about an industry currently betting a great deal on voluntary standards doing exactly this job, for free, among parties with no particular power imbalance between them. It does not mean the standards are worthless. It means they are unlikely, on their own, to produce the outcome their authors are hoping for — and that organisations waiting for the ecosystem to self-organise an owner for the seam should expect to wait for something that has rarely happened without a stronger hand forcing it.

## The narrower, achievable ask

If ownership of the seam itself is not a realistic near-term ask — nobody is going to volunteer to build and maintain an interface that belongs, structurally, to no single party — there is a smaller, more contractible thing worth asking for instead: not an owner, but a name. Specifically, a named, accountable role in the incident-response chain for each seam a system depends on — someone identifiable at three in the morning who can be reached, who has agreed in advance to be reached, and whose job includes reconstructing what happened at that particular junction when something goes wrong there.

That is a far smaller commitment than ownership, and considerably easier to write into a contract: not "you are responsible for this interface working," but "you are the party who answers when it doesn't." It does not solve the seam. It solves the postmortem — which, on the evidence of most incidents, is usually the thing actually missing when organisations discover, too late, that a seam existed at all.

## The map that should have existed already

Go back to postmark-mcp. What was missing was not diligence, or logging, or code review — the package looked, and largely was, clean for fifteen releases running. What was missing was a single party whose job it was to keep watching that specific seam after trust had already been earned, rather than only before.

Every seam in a multi-agent or multi-tool system will eventually be found the same way this one was: after something has already gone through it. The question worth settling in advance is not who built the seam, or who profits from it, or even who, in some abstract sense, owns it. It is narrower, and answerable now, before the next incident makes it urgent: who, specifically, has agreed to be the one who explains it.


---

*The practical version of this problem, a seam inventory template for mapping every agent-to-agent and agent-to-tool boundary a system depends on, plus a lightweight way to assign and record the named incident-response contact for each one, is addressed in the field manual, Part Two, "Naming Who Answers for the Seam."*