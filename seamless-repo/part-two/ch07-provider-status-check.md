# Chapter 9: Naming the Moment You Became the Provider

*Companion to "Congratulations, You're a Provider Now"*

The essay's pattern isn't a single incident, it's a gap that opens by default: nobody at a small company is asked, at the point of a product decision, whether that decision just changed their legal classification under the AI Act. This chapter is the question, made unavoidable, at the one point it actually needs to be asked, before launch.

## Worked example

**Change:** Fine-tuning a licensed foundation model on customer support tickets, shipping as "Smart Reply" under the company's own brand
**Own branding applied?** Yes — sold under the company's product name, no reference to the underlying model
**Substantial modification?** Yes — fine-tuned on proprietary data, materially changes output behaviour from the base model
**New intended purpose?** No — still general customer support, not repurposed into a high-risk use case
**Resulting classification:** Provider (two of three triggers met is sufficient), flagged before launch
**Decision made by:** Head of Product, with 20-minute legal consult, 2 September 2026

Twenty minutes, three questions, one classification decided before the feature shipped rather than discovered after a client's compliance team asked. That's the entire value of this chapter.

## The trigger-test

Run before shipping any product built on a third-party AI model.

**Own branding applied?**
Does the system carry your name, trademark, or product identity rather than the original vendor's? Yes counts as a trigger regardless of how minor the rebranding feels.

**Substantial modification?**
Fine-tuning, retraining, or materially changing the system's behaviour from what the vendor shipped. A thin prompt wrapper is not this. Training on your own data usually is.

**New intended purpose?**
Does this deployment point the system at a use case, especially a high-risk one, different from what the original system was built and assessed for?

**Resulting classification**
Any single trigger is worth flagging for review; two or more is a strong signal the classification has shifted from deployer to provider, and the obligations that come with it need addressing before, not after, launch.

**Decision made by**
Named person, with a date. A trigger-test nobody signed off on is just a document that existed, not a decision that was made.

## Who fills this in, and when

Whoever owns the product decision, before the feature ships, ideally as a standing step in the same review that already covers security or data protection, not a separate process nobody remembers to run. The essay's whole point is that this question currently isn't anyone's job by default; this chapter only works if it gets attached to a step that already exists.

The failure mode specific to this chapter: running the test once, at initial launch, and never again as the product evolves. A feature that started as a thin wrapper and quietly became a fine-tuned, rebranded, repurposed system six iterations later needs this test rerun at the point of substantial change, not just at the point of first ship.
