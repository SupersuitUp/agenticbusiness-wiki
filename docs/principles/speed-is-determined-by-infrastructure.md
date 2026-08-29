---
title: "Speed Is Determined by Infrastructure"
slug: /principles/speed-is-determined-by-infrastructure
description: "Speed determines success and failure, and speed is determined by infrastructure: purchasing, hiring, budgeting, reviews. Deep tech companies rarely die of technology. They die of organization."
image: "/img/comics/speed-is-determined-by-infrastructure.webp"
---

# Speed Is Determined by Infrastructure

*Speed determines success and failure, and speed is determined by infrastructure. How the company buys, hires, budgets, and reviews is its operating system, and companies rarely die of technology. They die of organization.*

![Three panels under the title SPEED IS INFRASTRUCTURE. One: a woman leans toward the glowing amber laptop; inside its screen a gleaming brass flywheel machine stands jammed behind tangled gears made of paperwork while three small rounded agents wait idle; caption JAMMED BY PAPERWORK. Two: she sketches and types while the agents inside the screen rebuild the paper gears into one clean harness, a row of simple buttons joined by a single amber line running to the flywheel; caption REBUILD THE BORING SYSTEMS. Three: she sits back with a mug as the flywheel spins fast inside the screen, lapping a smaller dim grey machine far behind on the same track; caption THE WEEKLY LOOP WINS. Footer: SPEED DECIDES WHO WINS. INFRASTRUCTURE DECIDES SPEED.](/img/comics/speed-is-determined-by-infrastructure.webp)

---

*Distilled from [Max Hodak](/mentors/max-hodak), "[What Really Kills Deep Tech Startups?](https://youtu.be/Xc4klGbq8v8)", Y Combinator Startup School talk, 2026.*

## What it is

Hodak opens with the line often attributed to General Omar Bradley: amateurs talk strategy, professionals talk logistics. His company, Science, ships retinal implants that restore vision to blind patients, and his talk about how it moves fast spends almost no time on the technology. It is about purchasing, hiring, budgeting, and performance review, because those unglamorous systems are what set the company's clock speed.

> "Speed determines success and failure, and speed is determined by infrastructure."
>
> — Max Hodak, 2026-08-08

The support systems are not overhead around the real work. They are the operating system the real work runs on:

> "How the company does purchasing and accounting and recruiting and performance reviews and budgeting and safety and quality is the operating system of the company, and that has a huge impact on how far you can take it."
>
> — Max Hodak, 2026-08-08

Science has a reputation for being unusually fast, and Hodak is explicit about the source: "It is mostly not that we are smarter. It is infrastructure like this. That is how speed is built."

## The anatomy of a slow company

Each system looks trivial until the seventeenth employee needs it. Purchasing: hand out credit cards and burn becomes uncontrollable; approve every purchase yourself and you become the bottleneck hassling a highly paid engineer over a $3,000 power supply that the week of delay will cost more than; install off-the-shelf procurement and orders take two weeks while your team clicks through enterprise workflow screens. The actual answer is budgeting: people who understand the resources they own, making trade-offs inside them. Hiring: without a defined process the top of funnel quietly consumes the whole team's time and still produces mediocre outcomes. Performance review: the annual 360 cycle is disruptive, slow, and mostly re-surfaces problems you already knew about and had not acted on.

Every one of those failure modes taxes iteration speed, and iteration speed is the whole game:

> "Rate of iteration separates success from failure. If you can learn one thing every week and there's a competitor that's learning a thing every month, they will never matter."
>
> — Max Hodak, 2026-08-08

Given two approaches to any problem, Hodak weights the one with the shorter iteration cycle even when the other has real redeeming qualities, because the compounding is that dramatic. And the stakes are existential: in his experience deep tech companies rarely fail because the technology does not work. They fail because, at hundreds of people and hundreds of thousands of square feet, nobody built the systems that connect strategy to execution.

## Build the harness, do not buy it

Science runs on Helix, internal software where almost everything the company does is a button somewhere: purchasing, batch records, manufacturing steps, recruiting, reviews. One database linking everything means cost attribution actually works (they know a wafer iteration costs $40,000, so experiments stop being "free"), and it enabled mechanisms no commercial tool offers, like company-wide candidate voting and continuous eigen-review performance scoring, where votes are weighted by the graph of who the well-rated people rate highly.

Hodak's argument for building rather than buying used to be contrarian and is now simply rational: nobody loves their ERP system, and companies that grow up around a harness fit exactly to them (YC's internal software, the manufacturing systems at the big aerospace and automotive innovators) get power that purchased software cannot deliver. Agents changed the economics; vibe-coding a purchasing system is now a reasonable seed-stage decision. The same move makes the company AI-native: gather everything that happens into one place, and the context is ready for agents to use. This is the deep tech articulation of [Own the Substrate](/principles/own-the-substrate), and the harness it produces is what makes a business machine-drivable in the sense of [The Machine-Drivable Business](/concepts/the-machine-drivable-business).

## How to apply it

- **Treat the boring systems as first-class engineering.** Purchasing, hiring, budgeting, and review deserve design effort proportional to how much clock speed they control.
- **Push spending judgment into budgets, not approvals.** The goal is people making trade-offs inside resources they understand, never a founder reviewing power supplies.
- **Measure your learning cadence.** Ask weekly what the company learned this week. If the honest unit is months, the infrastructure is the reason.
- **Put everything in one system agents can read.** Attribution, traceability, and AI-nativeness all fall out of a single connected record of what the company does.

## Further Reading

- [Action Produces Information](/principles/action-produces-information): the companion principle, from the same talk, for when the fast company gets stuck
- [You Cannot Delegate Your Judgment](/principles/you-cannot-delegate-your-judgment): the decision-making load infrastructure cannot carry for you
- [Own the Substrate](/principles/own-the-substrate): the general case for owning the systems you run on
- [The Machine-Drivable Business](/concepts/the-machine-drivable-business): what a company shaped like Helix makes possible
- [The Weekly Scorecard](/principles/the-weekly-scorecard): the EOS-scale version of a continuous signal
- [Max Hodak](/mentors/max-hodak): the mentor who articulated this principle
