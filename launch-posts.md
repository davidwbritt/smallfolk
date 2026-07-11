# Launch posts — paste-ready drafts

Rules of the road (from LAUNCH.md): one community per day, r/Solo_Roleplaying
first, reply to every comment for the first 24h, and always in your own voice —
edit anything here that doesn't sound like you. Read each sub's self-promo
rules on the day you post; a few require a flair or a specific weekday thread.

Links used below:
- Site: https://davidwbritt.github.io/smallfolk/
- itch: https://clevermonkey.itch.io/smallfolk
- Worked session: https://davidwbritt.github.io/smallfolk/example.html
- Sample village: https://davidwbritt.github.io/smallfolk/#bram-combe-7

---

## Day 1 — r/Solo_Roleplaying

**Title:** I built a free solo mystery sandbox: one click = a village, ten
suspects, a rumor table, and an oracle. No AI at the table, works offline.

**Body:**

Last night I arrived in a village called Ostenmoor. Two graves had been opened
in the night and closed again, tidily — nothing taken, and the sexton wasn't
sleeping. I played the whole investigation with a yes/no oracle and a journal,
and I genuinely didn't know who did it until the end, because the tool hid the
answer from me until I chose to look.

That's the thing I built: **Smallfolk** generates a complete village on one
page — 10-ish villagers with woodcut portraits and *interlocking* secrets, a
d8 rumor table where every rumor is about a real villager (marked TRUE/FALSE
for later), and one central mystery that casts actual locals as culprit,
suspect, and witness.

For solo play specifically:

- **Player view** hides all the secrets — so the mystery has a real hidden
  answer you can investigate without spoiling yourself
- A **journal** drawer: press ⚑ Begin and it writes your arrival scene; your
  oracle rolls and dice log themselves into it; **Export** gives you the whole
  session as markdown (I know this sub loves posting play journals)
- Built-in **oracle** (likely / even / unlikely → "Yes, and…" through
  "No, and…"), **spark words**, and a 2d6 **reaction roll**
- Everything is seeded: the URL is the village, forever — and every village
  belongs to a clickable regional shire map, so there's always a next town

Honesty section, because it matters here: **no AI runs at the table** — every
village is dealt from hand-curated tables by a deterministic algorithm, one
HTML file, works offline, no accounts, no ads, free. The tables and code were
built in an open human–AI collaboration, and the AI disclosure on the itch
page is checked accordingly. If that's a dealbreaker for you, no hard
feelings — I'd rather say it plainly than have you find out later.

Play it in the browser: https://clevermonkey.itch.io/smallfolk
Or the bare site (same thing): https://davidwbritt.github.io/smallfolk/
A full worked session, if you want to see the loop before trying it:
https://davidwbritt.github.io/smallfolk/example.html

It's free forever; villages you generate are CC0. If you try a solo session
in one, I would honestly love to read the journal.

---

## Day 2 — r/DMToolkit

**Title:** Smallfolk — a whole village on one page, where the rumors are
actually about the NPCs

**Body:**

Every town generator I tried gave me disconnected pieces: NPCs from one
table, rumors from another, hooks from a third — and none of them knew each
other. So I built the thing I wanted: one click gives you a village where
everything is cross-referenced.

Concretely, in one generated village: the innkeeper is skimming the levy to
pay a blackmailer; the shrine-keeper's private tallies "could hang someone";
rumor #5 confidently accuses the wrong woman; and the reward notice posted on
the moot hall door is about the actual crime. The rumor table marks which
rumors are TRUE and FALSE for you, with a note on why either matters.

What you get per click, on one printable page: 10–11 NPCs (portraits,
appearance, manner, a public want, a secret in red ink), a tavern with menu
and tonight's patrons, a smithy with prices, a shrine with a local god and
custom, three hooks, a village map, and one central Trouble weaving three
villagers together. **Player view** hides all the red ink for screen shares;
**Print/PDF** makes a 4-page handout; **Copy markdown** drops it into your
notes; the ‹ › arrows and a **shire map** put every village in a region with
a market town, a feud, and a pilgrimage road.

Seeded and deterministic — the URL *is* the village, so you can bookmark or
share one. System-neutral, free, no accounts, works offline; no AI at the
table (the tables/code were built in a disclosed human–AI collaboration —
nothing generates while you play). Villages are CC0, including for paid
adventures.

https://davidwbritt.github.io/smallfolk/ (or on itch:
https://clevermonkey.itch.io/smallfolk)

