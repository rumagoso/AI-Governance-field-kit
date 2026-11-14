# Seamless
### AI Governance for the Parts Nobody Owns

*A book by Rui Soares. Out in February 2027. Self-published, built in public, live.*

---

## What this is

Eighteen essays about where AI governance actually fails: not in any single control, but in the space between two things. Two regulatory clocks. Two agents. Two people who each assumed the other was watching. Most of the essays are paired with a practical companion in Part Two (a record, a worksheet, an inventory, something to actually fill in), seventeen chapters in all.

This repository is the book, and it stays live after publication. Regulations get amended. Enforcement actions happen. Templates get better the more people actually use them. A printed copy is a snapshot; this repo is the current version.

## How the essays are arranged

Not chronologically and not by length, but by what each step asks.

| Essays | What they ask |
|---|---|
| 1 | **Opening.** A system ending, and what it leaves behind. |
| 2–5 | **The human family.** Was a person present, competent, and did they understand what they agreed to? |
| 6–10 | **The gap between two things.** Clocks, boards, seams, hands, screens. |
| 11–13 | **The ground shifted and no bell rang.** Nothing failed; everything changed. |
| 14–16 | **Coverage and evidence.** Do you know what you have, and is it still true? |
| 17 | **Frontier.** A live incident, held open on purpose. Not a family. Still moving as the book goes to press. |
| 18 | **Capstone.** Every control passed and something still went wrong. |

The [Rosetta Stone](docs/rosetta-stone.md) indexes all eighteen by symptom ("an incident just happened and I don't know which deadline governs"), by regulation, and by family.

## Structure

```
part-one/     The eighteen essays, in reading order, each with a Part Two cross-reference
part-two/     The field manual: seventeen practical chapters, plus templates
assets/       Cover art and the Rosetta Stone visual
docs/         Rosetta Stone, priority guide, first 30 days, glossary, reading list
```

Read Part One in order, top to bottom. Part Two chapters can be used independently: pull whichever one matches a problem you actually have. Essay 15 has no separate chapter; it carries its own AI Inventory Template.

If you can only do some of it, start with [`docs/priority-guide.md`](docs/priority-guide.md), or follow [`docs/first-30-days.md`](docs/first-30-days.md).

## Using the Part Two templates

Every chapter in Part Two follows the same shape: a worked example first, so you can see it filled in before you fill in your own, then the fields, then a short note on who should actually be doing the filling in and how it tends to go wrong. None of them are meant to be exhaustive. Adopt one as written, use it on a real system, and let it tell you what it's missing for your own environment.

The one rule worth keeping across all of them: any field that records a status gets a named person attached to it too.

Blank copies of every template are in [`part-two/templates/blank-templates.md`](part-two/templates/blank-templates.md).

## Status

Actively being written. Essay and chapter content is drafted; citations are checked against primary sources as of the date each essay was written (see `part-one/00-ai-use-disclosure.md` for how that is maintained). Four essays carry an honesty note: the evidence for their anchor is exactly as strong as the note says, no stronger. Essay 17 is deliberately left open because the incident it describes is still unfolding. New entries are planned to stop around November 2026 so the book can go to press.

Some of the essays are published on LinkedIn ahead of the book.

## Contributing

Not yet formally open. If you find an error, an outdated citation, or a way one of the Part Two templates could be better after using it for real, open an issue. A more structured contribution process may follow after initial publication.

## Licence

**Part One (the essays):** © Rui Soares. All rights reserved.

**Part Two (templates and worksheets):** Licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Use, adapt, and redistribute freely, including commercially, provided you credit the source and release adapted versions under the same licence. This keeps improvements flowing back into the same open pool rather than disappearing behind someone else's closed terms.
