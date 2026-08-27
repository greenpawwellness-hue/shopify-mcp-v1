# Green Paw Grid Planner

A self-contained Instagram grid planner for Green Paw Wellness. Open
`index.html` in any browser — no build step, no dependencies, no network
calls beyond Google Fonts.

## What it does

Previews the next four weeks of posts as an Instagram profile grid, laid out
the way the feed actually fills in (newest top-left, so post 1 is the
bottom-right square). Clicking a square opens the full brief for that post:

- hook and angle
- shot list (reels) or slide-by-slide arc (carousels)
- a drafted caption and hashtag set
- CTA, what to shoot, and why the post earned a slot
- a compliance flag where the copy sits near the line

Below the grid: a bench of ideas that didn't make the cycle, and a
guardrails card carrying the brand brief's never-use words and their
approved replacements.

Post status (Idea / Drafted / Scheduled / Posted) is stored in the browser's
`localStorage`, so marks persist per browser and never leave the machine.

## Where the content came from

Every post traces to an existing Green Paw source rather than being invented:

| Source | Used for |
|---|---|
| `Green-Paw-Wellness-Master-Brand-Brief.pdf` | voice, vocabulary, colors, product line, compliance rules |
| `GPW Instagram Flywheel` | reel analytics, persona board scores, idea backlog, hook library, captured competitor angles |
| `01-Content-Studio-SYSTEM` | carousel arc, caption structure, hashtag rules |
| `Social Media Ideas` | ambassador carousel, FAQ topics |
| `Reel Hook Ideas / Content Brainstorm` | reel templates, breed-callout angles |

The mix was set against gaps the flywheel data made visible: reels kept
under 15 seconds (the 6.2s reel looped, the 22s and 31s reels leaked through
the middle), cats named in 5 of 12 posts (the cat persona scored three of the
last five planned reels at 4/10 for being dog-only), and the account's one
proven winner mined twice from different angles.

## Editing

Post content lives in the `POSTS` array in the inline `<script>`; bench ideas
live in `BENCH`. Both are plain objects — edit them directly. Brand colors
and bucket colors are CSS custom properties at the top of the `<style>`
block.

Post tile colors are intentionally theme-independent: the page chrome
responds to light/dark, but a post tile does not, because a real Instagram
post doesn't change with the viewer's OS setting.
