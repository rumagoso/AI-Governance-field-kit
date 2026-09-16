# Chapter 9: Naming the Moment You Became the Provider

*Companion to "Congratulations, You're a Provider Now"*

The essay's pattern isn't a single incident, it's a gap that opens by default: nobody at a small company is asked, at the point of a product decision, whether that decision just changed their legal classification under the AI Act. This chapter is the question, made unavoidable, at the one point it actually needs to be asked, before launch.

## Worked example

**Change:** Bruno fine-tuning a licensed foundation model on the bank client's product documentation and past support transcripts, shipping the chatbot under the bank's own brand on their website
**Own branding applied?** Yes — the chatbot appears as the bank's own assistant, no reference anywhere to the underlying model
**Substantial modification?** Yes — fine-tuned on the bank's proprietary data, materially changes output behaviour from the base model
**New intended purpose?** Possibly — the chatbot has started fielding questions that edge toward product eligibility, closer to a lending-adjacent use case than the general customer support it was built for
**Resulting classification:** Provider, likely, and the "possibly" on intended purpose is exactly the kind of ambiguity that needed a real answer rather than an assumption; flagged during this exercise, eighteen months after the chatbot had already shipped
**Decision made by:** Nobody, until now. Bruno built it, the bank approved the branding, and no one at either company had asked the classification question before this record forced it

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
