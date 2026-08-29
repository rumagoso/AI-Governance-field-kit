# Chapter 1: Retiring a System Without Losing the Argument

*Companion to "The Minimum Viable AI Eulogy"*

The essay made the case that decommissioning is where AI governance usually stops paying attention, not because anyone decided it didn't matter, but because nothing forces the question. A contract lapses, a vendor stops billing, and the system quietly stops being anyone's problem before it's stopped being anyone's risk.

The fix is not a longer policy. It's a form that cannot be marked complete with blanks in it.

## Worked example

**System:** Invoice-matching model (INV-AI-014), retired 12 Jan 2027
**Trigger:** Vendor contract lapsed, not renewed — 12 Jan 2027
**Data disposition:** Training data deleted, decision logs migrated to cold storage — confirmed by M. Duarte, Data Protection
**Downstream dependents notified:** Finance Ops (14 Jan), Procurement (14 Jan), external auditor on record (16 Jan)
**Inventory removal:** Confirmed off active register 20 Jan 2027
**Open retention conflicts:** One — seven-year statutory retention on decision logs outstrips the vendor's data-deletion clause; being resolved by Legal, target 28 Feb 2027

Six lines, five minutes to fill honestly, and it already tells you more than most decommissions ever get documented: who confirmed what, who still owes an answer, and by when.

## The Decommissioning Record

Fill one out per system, at the point a decommission decision is made, not after.

**System name / inventory ID**
The entry this record closes out. If the system isn't on the inventory, that's not this chapter's problem to solve, see Chapter 7.

**Decommission trigger**
Contract lapse, replacement, risk finding, business decision, other, dated. Write the real reason, not the official one, if they differ. "Vendor stopped invoicing us" is a valid trigger. It's also worth noticing if it's the *only* kind of trigger your organisation has ever recorded.

**Data disposition**
Kept, deleted, or migrated, and to where if migrated. This field has an owner, not just a status. "Deleted" with no named person who confirmed it is a claim, not a record.

**Downstream dependents notified**
Every person or system whose decisions ran through this system's output, listed, with a notification date next to each name. If you don't know who's downstream, that's the finding, write "unknown, investigating" rather than leaving it blank.

**Inventory removal**
The date the entry was actually taken off the active register, confirmed, not the date someone said they'd get to it.

**Open retention conflicts**
Anything still unresolved at the point of closure, who's resolving it, and by when. It is normal for this field to be non-empty. It is not normal for it to be silently dropped from the record because the rest of the form got finished.

## Who fills this in, and when

The record is filled by whoever is actually making the decommission decision, at the point they make it, not reconstructed afterward by whoever ends up doing the audit prep. A record built from memory three weeks after the fact isn't a record. It's a summary, and summaries smooth over exactly the gaps this form exists to catch.

Two ways this quietly fails without anyone intending it to:

**Filled by one person, confirmed by no one.** If the same person who decided to decommission the system is also the only name that appears anywhere on the form, the record documents a decision, not an audit of it. The named-person fields work because they're a commitment from someone who can be asked, later, "did you actually check this." A form where every name is the same name hasn't been checked by anyone but its author.

**Filled to close the ticket, not to be true.** The fastest way to complete this record is to write "notified" and "confirmed" everywhere and move on. Nothing in the form's structure stops that. What stops it is treating an honestly incomplete record, "unknown, investigating," a blank retention-conflict owner, a downstream dependent nobody's reached yet, as an acceptable outcome, and a suspiciously tidy one as the thing worth a second look.
