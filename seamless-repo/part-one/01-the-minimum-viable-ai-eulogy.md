# The Minimum Viable [AI] Eulogy

*Every AI system gets a launch ritual. Almost none get an exit plan — and the gap between the two is where governance debt quietly accumulates.*

Every AI governance framework has a baptism. A DPIA before launch. An AI Impact Assessment before deployment. An inventory entry the day the system goes live. Somebody blesses the thing into existence with paperwork.

None of them have a funeral.

Onboarding rituals, stacked three deep. Retirement gets a sentence, if it gets anything.

No one writes the eulogy.

## Baptised, Never Buried

An AI system goes live under review. Gets fine-tuned twice. Absorbs eighteen months of decisions nobody wrote down. Then quietly stops being used.

It leaves the same residue either way. Training data. Logs. Fine-tune artifacts. A dozen downstream workflows that assumed it would always answer.

Nothing forces you to deal with any of it. An unused AI system doesn't announce itself. It doesn't crash. Doesn't page anyone at 3am. It sits. Technically functional. Gathering the kind of debt that only surfaces when someone finally asks: is this thing still authorised to touch anything?

By then it's not a question. It's an audit finding.

No one writes the eulogy.

## The Exit Interview for a Machine

Go looking for the moment decommissioning actually happens — not should happen, does happen — and you'll find it's not a governance decision.

It's an invoice.

At least in the shops I've worked in. I suspect that's not rare. Nothing retires a system faster than someone in finance asking what a line item is for. Not a security review. Not a policy trigger. Not an architecture board deciding a model has drifted past use. The bill.

A system that still works has no natural enemy except its cost.

So the real gate is procurement, wearing governance's clothes. Fine. Weld the checklist to it, then — not to the gates that exist on paper and wait for someone to remember them:

- **Supplier offboarding.** Usually about data return. Rarely about the fingerprints a model leaves behind in your own systems.
- **New-supplier handoff.** Documents that the replacement works. Almost never documents what the old one knew that the new one doesn't — the near-misses, the edge cases quietly patched around, the scar tissue that made it trustworthy by the end.
- **Change Control.** A decommission is a change. If it doesn't go through the board that approved the last update, it isn't a decision. It's attrition.

Three gates. None fire on their own.

The invoice does.

## Keep or Delete: The Argument You're Not Allowed to Win

GDPR says delete what you no longer need.

A legal hold says keep it — because "no longer need" is doing a lot of work in a sentence written before anyone knew if there'd be a dispute.

The AI Act's logging floor — six months, for high-risk systems — isn't an answer either. It's a floor. Your exposure might run years past it. Or your obligations might demand you clear it sooner.

There is no formula. There's a decision, made by someone with the authority to make it, written down at the moment of retirement — not reconstructed later, under pressure, by whoever's on call.

Pick the wrong side and you have a problem. Pick no side and you have a landmine with a very long fuse.

No one writes the eulogy. Someone still has to sign the death certificate.

## The Minimum Viable Eulogy

Five questions. One shot, before the system slides into the "nobody remembers what this was" pile.

1. **What do we keep, and for how long?** State it against both the AI Act floor and your actual liability window. If they conflict with a deletion obligation, name the conflict. Don't quietly pick one.
2. **What breaks downstream?** Map what consumed this system's output — workflows, other automations, humans who trusted its answers — before you pull it. Not three weeks after something goes quiet.
3. **What does the successor need to know?** Hand over the near-misses with the spec. A clean handoff resets the clock to zero. A real one carries the scar tissue forward.
4. **Who tells the people who relied on it?** Not the dashboard users. The humans whose decisions ran through this system without them knowing it was there.
5. **Is it off the inventory?** Not eventually. Now, in the same motion that retired it. Otherwise the inventory doesn't shrink when things die — it fills with phantoms instead of gaps. Different failure. Same rot.

None of this is technically hard.

It's just invisible, until an invoice makes it visible.

Every system you deploy will stop being useful. Some day, whether or not anyone notices in time. Ending it well is one more part of the system nobody was ever assigned to own.

No one writes the eulogy.

Maybe someone should.

---

*The practical version of this problem — a working decommissioning checklist, retention-conflict resolution steps, and an inventory offboarding template — is addressed in the field manual, Part Two, "Retiring a System Without Losing the Argument."*