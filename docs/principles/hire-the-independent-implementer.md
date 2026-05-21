---
title: "Hire the Independent Implementer"
slug: /principles/hire-the-independent-implementer
description: "If the people building your AI stack make more money when you commit to one foundation-model vendor, they cannot be trusted with the architecture call. Hire the implementer whose paycheck is the same no matter which model you pick."
---

# Hire the Independent Implementer

*If the people building your AI stack make more money when you commit to one foundation-model vendor, they cannot be trusted with the architecture call. Hire the implementer whose paycheck is the same no matter which model you pick.*

![Four-panel comic in bold neo-comic action-zine style with high-tech power-armor visual DNA on a cream paper background. Title bar at top in chunky inked caps reads HIRE THE INDEPENDENT IMPLEMENTER. 1. THE BADGE TRAP: a captive consultant in a glossy charcoal suit and gold tie holds up a gold-ribbon partner badge reading PREMIER PARTNER · ONE VENDOR while a thick envelope labeled REBATE · CHANNEL ECONOMICS flows from a placard reading VENDOR A directly into his back pocket. The principal in his matte-navy Supersuit with vivid orange seam accents, helmet off, is being walked through a doorway labeled STACK · VENDOR-A ONLY. Speech bubble from consultant: Trust us. Best-in-class. Caption: The captive implementer's recommendation is sincere. It is also paid for. 2. THE LANE BREAKS: the principal at a workbench surveying a tall fragile teetering tower of stacked blocks labeled VENDOR-A · ONLY with cracks spider-webbing through it. A red regulatory notice falls from the sky labeled COMPLIANCE NOTICE · VENDOR-A DESIGNATED RISK. A clipboard floating in mid-frame reads RE-PLATFORM BILL · \$2.4M · 9 MONTHS. The same captive consultant lurks in the corner with an oily smile offering a contract scroll labeled MIGRATION SOW. Caption: When the lane breaks, the principal pays the bill twice. 3. THE INDEPENDENT BUILD: inside a high-tech innovator's workshop, an independent implementer (a Latina engineer in a simple workshop jacket with dark goggles up on her forehead, no badges anywhere on her clothing) wires a multi-model router. The router is a glowing cyan hub with four chunky pipes radiating out to placards labeled VENDOR A, VENDOR B, VENDOR C, VENDOR D. An open binder on the bench is labeled EVAL SET · WORKLOAD-FIRST. A wall placard reads NO PARTNER BADGES · PAID IN CASH · NO REBATE. The principal (partially suited, helmet off, no halo yet) is hands-on at the bench beside her pointing at a holographic eval-score readout. Caption: The independent implementer routes by eval, not by allegiance. 4. HYPERCONTEXT LOADED: first-person POV through the principal's armored hero's helmet visor. Translucent inked visor frame creates the panel borders. HUD overlays in cyan and gold read ROUTER · 4 PROVIDERS ACTIVE, SUMMARIZATION → PROVIDER B, REAL-TIME → PROVIDER C, COMPLIANCE WATCH · ALL GREEN, MIGRATION COST · CONFIG-ONLY. An orange-and-navy gauntleted hand reaches into the lower frame pulling a labeled lever marked ROUTE. Arc-reactor cyan glow at the bottom edge of frame. A single unified gold spiral halo hovers at the top of the visor frame. Caption: The hyperagent swaps vendors inside a sprint, because the architecture never assumed one. Footer bar at bottom in chunky inked caps: OWN THE EVAL. OWN THE ARCHITECTURE. OWN THE EXIT.](/img/comics/hire-the-independent-implementer.png)

---

*Distilled from public 2026 evidence: the Anthropic-Accenture $100M channel partnership, the Pentagon's supply-chain-risk designation of Anthropic, the Microsoft-OpenAI exclusivity unwind, and the broader principal-agent structure of every hyperscaler partner program.*

## What it is

Every major foundation-model vendor now runs a partner channel. Anthropic has the Claude Partner Network with an initial $100M commitment, anchored by Accenture, Deloitte, Cognizant, and Infosys. OpenAI runs the Solutions Partner Program. Google, AWS, and Microsoft each run their own. The partner-tier badge on a consultancy's website looks like a credential. It is also a compensation structure.

A consultancy that earns referral fees, training subsidies, co-selling support, and tier-status renewals from one vendor is paid, structurally, to talk you into that vendor's stack. They are not lying when they recommend it. They are doing the job their P&L hired them to do. The recommendation is sincere. It is also conflicted.

The principle: when you are picking who builds your agentic business, separate the architecture decision from the implementation decision. The implementer should be the people who execute the build well, not the people whose business model depends on which model you pick.

## Why it matters now

Three forces converged in 2025 and 2026 to make this principle load-bearing rather than aesthetic.

**The hyperscaler partner programs got big enough to bend incentives.** Anthropic's commitment to train 30,000 Accenture professionals as Claude practitioners is not a developer-education program. It is a distribution strategy. The downstream effect: every Accenture-led enterprise AI engagement now defaults toward Claude-on-Anthropic regardless of whether Claude is the right model for that workload. The same dynamic applies at Deloitte, Cognizant, and Infosys. The same dynamic applies to OpenAI's, Google's, and AWS's partner channels.

**Single-vendor lock-in turned out to be politically fragile.** In March 2026 the U.S. Department of Defense designated Anthropic a supply-chain risk and required all defense vendors and contractors to certify they do not use Anthropic's models in their work with the Pentagon. Anthropic appealed and lost in April. The designation was unprecedented for a U.S. company. Anthropic stays a strong vendor for many workloads. The point is that any agentic business with present or future exposure to the defense ecosystem, or to any enterprise customer with defense exposure, that had been built Claude-only by a Claude-aligned implementer was now structurally compromised by a policy decision it had no role in.

