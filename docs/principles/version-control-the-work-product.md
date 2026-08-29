---
title: "Version Control the Work Product"
slug: /principles/version-control-the-work-product
description: "Put every document the business produces into a private repository, along with the reasoning that produced it. A commit log shows what changed. The reasoning is what makes the archive usable by an agent later."
image: "/img/comics/version-control-the-work-product.webp"
---

# Version Control the Work Product

*Put every document the business produces into a private repository, along with the reasoning that produced it. The commit log shows what changed; the reasoning is what turns the archive into something an agent can learn from.*

![Three-panel warm editorial strip on cream paper. Title bar: VERSION CONTROL THE WORK PRODUCT. Panel one, captioned "THE FOLDER GOES COLD": a woman in her thirties with a short blonde bob and a burgundy turtleneck slides a thick finished document into a plain grey filing drawer, a faint chill settling over the dull metal, while the amber laptop sits closed on the desk. Panel two, captioned "COMMIT THE REASONING TOO": she has taken the document back out and lays it beside a small notebook where she writes her reasoning, and a warm amber thread ties the two together and travels into the now open glowing laptop where a rounded agent in a gold military cap waits. Panel three, captioned "YOUR OWN PRECEDENT, MINED": inside the glowing laptop the agent stands before a tall orderly wall of many such tied pairs, drawing threads out of them and weaving a single new clean sheet, which she holds in her hands outside the screen. Footer bar: A DIFF SHOWS WHAT CHANGED. WRITE DOWN WHY.](/img/comics/version-control-the-work-product.webp)

---

*Articulated by [The Boutique Corporate Attorney](/mentors/the-boutique-corporate-attorney) in conversation, 2026-08-24.*

## What it is

Most professional services businesses already organize their work into containers. A law firm opens a matter. An agency opens an engagement. Inside it accumulate drafts, markups, memos, and the versions that got sent. The container closes and the folder goes cold.

This principle says the container belongs in a private Git repository, and the drafts belong there as commits. The point is not backup, which the firm already has. The point is that the work becomes a corpus with a history: every version of every document the business has produced, in order, with the decisions visible as diffs.

> "Should I version control the agreement, and put everything I think about the whole process in there?"
>
> — The Boutique Corporate Attorney, 2026-08-24

The answer is yes, and the second half of that sentence is the part most firms drop.

## The reasoning is the part that gets dropped

A diff shows that a clause changed. It does not show why. An operator who reads his own repository a year later can reconstruct what happened; an agent reading it cannot, and neither can a new hire.

The attorney who articulated this principle spotted the gap himself before anyone pointed it out:

> "You can only see one level if you look at the changes, if it is not documenting what I am actually thinking while I am making the changes. Me telling it to do stuff is not necessarily an explanation of why I am telling it to do stuff. So I should add my principles."
>
> — The Boutique Corporate Attorney, 2026-08-24

That is the whole practice in one observation. Commit messages carry the reasoning, or a working notes file in the container does. Either way, the *why* has to be written at the moment it is cheap, which is while the decision is being made.

The principles that recur across containers graduate out of the matter folder and into the firm's judgment corpus. See [The Firm Super Suit](/concepts/the-firm-super-suit).

## What the corpus becomes

Once several years of work sit in a repository with reasoning attached, the firm can do things that were previously impossible:

- **Mine its own precedent.** An agent reads every agreement the firm has ever produced, de-identifies it, and assembles a form library out of the firm's actual positions rather than a vendor's generic templates. The firm has been generating this asset for years and throwing away the extraction.
- **Answer "how do we usually handle this."** Today that question routes to whoever has been there longest. With a corpus it routes to a search.
- **See its own drift.** A position the firm held three years ago and quietly abandoned is visible as a diff. Sometimes the drift was an improvement and sometimes it was an accident.
- **Onboard against real work.** A new hire reads the actual reasoning behind real decisions instead of a style guide.

## Draw the confidentiality line first

This is the principle with the sharpest edge, and it deserves an explicit boundary before the first commit rather than after the first incident.

Separate the containers by sensitivity, and give each level its own repository and its own access rules. Identified client material, privileged communications, and regulated records live under the tightest scope, and often should not be version-controlled at all. De-identified patterns and form language can live under a wider one. The firm's judgment corpus, which holds no client data, is wider still.

Write the line down before you write anything into a repository, and confirm it against the firm's professional obligations with someone qualified to make that call.

## Where to start

Do not migrate the archive. Start with the next container the business opens, and run it as a repository: the documents as files, the versions as commits, the reasoning in the commit messages or a notes file beside them. Run it for a month.

The signal that it is working is when someone asks a question about the work and the answer comes from the repository instead of from memory.

## Further Reading

- [The Firm Super Suit](/concepts/the-firm-super-suit): what the accumulated corpus becomes as a business asset.
- [Own the Substrate](/principles/own-the-substrate): the sibling ownership principle, applied one layer down at the inference surface.
- [The Machine-Drivable Business](/concepts/the-machine-drivable-business): the wider program this practice serves.
- [The Boutique Corporate Attorney](/mentors/the-boutique-corporate-attorney): the mentor who articulated this.
- [truthmanagement.wiki: Anointed Repository](https://truthmanagement.wiki/concepts/anointed-repository): the governance act that makes a repository canonical.
- [truthmanagement.wiki: Seed an Organizational Wiki](https://truthmanagement.wiki/playbooks/seed-an-organizational-wiki): the companion build for the judgment corpus this practice feeds.
