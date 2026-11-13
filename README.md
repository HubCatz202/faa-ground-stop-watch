# FAA Ground Stop Watch

**Live site: https://hubcatz202.github.io/faa-ground-stop-watch/**

A live timeline of the FAA nationwide ground stop of 13 November 2026 and what followed.

## How to use it

- **Status card.** The card at the top says whether the ground stop is in effect, lifting or lifted, and when the feed was last checked.
- **Timeline.** Every update is filed under a numbered event, from the first outages through to the restart. Tap an event to see only that one. Tap Official, News or Social to see one kind of source. Switch between newest first and oldest first.
- **Trending.** Topics people are talking about, ranked by how widely each one shows up across the sources checked on the latest pass. Cards move up and down as that changes.

## How often it refreshes

A fresh pass over news and social sources runs about every 5 minutes. The page re-checks for new data about every 75 seconds, so new entries appear on their own. There is no need to reload.

## How to read an entry

- Each entry is a three-sentence summary written by Claude from public reporting and public posts.
- **Confirmed** means an official said it on the record. **Reported** means credible press. **Unverified** means a single source, a social post or a disputed claim.
- A post or article that repeats something already logged is folded into that entry under "Same content also on" instead of getting its own.
- Trending is an estimate from search coverage, not a feed from the platforms themselves.

## Colour and accessibility

The colour scheme is built on the Okabe-Ito colour-blind-safe hues, adjusted so every text pairing meets WCAG AA contrast (4.5:1) in both light and dark themes. Status is never shown by colour alone: each state has a symbol and a word.

## Report a bug or ask for a feature

Use the button at the top of the site, or open an issue here.

## How it is built

- `index.html` is the whole app. Pushing to `main` redeploys it through GitHub Pages.
- `data.json` on the `data` branch holds the entries, topics and status. It is rewritten on every refresh.

Made by HubCatz202 and Claude Fable 5.2.
