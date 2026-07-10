# Smallfolk — a whole village on one page

One click gives a GM a complete fantasy village on a single printable sheet:

- **10–11 villagers** with procedural woodcut portraits, appearance, manner,
  a public want, a relationship — and a secret in red ink
- **One Trouble** — a central mystery that casts real villagers as culprit,
  suspect, and witness, and rewrites their secrets to cohere
- **A rumor table (d8)** where every rumor has a speaker, and the GM sees
  which are TRUE and which are FALSE and why
- **Four keyed locations** — inn (menu, tonight's patrons), smithy (stock &
  prices), shrine (local god & custom), moot hall (three adventure hooks
  posted as notices)
- **A survey map**, GM/Player view toggle (red ink vanishes for screen
  sharing), print stylesheet, and **copy-as-Markdown** for prep notes

Everything is cross-referenced: rumors point at real people, patrons have
real grudges, hooks lead somewhere. Deterministic per seed — the URL *is*
the village. `index.html#wether-hollow-42` is the same village for everyone,
forever. System-neutral; no game's trademarks anywhere.

**Positioning:** no AI, no accounts, no ads, works offline, one file.
The tip link is the business model.

## Deploy to GitHub Pages (5 minutes)

```bash
cd smallfolk
git init && git add . && git commit -m "Smallfolk v1"
gh repo create smallfolk --public --source=. --push
gh api repos/{owner}/smallfolk/pages -X POST \
  -f "source[branch]=main" -f "source[path]=/"
```

Or in the web UI: create repo → upload files → Settings → Pages →
Deploy from branch `main` / root. The site is `https://<user>.github.io/smallfolk/`.

## Turn on the money

1. ✅ Tips go to [ko-fi.com/clevermonkey](https://ko-fi.com/clevermonkey) —
   wired into the toolbar and footer via `SUPPORT_URL` in `index.html`.
2. Optionally mirror the page on **itch.io** as a free/pay-what-you-want web
   tool — that's where Watabou's audience lives, and itch handles tips natively.

## License suggestion

MIT for the code; declare generated villages CC0 so GMs can publish them in
paid adventures without asking. (Generosity is the growth engine here —
same call Watabou made.)

## Roadmap candidates (post-launch, by demand)

- More Troubles (target 12+), more roles, name-flavor packs (norse, coastal…)
- "Open in Watabou" cross-link for a full village map
- PNG export of the portrait strip; NPC-only mode; hamlet/town size toggle