Built it for my own prep nights; feedback very welcome — the most-requested
thing gets built next.

---

## Day 3 — r/rpg_generators

**Title:** Smallfolk: seeded one-page village generator — interlocking NPC
secrets, derived rumor tables, regional shire maps, single HTML file

**Body:**

Technical bits first, since this sub appreciates them:

- **One self-contained HTML file** (~100KB, no dependencies, no network);
  GitHub Pages + itch, MIT-ish open source
- **Deterministic seeded generation** — the URL hash is the seed; same seed,
  same village, forever. `#daily` resolves to a UTC-dated seed (village of
  the day, same for everyone)
- **Coherence engine**: the Trouble template casts real roster NPCs as
  culprit/suspect/witness and rewrites their secrets to match; rumors are
  derived from actual secrets (distorted-true) or planted false, each tagged
  for the GM; tavern patrons reference their real relationships
- **Shires**: the numbered sheets of a seed-base (`foo-1…foo-9`) form a
  region with a generated map, market town, shrine, feud, and wedding — all
  consistent from any member village
- Procedural woodcut portraits (layered SVG), procedural village map, print
  stylesheet, markdown export, GM/player view, plus a solo suite (oracle,
  journal, reaction roll)

Provenance, stated plainly: no AI at runtime — it's tables and a PRNG. The
tables and code were written in a human–AI collaboration and it's disclosed
on the itch page. Output is CC0.

https://davidwbritt.github.io/smallfolk/
Sample village: https://davidwbritt.github.io/smallfolk/#bram-combe-7
Source: https://github.com/davidwbritt/smallfolk

Happy to talk implementation — the interconnection pass was the fun part.

---

## Day 4 — r/osr

**Title:** One-page village with a d8 rumor table where the GM knows which
rumors are lies — free, printable, system-neutral

**Body:**

I wanted the village equivalent of the one-page dungeon: everything a session
needs on a sheet I can print and spill ale on.

One click gives you: a village map, 10-ish villagers with woodcut portraits
and one secret each (in red ink — the player-view toggle removes the red pen
for handouts), a tavern with prices in honest copper, a d8 rumor table where
every entry has a speaker and a TRUE/FALSE mark, reaction rolls on 2d6, three
hooks posted at the moot hall, and one Trouble with a culprit, a falsely
suspected neighbor, and a witness who isn't talking. Prints to a clean
four-page handout.

The flavor leans hard into the mud: *"Nails, honest, per score — 4 coppers.
A sword, old. No questions asked or answered — 9 silvers."* Village mottos
like "Lock nothing; everyone knows everything." Every village sits in a
hundred with a market town, a shrine, and a feud over a moved boundary stone.

Free, no accounts, works offline, one HTML file, CC0 output. No AI at the
table — hand-curated tables and a seeded PRNG (the tables themselves were
built in a disclosed human–AI collaboration; saying it up front so nobody has
to ask).

https://davidwbritt.github.io/smallfolk/ · also on itch:
https://clevermonkey.itch.io/smallfolk

---

## Day 5 — Bluesky (thread of 2)

**Post 1:**
Meet Ostenmoor. Two graves opened in the night and closed again, tidily.
The shepherd did it — those were her letters buried with the dead — but
suspicion has landed on the innkeeper, over a mended spade.

None of this was written by hand. It's one seed of Smallfolk, my one-page
village generator: davidwbritt.github.io/smallfolk/#bram-combe-7

**Post 2:**
Every village: 10 folk with interlocking secrets, a d8 rumor table (GM sees
what's true), a tavern, a Trouble, a shire map of neighbors. Free, offline,
CC0, no AI at the table. Solo-friendly: oracle + journal built in.

#ttrpg #osr #solorpg #dnd

---

## Comment-thread ammunition (for replies, any venue)

- If asked "why not just use donjon/Eigengrau/Watabou": genuinely praise
  them (Watabou for maps especially — we're complementary, not competing);
  the difference is *coherence on one page*: the rumors are about the NPCs,
  the hooks are about the Trouble, and it fits on a sheet.
- If asked about the AI disclosure: the answer is already in every post —
  expand honestly, never defensively. "Nothing generates at the table; the
  tables were built with an AI collaborator and edited by a human; disclosed
  everywhere. The alternative was hiding it, and this hobby deserves better."
- If someone requests a feature: "good idea" costs nothing, and the roadmap
  rule is that the most-requested thing gets built — say so, then do it.
- If someone posts a journal or a favorite seed: that's the whole game.
  Celebrate it, ask to quote it on the itch page.
