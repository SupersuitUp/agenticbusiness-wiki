---
title: "Steal the Nouns"
slug: /principles/steal-the-nouns
description: "Most of your domain model is generic and already published as a free standard. Adopt those types as-is, and spend every remaining hour of modeling effort on the part no standard will ever cover."
image: "/img/comics/steal-the-nouns.png"
---

# Steal the Nouns

*Most of your domain model is generic and was standardized years ago by someone else. Adopt those types as-is, extend where your business is genuinely different, and spend every remaining hour on the part no standard will ever cover.*

![A warm editorial plate on a wooden workbench. A glowing translucent amber laptop sits open on the left; inside its screen the Chief of Agents, a small rounded figure in a gold peaked cap, lifts a ready-made shape down from a tall shelf of identical stock bowls, blocks, and discs, with a neat stack of the same shapes already gathered at his feet. Outside the laptop, in the real world on the right, a pair of ordinary human hands leans in with a fine engraving tool and cuts notches into one small irregular hand-carved piece unlike anything on the shelf, wood shavings scattered across the bench. No text anywhere in the image.](/img/comics/steal-the-nouns.png)

---

*Distilled from [Frank Coyle](/mentors/frank-coyle), ["Why Agentic Systems Need Ontologies"](https://www.youtube.com/watch?v=Sir59K8ZDPU), conference talk, 2026-07-23.*

## What it is

An allocation rule for the moment a business writes down what its agents are allowed to know and do.

Making a business readable to agents requires a domain model: the canonical list of what exists here and what is true about it. [Ontology as Substrate](https://appliedai.wiki/disciplines/ontology-as-substrate) covers what that model is and how to build one. This principle covers a narrower and more expensive question, which is where the hours go once you start.

The answer almost every team gets wrong: they spend the bulk of the effort on the parts that are identical across every company on earth, and hand-wave the part that actually makes money.

## The three weeks that vanish

Watch a team start. They open with the universal objects, because those feel like the foundation.

Is a person's name one field or three? Is an organization its own type, or a Person with a flag? Is Money a decimal, or an integer of cents plus a currency code? Does an address have a state, a province, or a region? Should Customer and Vendor be separate types when half the list is both?

These are real questions with real answers, and none of the answers are proprietary. Every company has faced them. Several groups solved them in public and published the results. A team that spends three weeks re-deriving them has spent three weeks producing something a competitor can download.

The three weeks are the smaller cost. The real one is that modeling energy is finite and gets spent in order. By the time the team reaches the pricing exceptions, the approval thresholds, the way this business actually decides a deal is closed, everyone is tired and the section gets a paragraph. That section was the entire point.

## What is already published and free

Coyle's version of the point, from someone who watched the first attempt at this collapse in the 1980s:

> "There are existing taxonomies that people have been working on for the last 15 to 20 years. Things like schema.org, which has a whole set of terms and relationships, so you don't have to reinvent the wheel."
>
> Frank Coyle, ["Why Agentic Systems Need Ontologies"](https://www.youtube.com/watch?v=Sir59K8ZDPU), 2026-07-23

Four bodies of work worth knowing by name.

**schema.org** is the default starting point for anything commercial. Built by Google, Microsoft, Yahoo, and Yandex around 2011 so search engines could read structured data off web pages. Hundreds of types and over a thousand properties, covering Person, Organization, Product, Offer, Order, Invoice, Event, Place, PostalAddress, Review, Service, and most of the rest of ordinary commerce.

**Dublin Core** is fifteen elements for describing a document: title, creator, subject, description, publisher, date, format, identifier, language, rights, and a few more. It comes from the library world, it has been stable since the 1990s, and it is what to reach for when the objects are documents rather than transactions.

**FOAF** models people and the links between them. Worth reading for how it handles identity, though it is largely a legacy artifact of the mid-2000s semantic-web era and does not warrant wholesale adoption today.

**DBpedia** is a different kind of thing. It is a knowledge base rather than a vocabulary: millions of real-world entities extracted from Wikipedia infoboxes, with stable identifiers. Useful when you need a canonical record for a country, a public company, or a well-known person, and would rather link to one than maintain your own.

> "This stuff has been out there underlying a lot of what we already do. So take advantage of these things that already exist."
>
> Frank Coyle, ["Why Agentic Systems Need Ontologies"](https://www.youtube.com/watch?v=Sir59K8ZDPU), 2026-07-23

## Extend, do not replace

Take the generic types roughly as-is. Where your domain has something the standard lacks, declare your type as a specialization of theirs with your fields added. Bending the whole business to fit the standard's shape is the opposite error, and it costs just as much.

Your `Engagement` is a schema.org `Service` with four fields nobody else has. Your `Deal` is an `Order` with your stage model bolted on. The standard carries the parts that are the same everywhere and your extension carries the parts that are yours, which means a reader can tell those two apart at a glance. That legibility is worth something on its own.

Then spend everything you saved on the 20% that is genuinely yours. The payoff for taking the generic 80% is the cleared calendar rather than the saved effort itself. It buys a serious job on the part no standard will ever cover, which is the part where the money is.

## The 2026 argument the designers never had

Here is the reason this principle is worth more today than when any of these standards were written, and it is the strongest business case for adopting one.

These vocabularies are marked up across an enormous fraction of the public web. Every model in production has read millions of real examples of a schema.org `Order`, `Offer`, and `Product`, in every messy variation the web contains. It has read zero examples of your internal schema.

So a model is materially better at emitting and parsing a standard-shaped object than a bespoke one. Better extraction from unstructured input, fewer malformed objects coming back, fewer tokens spent explaining what your field names mean, less prompt real estate defending your conventions. **Using a widely known vocabulary means your schema is already in the model's head.**

This is an accuracy-per-dollar argument rather than a philosophical one, and it is measurable on your own data in an afternoon. It is the same reason an agent performs better in a codebase that follows ordinary conventions than in one full of clever private ones. Convention is not aesthetic preference once a model is the primary reader.

## Rent the vocabulary, own the substrate

This sits next to [Own the Substrate](/principles/own-the-substrate) and appears to contradict it. It does not, and the distinction is worth holding precisely.

The substrate is the reasoning surface: weights, system prompts, the runtime. It is where your strategy lives, it is under a vendor's control, and it can change under you without notice. That is why you own it.

A published vocabulary is the opposite kind of dependency. It is a public standard, not a service. Nobody can revoke schema.org, rate-limit it, or silently change what `PostalAddress` means on a Tuesday. It has no runtime and no owner who can hold you hostage. And it gets more valuable the more widely it is used, because interoperability and model familiarity both scale with adoption.

Own the parts that can be taken away from you. Take the parts that cannot.

## Where the standard stops

The failure mode on the other side is treating the standard as more than it is.

schema.org is deliberately permissive. Almost every property is optional, ranges are loose, and a great deal is left open, because it was designed for the open web where partial and inconsistent data is the norm. That design is correct for its purpose and wrong for yours.

It gives you the nouns. It does not give you "an order can be refunded at most once," "a customer and a support rep are never the same entity," or "status is one of exactly these three words." Those are the constraints that stop an agent from doing something expensive, and they are yours to write. [Neurosymbolic AI](https://appliedai.wiki/concepts/neurosymbolic-ai) covers why those constraints have to be formal rules a checker enforces rather than instructions in a prompt.

Borrow the vocabulary, then tighten it hard for your own checks. Steal the nouns, write your own verbs and limits.

## What good looks like

An operator running this principle can:

- Name which standard their domain model started from, and point to the specific types they adopted unchanged
- Show which of their types are extensions of a public type and which are genuinely native to the business
- Say what fraction of the modeling effort went to the proprietary 20%, and defend it as the majority
- Produce the list of business constraints that sit on top of the vocabulary, none of which came from the standard

## Common mistakes

- **Starting the model with Person and Money.** These feel foundational and are entirely commodity. Starting here guarantees the proprietary work gets the tired end of the week.
- **Adopting a standard wholesale and bending the business to fit.** The standard covers the generic layer. Where your business is genuinely different, extend it. A model that cannot express what makes you money is worse than no model.
- **Confusing the vocabulary with the constraints.** A permissive standard will happily accept a second refund on the same order. The nouns come from the standard and the limits come from you.
- **Building a private schema for the sake of differentiation.** The schema is not the moat. What you know about the domain is the moat, and a private vocabulary just makes the model worse at reading it.
- **Skipping the standards review because the domain feels unusual.** Almost every business believes its objects are special. Most of the objects are an Order, a Person, an Invoice, and a Service with different labels on them.

## Further Reading

- [Ontology as Substrate](https://appliedai.wiki/disciplines/ontology-as-substrate): what a domain model is and the craft of building one. This principle is the budgeting decision layered on top.
- [Neurosymbolic AI](https://appliedai.wiki/concepts/neurosymbolic-ai): why the constraints on top of the vocabulary belong in a formal checker rather than a prompt.
- [Ontology-Driven Development](https://appliedai.wiki/disciplines/ontology-driven-development): the engineering methodology that turns the model into software.
- [The Machine-Drivable Business](/concepts/the-machine-drivable-business): why the business needs a readable model at all, and how much of the operating machinery is undifferentiated.
- [Own the Substrate](/principles/own-the-substrate): the dependency you should own, and the contrast that makes this one safe to rent.
- [Frank Coyle](/mentors/frank-coyle): the source of this principle.
