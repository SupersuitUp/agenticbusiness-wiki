# agenticbusiness.wiki

*What mentors who have lived it would tell you about building a business that properly applies AI.*

Live at **[agenticbusiness.wiki](https://agenticbusiness.wiki)** (noindex, public).

---

## What this wiki is

Mentor-sourced ground truth for principals building agentic businesses. The wisdom is captured from conversations with specific operators who have built businesses worth the bar, attributed by name, with verbatim quotes where they said it best.

A business is **agentic** when it applies AI to its highest and best use: multiplying the human potential of the people inside it, in service of a mission that existed before the AI did. The goal is not headcount reduction. The goal is a business that delivers value at a scale that was previously impossible while keeping the irreplaceably human elements intact.

This wiki captures what the operators behind it have learned, plus what their mentors have shared, so the next principal does not have to discover it from scratch.

## Who it is for

The reader is the **principal**: the founder, the CEO, the operator of a business they are trying to build well. Someone who has decided to apply AI seriously, who wants to do it without losing the soul of what they built, and who is hungry for advice from people who have already navigated the harder parts of building.

Not for AI hobbyists. For people running a business with real stakes.

## How the wiki is shaped

- **[Start Here](https://agenticbusiness.wiki/)**: framing, in-progress disclaimer, what an agentic business is
- **[Principles](https://agenticbusiness.wiki/principles)**: the load-bearing rules. One per page, attributed to the mentor who articulated it.
- **[Mentors](https://agenticbusiness.wiki/mentors)**: who the wisdom comes from. One page per mentor.
- **[Concepts](https://agenticbusiness.wiki/concepts)**: the lexicon. Grows as terms recur across mentor conversations.
- **[Reference](https://agenticbusiness.wiki/reference)**: glossary, voice rules.

## Attribution

Every principle on this wiki names the mentor whose conversation surfaced it. Verbatim quotes live in blockquotes with the mentor's name and the date of the conversation. The wiki is the operators' wisdom captured, not the wiki author's invention. Where a principle has been articulated by multiple mentors, all contributors are credited.

## In-progress disclaimer

The wiki is a working document. Pages here are the best-current-capture of conversations with specific mentors, not finished theory. Expect substantial pruning, new principles surfacing, and old framings getting replaced when a sharper version arrives from a later conversation. The canon is what survives ten mentors and three years of building.

## Mentors currently on the wiki

- **[Michael B. Ajouz](https://agenticbusiness.wiki/mentors/mike-ajouz)** — Spar Holdings LLC, founding member of New Mountain Capital. Sourced the foundational principles on magic moments, niche domination, chips-not-cash, missionary-mercenary integration, and choosing which game to play.

## Voice rules

- No em dashes. Use periods, commas, or colons.
- One coined term lives in one place. Cross-link, do not redefine.
- Italic one-line definition under every H1.
- Verbatim quotes from mentors live in blockquotes with `— Name, YYYY-MM-DD`.
- Further Reading at the bottom, internal links first.
- Absolute paths for cross-links: `/principles/term`, not relative.
- `onBrokenLinks: 'throw'`. A broken cross-link fails the build.

Full voice rules: [reference/voice-rules](https://agenticbusiness.wiki/reference/voice-rules).

## Local development

```bash
npm install
npm start -- --port 4444
```

Opens at `http://localhost:4444`. Hot-reload on content changes.

Build to validate:

```bash
npm run build
```

## Deploy

Vercel auto-deploys from `main`. To deploy manually:

```bash
vercel --prod
```

## Repo layout

```
wiki.config.json    Per-wiki branding (single source of truth)
docusaurus.config.ts
sidebars.ts
docs/
  start-here/
  principles/
  mentors/
  concepts/
  reference/
src/
  css/custom.css
plugins/search-plugin/
scripts/
  generate-llms-txt.sh
  llms-txt-env.mjs
middleware.ts       Edge bot-block
static/
  img/favicon.png
  robots.txt
```

## Lineage

Forked from [SupersuitUp/wiki-template](https://github.com/SupersuitUp/wiki-template) on 2026-05-15. Conventions and tooling inherit from the template; content is original.
