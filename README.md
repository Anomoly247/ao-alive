# AO ALIVE — our own rebuild

Our own rebuild of the **AO ALIVE home page** for **anomoriginals.lol**,
replacing the Manus build.

## Why this repo exists

The live anomoriginals.lol home page was built in Manus, and its source was
never in GitHub — a full search of all 34 Anom Originals repos (Nov 20, 2026)
found none of the live page's code. Eliza is done paying for Manus. So we are
rebuilding the site ourselves, here, hosted free on GitHub Pages.

**Status: work in progress, draft preview only — NOT live yet.** The live
domain still points at Manus. Nothing here changes the live site. The switch
happens only with Eliza's explicit say-so, after she has seen and approved
the preview.

## What is in here

- `index.html` — the home page, plain static HTML. No build step, no server,
  no sign-in, no payments, no tracking.
- `styles.css` — the page's styles, built to the **AO ALIVE Living Design
  Standard v2.0** (Eliza's spec, `AO_ALIVE.pdf`): Void `#0A0A10` canvas,
  True Black `#000000`, Panel `#141423`, Deep `#08080f`; cyan `#00eaff` =
  Active, magenta `#ff00c8` = In Build, gold `#d8ae55` = Planned; Space
  Grotesk / Space Mono display, Inter body, JetBrains Mono technical;
  glassmorphism panels (blur 18px, radius 16–24px); staggered breathing —
  Houses 3.2s / 3.6s / 3.9s / 4.1s, logo 2.6s, orbits 3.8s / 4.0s / 6.0s /
  7.0s, 180-star drift, every element on its own period, and
  `prefers-reduced-motion` respected. No purple anywhere in the UI CSS;
  the dragon art keeps its own colours.
- `assets/` — Eliza's own dragon and character art, downloaded from the live
  site's own files. All artwork, characters, and worlds are original
  intellectual property of Anom Originals.

## The flow (Eliza's decisions, Nov 20, 2026)

A brand-new visitor meets the page in this order:

1. **Vision first** — what AO is, in the live page's own words.
2. **Safe word right after** — "Oly Oly All Come Free."
3. **A tiny story** — one small thing to try (the Anoms Corner guided
   reflection already on the live site; nothing is saved or sent anywhere).
4. **Then into the worlds** — the 17-world constellation, with the same
   LIVE / BUILD / PLANNED statuses as the live page.

## The fixed AO NETWORK strip

The live strip was one row that scrolled sideways with a hidden scrollbar,
so the last two links (anomarsty.lol and the aoliving alias) slid off the
edge where nobody could see them. Here the six links wrap onto a second row
instead, so all six are always visible. Same links, same order, same dark
style. The fix is one CSS idea:

```css
.ao-network__links { flex-wrap: wrap; }
```

## Honest note about the two Manus links

Two of the six network links are still hosted on Manus:

- **aosanctry-hukq4zpo.manus.space** — the Sanctuary runtime. It will need
  a new home when Manus goes.
- **aoliving-kry92twk.manus.space** — a WebDev-hosted alias. It is just a
  copy of this home page, so nothing is lost there.

They are kept in the strip for now because they are part of the live site
today, and each is flagged on the page itself.

## Hosting

Free GitHub Pages project page (main branch, root). No CNAME file is in this
repo on purpose — the anomoriginals.lol domain still points at Manus until
Eliza approves the switch.

## What this rebuild does NOT do

- No invented lore. Wendigo and Ozka stay as they are on the live page.
- No merged versions, no changed prices, no new shop.
- No sign-in, no accounts, no data collection. The contact link is a plain
  `mailto:` to anom@anomoriginals.lol.
- No Fubar link anywhere in AO materials (Eliza's rule: the word is fine,
  the link is not).
