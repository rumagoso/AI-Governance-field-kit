# Congratulations, You're a Provider Now

*A composite of a pattern lawyers report seeing repeatedly: a small company fine-tunes and rebrands a foundation model, and under the AI Act may have just become a provider, without anyone noticing the moment it happened.*

A small software company licenses a foundation model through an API, fine-tunes it on its own customer data, wraps it in its own product name, and sells it as a feature of their platform. Nobody in the company thinks of this as becoming an AI provider. As far as anyone there is concerned, they bought a tool and built something on top of it, the way they'd build on any cloud service. Under the AI Act, they may have just done something considerably larger than that, and the moment it happened is not marked anywhere on their calendar.

## The line nobody drew

Article 25 sets out the conditions under which a deployer, an organisation merely using someone else's AI system, becomes a provider, the party carrying the Act's full weight: conformity assessment, technical documentation, post-market monitoring, registration in the EU database if the system is high-risk. The triggers are specific: putting your own name or trademark on the system, making a substantial modification to it, or changing its intended purpose in a way that turns a general-purpose model into a high-risk application. Fine-tuning on your own data, rebranding it as your own product, and pointing it at a new use case checks more than one of those boxes at once, and it is precisely what a small SaaS company building "AI-powered" features is structurally likely to do.

None of this requires bad intent, or even carelessness in any conventional sense. It requires only that nobody with legal or compliance visibility was in the room when the product decision was made, which, at companies too small to have a dedicated AI governance function, is closer to the default than the exception. The original model vendor's terms of service almost always place the compliance burden downstream, on whoever deploys the model, without necessarily making clear that "deploying" and "becoming the provider" are two different legal positions with two very different obligation sets.

## Why the gap is structural, not careless

This is not a story about one company's oversight. It is a story about where the AI Act places its tripwire, at the point of technical modification, and where a typical SME's decision-making actually happens, in a product or engineering conversation with no legal review attached, because reviewing every fine-tuning decision for regulatory reclassification is not yet a habit anyone has built. Large enterprises with dedicated AI governance teams catch this at the design stage, because someone's job is to ask the question. Smaller companies, that this book's readers are more likely to be, usually don't have that role yet, and the Act does not pause its triggers to wait for one to exist.

## The narrower ask

The honest response here is not "get a lawyer to review every model integration," which is correct but unhelpful advice for a ten-person company. It is a single, specific question, added to whatever product-decision checklist already exists: does this change put our name on the system, materially modify its behaviour, or point it at a new purpose? If yes to any of the three, the classification question needs an answer before launch, not after a client, or a regulator, asks first.

Nobody currently owns the moment a deployer quietly becomes a provider. Until an enforcement case draws that line in public, the honest position is that it belongs to whoever asks the question first, and right now, for most companies this size, nobody has been assigned to ask it at all.

---

*The practical version of this problem, a short trigger-test to run before shipping any product change built on a third-party AI model, is addressed in the field manual, Part Two, "Naming the Moment You Became the Provider," the earliest and least visible part nobody owns, since it happens before anyone's even looking for it.*
