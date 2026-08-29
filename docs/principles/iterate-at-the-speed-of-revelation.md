---
title: "Iterate at the Speed of Revelation"
slug: /principles/iterate-at-the-speed-of-revelation
description: "Sit with the customer while they use the product, read what their usage reveals rather than what they report, and ship each fix in the moment that produced it. Observed use arrives faster than most teams are built to act on."
image: "/img/comics/iterate-at-the-speed-of-revelation.webp"
---

# Iterate at the Speed of Revelation

*Sit beside the customer while they are using the product, read what their usage reveals rather than what they report, and ship each fix in the moment that produced it. Observed use arrives faster than most teams are structured to act on, and the structure that can keep up is one or two people.*

![Three panels at one wooden table, the same two people throughout: an operator in a rust-red sweater and a customer in an olive jacket holding his own plain tablet, with her glowing amber laptop open at her side, a small commander in a gold cap and two agents at work inside its screen. One, captioned WATCH THEIR HANDS: he works on his tablet with a stalled expression while she sits turned toward him, hands still, saying nothing. Two, captioned TELL YOUR AGENTS: he is still on his tablet, not looking up, while she gestures toward her own laptop and the agents inside pull apart and rebuild a small panel of shapes. Three, captioned NOW REFRESH: she points at his tablet, he taps it, and his hand moves on freely. He never touches or looks at the glowing laptop in any panel.](/img/comics/iterate-at-the-speed-of-revelation.webp)

---

## The old loop had a hole in the middle

The standard practice for learning what a product should be was to schedule the learning. You booked a research session, ran it, wrote it up, and fed the writeup into a roadmap that would produce a change some months later.

At large companies the practice hardened into a job. Dedicated user researchers would spend a quarter studying a population of users, in genuine depth, and produce a finding. They had no capacity to change the product, and the people who could change the product were not in the room where the finding was made. So the loop had a hole in the middle: the person who saw the truth could not act on it, and the person who could act on it received a summary of a summary, weeks after the moment had cooled.

Every part of that arrangement was rational when a change cost weeks. Batching the learning made sense because acting on it was expensive. Now that a change costs minutes, batching the learning is the expensive part. The research calendar is the bottleneck, and it is a bottleneck that exists for no reason other than habit.

## Observed use is the input, and proximity is what produces it

Rename the thing being harvested and the practice changes. You are not collecting feedback. You are reading usage: watching a real person try to accomplish something real with your product, and seeing in what they do the thing you could not have reasoned your way to. Call what you take away revelation, and keep track of where it came from. It is produced by their behavior, and only rarely by their commentary.

Revelation does not arrive on a schedule and it does not survive transport. It happens at a particular second, on a particular screen, with a particular person's face doing a particular thing. If you are in the room, you see it. If you are reading a report, you get the sentence that survived four rounds of paraphrase.

So the practice is embedding: be physically or virtually present while the customer works, watch them hit the wall, change the product, and hand it back before they have left the wall behind. The strong signal is the wall itself. Where their hand hesitated, which step they did twice, what they abandoned and worked around, how long the screen held them before anything happened.

What they say about the product is a weaker signal than what their hands did with it, and it is weaker in a specific way: people narrate their experience through what they think you want to hear, and they are not reliable narrators of their own confusion. A person can tell you a screen was fine ten seconds after failing at it. The recording of what they actually did carries no such distortion.

So ask, but ask about the wall you just watched rather than about the product in general: did that change unblock you, and does it get you to the next step of what you were doing. That question has an answer within seconds, and the answer either ships or it does not.

## The worked case: twenty versions in one night

The check-in software for a live event went through twenty shipped iterations across a single evening, while the event was happening and people were walking through the door.

The operator stood where the software met the guests. Each version answered something a real person had just done in front of him: a field nobody understood, a step that took one tap too many, a state the flow had not anticipated because no one imagined a hallway that crowded. He changed it, redeployed, and watched the next arrival meet the new version.

Nothing about that evening required a large team, a research plan, or a roadmap. It required proximity, an operator who could ship, and a willingness to treat the twentieth version as the point rather than the first one. What matters is the distance: seeing the problem and shipping the fix sat close enough together that the same person could hold both ends of it.

## Pick the person who is desperate for it

The practice depends entirely on who you embed with, and the selection rule is narrow.

Embed with the customer who was already trying to use your product in its ugliest, most unfinished form. Not the friendly one, not the prestigious logo, not the person who agreed to a call because they are polite. The one who wanted the thing badly enough to fight your prototype for it.

That person gives you their time for a reason that has nothing to do with helping you. Your product is carrying them toward something they actually want, and every fix you ship in front of them moves them further along it. The exchange is honest on both sides: you are getting usage worth watching, and they are getting the only thing that would justify sitting next to a founder all evening, which is progress on their own mission.

The deeper reason to pick this person is that only they generate usage worth reading. A user who does not need what you are building will move through it politely, avoid the hard paths, and produce a clean session that teaches you nothing. A user who needs it will push until something breaks, because the wall is in their way and they want it gone. Their frustration is data you cannot get any other way, and it shows up in their hands before it shows up in their mouth.

