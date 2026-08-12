# Every Hand That Touched It

*A regulator in Beijing fined three platforms not for generating unlabelled content, but for losing the label somewhere between generation and a user's screen, the part of the chain nobody in Brussels has yet been asked to own.*

In April 2026 China's internet regulator penalised three platforms, CapCut, Maoxiang, and Dreamina AI, for failing to properly label AI-generated content. None of the three had been accused of hiding what their tools produced. The generation step was compliant. Somewhere between the image leaving the model and reaching a user's screen, the label meant to travel with it did not survive the trip.

This is a smaller story than it sounds, and a more useful one. China's AI content-labelling regime, mandatory since September 2025, does not ask a service to mark its output once and be done with it. It asks every party that subsequently touches the content, the platform that hosts it, the app that distributes it, the service that re-exports it, to check the label is still there and reattach it if it isn't. The CapCut case was not a story about deception. It was a story about a label that had to survive several hops through ordinary, unremarkable technical processes, and didn't.

## A label built to be lost

The mechanism repays study before judgment. China's rules specify two kinds of label: an explicit one, visible to a viewer, typically a watermark or on-screen text reading "AI-generated"; and an implicit one, embedded in file metadata, readable by machines further down the chain. Both are fragile in well-understood ways. A screenshot strips a watermark. A format conversion strips metadata. Re-exporting through editing software strips both. None of this requires anyone to be trying to cheat the rule. It is simply what happens to files as they move.

Regulators evidently knew this when they wrote the law, which is presumably why the obligation does not end at the point of generation. Platforms are required to check incoming content for labels and, where metadata survives but the visible marker has been stripped, to reconstruct and reapply it before the content reaches a user. The law is not naive about how fragile its own labels are. It is built around that fragility. Responsibility does not sit with whoever made the content. It travels with the content, and reattaches at every hand that receives it.

## A different assumption, where the sun rises first

On the other side of the world, where the working day begins several hours earlier, the European Union's comparable rule reads differently, not because Brussels disagreed about the risk, but because it was solving a narrower problem. Under Article 50 of the AI Act, providers of generative systems must ensure their output is marked as artificial. Deployers of certain systems, deepfakes chief among them, must disclose that fact to the people encountering the content. Both are real duties. Neither extends downstream. Once the label has been correctly attached at the point of generation or deployment, the legal obligation has, on its face, been discharged. What happens to that label afterwards, whether it survives a re-upload, a compression pass, a screenshot shared three platforms later, sits outside the rule's reach.

Set the two regimes side by side and the difference is not one of seriousness. It is one of geography, in the sense that matters to lawyers: where liability is deemed to live. China's rule assumes the label will be lost in transit and builds a chain of custody to catch the loss at every link. Europe's rule assumes a correctly attached label is the provider's problem to have solved, and stops there.

## The question nobody has had to answer yet

Nothing about the European approach is obviously wrong. A single point of accountability is simpler to audit, simpler to enforce, and does not require every platform in a distribution chain to build label-verification into its own pipeline. But it has not yet been tested against what China's regulator demonstrated in public in April: that the assumption underneath a single-point rule, that a correctly attached label stays attached, does not reliably hold. CapCut's watermark almost certainly satisfied an Article 50-equivalent test at the moment of generation. It failed China's rule anyway, because by the time the content reached its audience the label was gone, and nobody downstream had been made responsible for noticing.

None of this argues that Europe should import China's chain-of-custody model wholesale; the compliance burden it places on every platform in a pipeline is real, and proportionate only if label loss is common enough to justify it. But the question the European regime has not yet had to answer is worth asking plainly: when a label is, by design, as fragile as a watermark or a metadata field, is attaching it once actually equivalent to disclosure, or is it equivalent to disclosure only until the first re-upload, the first screenshot, the first ordinary thing an ordinary user does with a file?

Nobody has had to ask that question in Brussels. Beijing's regulator asked it in April, and the answer it got back had three names on it.