**The platform layer itself is moving.** In April 2026 Microsoft and OpenAI restructured their exclusivity agreement. Microsoft's license to OpenAI is now non-exclusive and OpenAI can serve products across any cloud. The OpenAI-Apple partnership soured and OpenAI is weighing breach-of-contract action. The OpenAI-Nvidia framework died and was replaced by a multi-investor structure that includes Amazon. The vendors themselves are explicitly diversifying, decoupling, and refusing to bet their futures on a single counterparty. The principal who hires a single-vendor-aligned implementer is doing the opposite of what the vendors are doing.

The implication for the principal of an agentic business: the implementer's incentive structure now matters as much as their portfolio.

## How the conflict shows up in practice

The captive implementer does not announce itself. It shows up as a series of small architectural choices that all run downhill.

- The proof-of-concept gets built directly against one vendor's SDK rather than against a thin abstraction layer.
- Evals get framed in terms of one model family rather than the workload's actual quality bar.
- The team's accumulated skill is in one vendor's tooling, so the next problem also gets solved with that vendor.
- The deployment topology assumes one cloud's region and identity model.
- Re-platforming, when the day comes, costs an order of magnitude more than the original build.

None of these are sabotage. Each is the path of least resistance for a team paid by a partner program to specialize in one stack. The principal pays the bill twice: once for the build, and again later for the migration.

## What good looks like

The independent implementer has a few visible signals.

**No partner-tier badge from any foundation-model vendor.** Or, if they hold partner badges, they hold three or more and can show client work split across all of them. Diversified badges cancel out the bias the way diversified holdings cancel out single-stock risk.

**The architecture is multi-model from day one.** The application layer talks to a thin model-router or gateway. The router knows about four or more model providers. Swapping a provider takes a config change and an eval re-run, not a rewrite.

**Evals come before model selection.** The implementer insists on building a real eval set for the workload before recommending any model. The recommendation falls out of the eval, not out of the implementer's specialty.

**The implementer will name a counter-vendor for the workload.** Ask which model they would not pick for this job and why. An independent implementer answers cleanly. A captive one deflects.

**Data and prompts are portable.** Conversation history, embeddings, fine-tuning data, system prompts, and tool definitions live in a format and a storage system you control. Migrating between providers does not require excavating proprietary formats.

**Compensation is paid by you, in cash, with no rebate flowing back from any vendor.** If the implementer is taking partner-program economics on the side of your engagement, those economics belong on the table during the contract conversation. Many independent implementers refuse partner-program participation explicitly to avoid the conflict. That refusal is a feature.

## How to interview for it

Four questions surface a captive implementer in under ten minutes.

1. *Which foundation-model partner programs are you part of, at what tier, and what does that tier pay you?*
2. *Walk me through the last engagement where you recommended a model you do not specialize in. Why did you make that call?*
3. *If we hired you and a new model from a different provider became measurably better on our workload six months in, what does your process look like for switching us over? What does it cost us?*
4. *What does your architecture look like for a workload where we need to be able to swap the model in production within a week?*

The captive implementer answers question one with reluctance and questions two through four with evasion. The independent implementer answers all four briskly because they have already been asked.

## Common mistakes

- **Confusing the partner-tier badge with quality.** The badge proves the implementer can build on that vendor. It says nothing about whether that vendor is right for your workload.
- **Letting the implementer run the eval.** A captive implementer who designs the eval will design an eval their preferred model wins. The principal owns the eval set. The implementer executes against it.
- **Hiring the implementer who already trained you up on their preferred vendor.** Training programs from a captive implementer are recruiting funnels for the vendor they are aligned with. By the time you are picking the production stack, your team is fluent in one vocabulary and intimidated by the others.
- **Treating "we are model-agnostic" in marketing copy as proof.** Every implementer's marketing copy claims model-agnosticism. Verify with the four-question interview and with a portfolio split across vendors.
- **Picking the wrong moment to ask.** Once the engagement is signed and the team is staffed against one vendor's stack, the architectural die is cast. The independent-implementer question has to be answered before the SOW.

## Worked examples

A specialty-finance operator hires a Big-Four AI practice that holds Premier-tier status in one foundation-model vendor's program. The deal is signed. The intake interview is run by a partner whose bonus is partially tied to certified consultants billing on that vendor's stack. The reference architecture comes back model-coupled. Two years in, the operator's regulators add a guidance note constraining which vendors are acceptable for credit-decision models. The operator is forced into a nine-month re-platforming engagement, billed by the same firm that built the original.

A media holdco hires a small independent shop that runs every project through a model-router with five providers wired in and refuses to participate in any single vendor's partner program by policy. Two years in, the holdco's workloads end up split: long-context summarization on one provider, multimodal on a second, low-latency real-time on a third. When one provider raises prices, the workload shifts. When a regulator names a problem vendor, the affected workload migrates inside a sprint. The holdco never pays a re-platforming bill because the architecture never assumed a single platform.

The two outcomes are not driven by talent. They are driven by who was paid by whom.

## Further Reading

- [Missionary and Mercenary](/principles/missionary-and-mercenary): the integration of caring about the work with running the business well, which is exactly what is missing in a captive implementer
- [Leverage and Chokepoints](/principles/leverage-and-chokepoints): the structural reason a single-vendor architecture is itself a chokepoint, against you
- [Protect the Mission Vehicle](/principles/protect-the-mission-vehicle): the mission-vehicle frame for why your AI architecture has to be defended from outside capture
- [appliedai.wiki](https://appliedai.wiki): the implementer-facing wiki, for principals who want to know what good implementation craft looks like before they hire for it