## Pick a problem that does not need a mobile app

The loop has a hard dependency most people discover late: your iteration speed is capped by your slowest path to production, and on mobile that path runs through Apple.

A web app can go from observed problem to shipped fix in the length of a pause in conversation. Change it, deploy, tell the person to refresh. A native mobile app cannot do that. Every change goes through a build, a submission, and a review queue owned by someone else, and this practice collapses when the person sitting beside you cannot see the fix until next week. On mobile the twenty-versions-in-one-night evening is structurally unavailable, not merely harder.

So treat the platform as a choice you make in service of the loop. When picking what to work on, favor problems a web app can carry, and be suspicious of an idea whose first version has to be native. The question that matters early is which platform lets you change the product while the customer is still sitting in front of it.

If the problem genuinely demands a native app, know that you are buying the review queue and plan around it: prove the shape on the web first, and port once the shape has stopped moving.

## The team that can run this is very small

Now count the handoffs. Someone must watch the customer use it. Someone must decide what the observed behavior means. Someone must make the change. In the old arrangement those are three people in three functions, and each handoff adds a translation loss plus a scheduling delay, which is exactly why the loop was measured in quarters.

Run all three inside one head and the loop closes in the length of one conversation. The product person is the engineer. The researcher is the person shipping. There is no writeup, because there is no one to write it up for.

This is where the practice turns into a claim about company shape. An agentic business should be very small, and often it should be one person, because the loop that decides whether the product is any good runs fastest when it does not cross a boundary between people. Headcount was how you bought throughput when a human had to do each step. It is now mostly how you buy latency. The solopreneur running this loop against a niche of customers who are desperate for the thing will out-learn a funded team that is still coordinating, and out-learning is the only compounding advantage available at the start.

## What overengineering means now

The failure mode this principle exists to prevent is building past your last revelation.

Overengineering used to mean gold-plating: too many features, too much abstraction, too clever an architecture. The definition has moved. Overengineering now means any work you did beyond the last thing you actually watched a user do, because that work is a bet placed with no information at a moment when information was cheap and available. The more capable your tools, the more of it you can produce, which is why the risk is higher than it was, not lower. Ability to build fast is not the same as license to build far.

The discipline is to keep the built thing tethered to the last observed session, and to go watch another one before extending further. Ship the smallest change that answers what you just saw happen, put it back in front of the person whose usage produced it, and let what they do next pay for the next unit of work.

## Supporting voices

[Christopher Pedregal](/mentors/christopher-pedregal), who runs Granola, arrived at the same practice from inside a venture-backed company and stated the threshold precisely. One person's confusion is enough to act on:

> "You don't need to hear the same thing from 10 people. If I put a prototype in front of you and you say this button's super confusing, and I look at it and I'm like, oh I totally understand why you're confused, I don't need 10 other people to tell me that. I should go and I should change that button immediately, so that next time I show it to somebody I learn what the next problem is. And I think this is something that, especially in big companies, that's unheard of."
>
> — Christopher Pedregal, 2026-01-14

His argument for why a slow loop is worse than no loop is about the operator rather than the customer. The context that produced the decision expires:

> "If it takes a month to get feedback on it, it's almost not worth doing, because the thinking you had when you made the original decisions, you don't even remember."
>
> — Christopher Pedregal, 2026-01-14

He also names the reason overengineering cannot be reasoned away:

> "The right solution is unknowable until you go out and you try it and it gets contact with the world. You can't sit and design the perfect thing. You need to put stuff out there, probe the system, and see how the system probes back."
>
> — Christopher Pedregal, 2026-01-14

His clearest illustration of why watching beats asking is a usability recording he describes: the user fits the square block into the square hole, the designer is delighted, and then the user picks up the circle and pushes it at the square hole too. Nothing in that session had to be said out loud for the product's real problem to be visible.

> "You just see basically completely misunderstanding the product in front of them."
>
> — Christopher Pedregal, 2026-01-14

And he supplies the discipline that keeps embedding from turning into order-taking. Take their context, ignore their requests, and distrust their compliments: "so I categorically ignore all positive things that people say." His rule for a session is to never ask someone whether they would use a thing, or to ask and then discard the answer, and to probe any stated intention from the negative side instead. Read the behavior, weigh the commentary, and let your own judgment decide what gets built.

## Further Reading

- [Go and See, Two Eyes Two Ears](/principles/go-and-see)
- [Get Pathologically Close to the Customer](/principles/pathologically-close-to-the-customer)
- [Action Produces Information](/principles/action-produces-information)
- [Continually Improving Products](/concepts/continually-improving-products)
- [Minimum Proofpoint](/principles/minimum-proofpoint)
- [A Bias for Iteration Is the Price of Admission Now](https://appliedai.wiki/perspectives/a-bias-for-iteration-is-the-price-of-admission-now) on appliedai.wiki: why comfort with rapid iteration is now the entry requirement rather than an edge.
- [Revelation Is the Bottleneck](https://hyperagency.wiki/concepts/revelation-is-the-bottleneck) on hyperagency.wiki: the philosophy underneath this practice, and why a fast builder without proximity elaborates instead of iterating.
