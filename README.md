# Hidden Tide

**The Hitchhiker's Guide to the Ocean's Hidden Data** - a playful, ocean-native guide to AI-native discovery from free ocean data that already exists. Live at [hiddentide.com](https://hiddentide.com).

## What this repo is
A single static site. No framework, no build step, no dependencies. Just open `index.html`.

- `index.html` - the main guide (the Big Idea, the 42 ideas, the Four, Category Zero, the data estate).
- `method.html` - the methods reference ("the manual in the glovebox").
- `roster.html` - the expedition roster (who is diving on what).
- `roster.json` - **the crew list. This is the file the roster reads.** Edit it to add a crew member; the page updates automatically.
- `netlify.toml` - Netlify config (publish = `.`, no build).
- `robots.txt` + `sitemap.xml` - crawler and AI-answer-engine discovery (all bots welcomed).
- `llms.txt` - a structured brief for LLMs / AI answer engines, with the honesty framing up top so the project is represented accurately (candidates, not results).
- `favicon.svg` - tab icon.

Each page's `<head>` also carries: meta description, canonical URL, Open Graph + Twitter cards, `theme-color`, and (on the home page) a `WebSite` JSON-LD structured-data block for clean entity attribution by search and AI engines.

### After go-live (manual, one-time)
Verify the site in Google Search Console and Bing Webmaster Tools and submit `sitemap.xml`. (Optional: add a 1200x630 `og:image` for richer social/link previews - not included, needs a real image asset.)

## Deploy
Hosted on Netlify, auto-deploys on every push to `main`. Domain (hiddentide.com) is on Infomaniak DNS pointed at Netlify. No build command; publish directory is the repo root.

## Join the crew (claim a dive)
Pick any idea (the 42) or a Category Zero engine, then add yourself to `roster.json` via a pull request (or open a "claim a dive" issue and a maintainer adds you). One object:

```json
{
  "title": "The Barnacled Cartographer",
  "handle": "@yourhandle",
  "github": "https://github.com/yourhandle",
  "diving": "#11 The Shrimp Are Doing Your Oceanography",
  "link": "index.html#idea-11",
  "since": "2026-07-10",
  "status": "scout",
  "statusText": "scouting",
  "blurb": "one honest line on what you are up to"
}
```

`status` is one of `scout` / `build` / `found` (amber / teal / pink chips). `title` is your Guide-given expedition name. The first four entries are the AI Dreamers that charted the map, kept honestly labelled `(AI)`.

## The one rule
If you find something, it only counts once it **replicates on data you did not use to find it**. See `method.html`.
