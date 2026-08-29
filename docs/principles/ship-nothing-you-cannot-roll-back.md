---
title: "Ship Nothing You Cannot Roll Back"
slug: /principles/ship-nothing-you-cannot-roll-back
description: "The moment software has a second user, a bad change stops being your inconvenience and becomes someone else's outage. Automatic versioning is what makes going back one action instead of an excavation."
image: "/img/comics/ship-nothing-you-cannot-roll-back.webp"
---

# Ship Nothing You Cannot Roll Back

*Automatic versioning stops being a nicety the moment somebody other than you depends on the software. Every deploy leaves behind an immutable version you can return to in one action, because the hour you need that is the hour you are least able to build it.*

![Three panels. One, a calm afternoon: a woman at a warm wooden desk writes in a notebook, turned away from the glowing amber laptop where a neat stack of identical cards is quietly assembling itself, one sliding onto the top of the stack on its own, untouched and unnoticed. Two, the same desk at night with the laptop the only light: the top card has gone dull and cracked and a sub-agent has stepped back from it, and she reaches one tired unhurried hand in and lifts the card beneath it back into place. Three, close on one card lying open like a folder, holding small labelled slips resting together, code and data and environment and decisions and notes, her hand at the edge of it and not lifting it.](/img/comics/ship-nothing-you-cannot-roll-back.webp)

---

## What it is

Every change that reaches a user leaves behind a complete, addressable, immutable version of what was running before it. Going back is one command, and it is the same command every time.

The word doing the work is **automatic**. Versioning that depends on somebody remembering to tag a release is versioning you have on the calm days and lack on the bad ones, and the bad ones are the only days it exists for.

## The threshold is the second user

While you are the only user, a broken deploy is an inconvenience with a known owner who has full context and can sit with it until it is fixed.

The second user changes the category. Now a bad change is somebody else's outage, on somebody else's schedule, discovered by somebody who cannot read the code and does not know what changed. Your recovery time is their downtime.

That is the line where this moves from good practice to a condition of operating, and most operators cross it without noticing, because the second user arrives quietly.

## "We will add versioning when we need it" is the trap

You will add it when you are calm, thinking clearly, and nothing is on fire.

You will need it when you are none of those things: mid-incident, tired, with a customer waiting and four plausible causes. That is the worst possible moment to discover that going back means reconstructing last week's state by hand from memory and a chat log.

The build is cheap on a Tuesday afternoon and impossible at 11pm.

## What a safe version actually contains

Four properties, and a version missing any one of them will fail you at the moment it matters.

**It is immutable and addressable.** Not "the state of main last Thursday". A specific thing with a name you can say out loud.

**It carries everything that drifts, not only the code.** Configuration, environment, database schema, and in an agentic business the prompts, the model identifiers, the skill files and the evals. Carry the decisions too, one line on what this release was for, because six months later the person reading it is you and you will not remember. A rollback that restores the code and leaves the prompt from the broken release has restored nothing.

**Going back is ONE action.** If recovery is a documented seven-step procedure, you do not have rollback. You have a runbook, and a runbook executed under pressure by a tired person is where the second incident comes from.

**It has been rehearsed.** An untested rollback is a belief. Roll back to yesterday's version on purpose, on a normal day, and time it.

## The agentic business raises the stakes twice

**Change arrives faster than review.** Agents ship at a rate no human approves one by one, so the ability to undo becomes the control that scales when reading every diff stops scaling.

**The artifact got bigger.** A prompt edit is a deploy. A model version changing under you is a deploy you did not make. See [Own the Substrate](/principles/own-the-substrate) for why the reasoning surface has to be pinned and reproducible; this principle is that same discipline applied to your own releases, and neither works alone. Pinning the model while your prompts are unversioned leaves you in the same place.

## The test

Ask one question and insist on a number: **how long from "this is wrong" to "the old one is back"?**

If the answer is a duration, you have rollback and you know its cost. If the answer is a description of a process, you have a plan. If nobody knows, you have hope, and you will find out the number during your first real incident, in front of the user who found it for you.

## Further Reading

- [Own the Substrate](/principles/own-the-substrate)
- [Speed Is Determined by Infrastructure](/principles/speed-is-determined-by-infrastructure)
- [The Machine-Drivable Business](/concepts/the-machine-drivable-business)
- [Action Produces Information](/principles/action-produces-information)
- [You Cannot Delegate Your Judgment](/principles/you-cannot-delegate-your-judgment)
