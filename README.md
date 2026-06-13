# date ♥

A one-way dating site — a dating site with exactly one person on it. The point
isn't to match against a pool of people; it's to get to know **one** person
(Sankha), feel out the compatibility, and chat with an agent who speaks in his
voice.

> **Draft.** This is an initial scaffold — not deployed. The chat agent runs on
> scripted placeholder answers for now; the plan is to feed it curated personal
> notes so it can answer genuinely while keeping private things private.

Intended deploy: **date.sankhacooray.com** via GitHub Pages (CNAME present, not
yet wired).

## Sections

1. **How it works** — the one-way, one-person premise
2. **Subtle clues** — small true things about personality + lifestyle, with
   cross-links to the sibling sub-sites (coffeelab, ensemble, fold, palette, mixlab)
3. **Compatibility** — a 5-question, nothing-saved vibe-check with a playful verdict
4. **Ask the agent** — a stubbed chat UI (canned responses keyed on topics)

## Files

| File | Purpose |
|------|---------|
| `index.html` | Single-file site, all CSS + JS inline |
| `CNAME` | GitHub Pages custom-domain pointer (date.sankhacooray.com) |

## Design notes

- Same type family as the sibling sites (Instrument Serif / DM Sans / JetBrains
  Mono), but its own warm "candle-lit" palette — rose + amber on deep wine.
- The compatibility quiz and chat are entirely client-side; nothing is stored or
  sent anywhere.

## Next steps

- [ ] Replace the scripted agent with a real model + curated personal-notes context
  (see `claude-api` skill; keep a clear public/private boundary)
- [ ] Decide what's safe to expose vs. what only "the real him" should answer
- [ ] Add icon set, OG image, PWA manifest (`web-share-meta-and-manifest` skill)
- [ ] Wire up GitHub Pages deploy + DNS for date.sankhacooray.com (not done yet)
- [ ] Add to the workspace's central dashboard if/when one exists
