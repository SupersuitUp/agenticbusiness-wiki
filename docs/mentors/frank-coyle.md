---
title: "Frank Coyle"
slug: /mentors/frank-coyle
description: "Computer-science educator at UC Berkeley with 35 years in the field and an early career in neuroscience. Worked in expert systems during the 1980s boom and watched them collapse. Source on reusing published vocabularies rather than modeling a domain from scratch."
---

# Frank Coyle

*Computer-science educator at UC Berkeley with 35 years in the field and an early career in neuroscience. Worked in expert systems during the 1980s boom and watched them collapse. Source on reusing published vocabularies rather than modeling a domain from scratch.*

---

## Background

Coyle teaches computer science at UC Berkeley and has worked in the field for roughly 35 years. His early career was in neuroscience, which he describes as becoming relevant again now that agentic AI is pulling cognitive science back into the conversation.

The part of his history that earns him a page here is the middle stretch. He worked in expert systems during the 1980s commercial boom, when hand-authored rule engines were expected to be the whole of AI, companies raised money on that expectation, and national programs were built around it. He watched the approach fail on scale and the field fall into the AI winter that followed.

That gives him an unusual vantage point in a field where most commentary starts in 2023. He is not nostalgic about the symbolic era. His read is that the rule-based half failed on the cost of authoring rather than on correctness, that the model has now solved the authoring problem, and that the useful engineering sits at the join between the two halves.

## Why he is on this wiki

Most advice on making a business readable to agents is about the effort itself: write down your objects, define your relationships, keep the model current. Coyle contributes the part that decides whether that effort pays, which is where the hours go.

His claim is that fifteen to twenty years of published vocabulary already covers the generic layer of nearly every business, that reusing it is a competitive advantage rather than a shortcut, and that a team writing its domain model from a blank file is spending scarce effort producing something a competitor can download. For an operator budgeting a modeling project, that reframes the whole exercise.

He teaches rather than sells, so the framings arrive without a product attached.

## Principles contributed to this wiki

- **[Steal the Nouns](/principles/steal-the-nouns)**: most of a domain model is generic and already published as a free standard. Adopt those types as-is, extend where the business is genuinely different, and spend every remaining hour on the part no standard will ever cover.

## How to cite him

Coyle's public teaching is the source: conference talks, course material, and his site at codesupreme.ai. Cite by name, source title, and date. For verbatim quotes, use a blockquote:

> Quote text here.
>
> Frank Coyle, [Source title](URL), Format, YYYY-MM-DD

When the principle is distilled rather than quoted verbatim, note the source at the top of the principle page in the format: "*Distilled from [Frank Coyle](/mentors/frank-coyle), '[Source title](URL)', conference talk, YYYY-MM-DD.*"

## Field Notes

### 2026-07-23, "Why Agentic Systems Need Ontologies" (Conference talk)

A 21-minute talk tracing two lineages that spent decades blocked on scale and have now converged: agents from the 1956 Dartmouth workshop, and formal knowledge representation from Aristotle through Quine to Gruber's 1993 definition. His central reframe is that hallucination is the mechanism of a language model rather than a defect of it, so the engineering move is to surround the probabilistic component with a formal layer that cannot invent anything.

The insight lifted to this wiki is the reuse argument: schema.org, Dublin Core, FOAF, and DBpedia already cover the generic layer, and starting from one of them beats a blank file. He pairs it with a method correction, which is to build the model both top-down (experts enumerating entities) and bottom-up (watching what actually shows up in real customer interactions), since top-down alone is precisely what failed to scale in the expert-systems era.

> "There are existing taxonomies that people have been working on for the last 15 to 20 years. Things like schema.org, which has a whole set of terms and relationships, so you don't have to reinvent the wheel."
>
> Frank Coyle, [Why Agentic Systems Need Ontologies](https://www.youtube.com/watch?v=Sir59K8ZDPU), AI Engineer conference, 2026-07-23

Threads from the talk that landed on sibling wikis rather than here: the neurosymbolic architecture itself, the placement rule for validation in an agent loop ("Pydantic at the door, ontology at the ledger"), and what a formal reasoner catches that a prompt waves through. Those live at [Neurosymbolic AI](https://appliedai.wiki/concepts/neurosymbolic-ai) on the applied-AI craft wiki.

Where the insight landed on this wiki:

- [Steal the Nouns](/principles/steal-the-nouns)

## Further Reading

- [Steal the Nouns](/principles/steal-the-nouns)
- [The Machine-Legible Business](/concepts/the-machine-legible-business): why a business needs a readable domain model in the first place
- [Mentors](/mentors): the other mentors on this wiki
- [Principles](/principles): the load-bearing rules of building an agentic business
