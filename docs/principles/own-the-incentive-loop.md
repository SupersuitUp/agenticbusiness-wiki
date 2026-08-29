---
title: "Own the Incentive Loop"
slug: /principles/own-the-incentive-loop
description: "An incentive loop pays people in product for a verifiable public action. Renting one costs you the customer graph. The API is cheap now and the software is a day of building, so build it."
image: "/img/comics/own-the-incentive-loop.webp"
---

# Own the Incentive Loop

*Rewarding people for spreading your launch used to mean renting a quest platform that took your customer graph as the price of admission. It does not anymore. You own the account, so you can see the follow and the retweet yourself.*

![Three panels in one warm room, the same woman in a rust cardigan at her desk beside a glowing amber laptop. One, THE PLATFORM KEEPS THE LIST: inside the laptop a queue of people hand their cards to a clerk in a gold cap who files every card into a cabinet behind him and slides a single thin slip out to her; the shelf beside her desk is empty. Two, YOUR PAGE, YOUR LIST: the counter and cabinet are gone, the same gold-capped agent ticks three tall checkboxes in turn, and each person's card travels out of the screen and stacks up on her own desk. Three, CONVICTION CARRIES IT FURTHER: she holds up a card marked with one bold ink stroke, and inside the laptop a small ring of people holding coupons passes that same mark outward to a much larger crowd beyond them who hold no coupons and carry it on. Footer: BUILD THE LOOP. KEEP THE PEOPLE.](/img/comics/own-the-incentive-loop.webp)

---

*Distilled from operating experience running incentive campaigns on GUILD.xyz as a consultant, campaigns hundreds of thousands of people saw, and from a 2026 launch built to this pattern in-house.*

## What it is

An incentive loop is a campaign that pays people in something real for a specific, verifiable public action. Follow the company account. Follow the founder. Retweet the announcement post. Leave a comment on it. The participant does the thing, the software checks that they did it, the reward lands.

For most of the last decade the sensible way to run one was to rent it. Quest platforms existed because the two hard parts, verifying a social action and holding the state of a multi-step claim, were genuinely hard to build and easy to buy. That is no longer true. Building the loop yourself is now the default option, and renting is the exception you should have a reason for.

## Why the math inverted

Three things moved at the same time.

**API access got cheap.** The 2023 lockout priced independent builders out of X's API entirely, and that era is what most operators are still pricing against. The tiers that cover a launch campaign now cost a rounding error against the campaign's own reward budget.

**You own the account doing the announcing.** This is the part operators forget. Verification is a read against data you already hold rights to: does this handle follow us, does this handle follow the founder, did this handle retweet this specific post ID. A handful of API calls, on your own account, about your own post.

**The software is a day of agentic building.** A claim page, a state machine over four steps, and a coupon grant is not a quarter of engineering anymore. It is an afternoon, and the operator can watch it get built.

Rent-versus-build was a real question when the build was a quarter and the API was closed. With the build at a day and the API open, the question answers itself.

## The data is the rent

The subscription is the visible price of a quest platform, and it is the smaller one.

Participants sign up with the platform in order to participate with you. The identity graph that results, who showed up, which handle or wallet they used, what else they have claimed across other campaigns, accrues to the platform as well as to you. That is how the category works. Aggregating participants across many campaigns is the product, and it is exactly what makes a quest platform worth using in the first place, because the audience is already standing there.

The campaigns that sourced this principle ran on GUILD.xyz, they reached hundreds of thousands of people, and they worked. The tradeoff was fine at the time, and it bought real distribution with tooling nobody could have built cheaply themselves. The change is that the tradeoff is no longer necessary, and a tradeoff you no longer have to make is one you should stop making.

Every participant who follows, retweets, and claims is a deposit. Owning the loop means the deposit lands in your [compounding customer intelligence](/concepts/compounding-customer-intelligence). Renting the loop means it lands in somebody else's, and yours gets a copy.

## Manual verification is where the loop dies

Under launch pressure there is a third option operators reach for, and it is worse than either renting or building. Ask people to paste a link to their comment. Have someone on the team open each link and confirm it. Apply the discount by hand.

The reflex is close to universal, and it kills the loop three ways.

**It does not survive volume.** The campaign exists to produce more claims than a person can look at. Succeeding at the campaign is what breaks the process, so the failure arrives at the exact hour it costs the most.

**It puts a human between the action and the reward.** The person retweeted because they were in the moment. A review queue delivers the reward hours or days later, after they have moved on. Instant is most of the power here, and the queue spends it.

**A discretionary reward reads as discretionary.** Someone who did the work and is waiting on a human to bless it is the person who posts about being stiffed. An automated check is a promise the software keeps on its own. A queue is a promise a busy team keeps when it gets to it.

The counterargument is real and worth stating plainly. At launch nobody has bandwidth, and "we will verify manually" is what a stretched team says when the automation sounds like a week of work. It is a day. The manual queue costs more than a day inside the launch week alone, and it charges that cost at the worst possible hour. Build the automated check first, and keep a human review queue only as the fallback for the edge cases the check cannot settle.

## The reward should be your own product

Pay in product. Three free months of the thing you just launched costs you marginal inference and storage instead of dollars, and it does two jobs where cash does one. It buys the public action, and it puts the person inside the product with a habit starting to form. A cash bounty buys the action alone, from someone who takes the money and leaves.

Tier the reward by who is claiming, and start with the people you already have.

- **Existing customers are the first audience, not the afterthought.** They have an account, a payment relationship already on file, and the strongest reason of anyone to claim. They are also the only audience you can reach on purpose: fire a prompt inside the product dashboard at the moment the announcement posts, instead of hoping they stumble across the campaign somewhere else. Their reward is an extension on what they already pay for, which costs you a delayed renewal rather than a check and buys retention on top of the public action.
- **New users are the second surface.** The public claim page catches the traffic the retweets bring in. Their reward is the trial that onboards them, paid for with capacity you already have.

Same campaign, two different jobs, one budget line measured in compute rather than currency. The sibling principle [Chips Not Cash](/principles/chips-not-cash) makes the same trade from the other side of the table: take the asset that compounds, not the currency that gets consumed.

## The claim window has to close

A reward with no deadline converts a fraction of what the same reward converts with one.

The loop is not up against a rival offer. It is up against the intention to do it later, which is where these campaigns go to die. Someone reads the announcement, agrees with every word, means to retweet it after the meeting, and never does. No amount of extra reward fixes that. A closing window does.

So say the window out loud and keep it short. Act today and the month is on us. The deadline is what converts an audience that agrees with you into an audience that acted.

## What the loop actually looks like

The whole artifact, end to end, from the launch this principle was proven on:

1. The announcement post goes out from the company account. Its post ID is the anchor for everything downstream.
2. The claim page asks the visitor for their handle and nothing else.
3. **Step one: follow the company account.** The page verifies the follow against the company's own follower data.
4. **Step two: follow the founder's account.** Verified the same way.
5. **Step three: retweet the announcement.** Verified against that specific post ID, so a retweet of some other post does not count.
6. **Claim.** With all three green, the page grants a coupon good for three free months, and it says plainly on the way in that the window closes today.

Two details carry more weight than they look like they do. Each step is a persisted state on the participant's record, so a person who drops out at step two comes back to step two instead of starting over. And each verification reads your own account's data, which is why none of this requires a third party to sit in the middle holding the participant list.

That is the artifact this principle produces. A page, a table, and a coupon grant.

## A prize without a point of view is a bribe

The mechanics above are the cheap half. They get the reward into the right hands. They do nothing to make the retweet travel past the people you rewarded.

What makes it travel is that the post says something the sharer actually wants their name on. The launch this spec came from was built around a claim before it was built around a reward, and the claim had a line:

> Protect your right to co-write.

Two things in that line are doing real work.

The first is who it is addressed to. It speaks to people who have already changed how they work. Once you have co-written with AI and watched it make your work better and faster, you will defend it without anyone having to persuade you. The campaign hands people who already crossed that line something to stand behind, which is a far shorter distance to travel than recruiting a stranger to a cause.

The second is the generalization, and it is the sharp end. Co-design is uncontroversial. Co-working is uncontroversial. The word is already in ordinary use for every other kind of assisted work. Singling writing out of that set and treating assistance there as suspect is an inconsistency in the norm. Naming the inconsistency is a stance about authorship, and it gives the sharer an argument they can defend in their own replies, which is the real test of whether a post travels past the first ring.

It ran at a moment when AI-assisted writing was widely treated as something to be caught and punished, and the people who spread it were people who had been on the wrong end of that or expected to be. The reward bought speed and volume on an opinion they already held.

The test, before you spend anything:

> Would a meaningful number of these people have posted this unpaid, because it says something they want their name on?

If the answer is no, the reward is doing all the work. The campaign stops dead at the boundary of the people you paid, and what you built is a bribe with good software around it.

## Further Reading

- [Own the Substrate](/principles/own-the-substrate): the same instinct on the inference side. This principle is its growth-side case.
- [Compounding Customer Intelligence](/concepts/compounding-customer-intelligence): why keeping the participant graph is the point.
- [Chips Not Cash](/principles/chips-not-cash): the pay-in-the-compounding-asset sibling.
- [It's Not Cold If They Liked Your Post](/principles/not-cold-if-they-liked-your-post): everyone who engaged with the campaign is the warm list you just built.
