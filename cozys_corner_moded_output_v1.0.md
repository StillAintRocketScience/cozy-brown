---
id: okf://cozys-corner/mode-d-output
title: Cozy's Corner — STORYFRAME-V Mode D Website Output v1.0
type: Worked Example
status: draft
version: 1.0
source: STORYFRAME-V v1.3.0 Mode D run #1 (2026-07-04)
relations:
  - {predicate: DERIVED_FROM, target: okf://cozys-corner/silo-map}
---

# COZY'S CORNER PRODUCE MARKET — Mode D Output v1.0
*STORYFRAME-V v1.3.0 · Mode D "Website" · consumer: naics_client · 2026-07-04*

> **3-line summary:** Production Mode D run #1 — Website Prompt Manifest (1 hero-image prompt + 3 clip prompts) and Site Build Brief for the Cozy's Corner cinematic home experience (Silo 1 hub). Gate confirmed 2026-07-04 with Sir's project brief superseding earlier direction (terracotta/gold accents adopted over DESIGN.md v0.2 tomato red — conflict surfaced and resolved). SNAP/EBT confirmed 2026-07-04; weekly deals populated with simulated placeholder data (incl. Soursop line). Store hours supplied 2026-08-03 (Mon–Sat 8 AM–6 PM, closed Sunday) — no store-hours [GAP] remaining; only real weekly-deal prices left before publish.

```
metadata:
  build_id:            storyframe-v
  build_version:       1.3.0
  mode_used:           D
  website_classification:
    website_archetype: local_business
    confidence:        0.96
    chained:           false
    clip_plan:         3 clips · 1080p · 16:9 · ~8s (spec) / ~10s (as generated) · no audio
    format_source:     auto (gate-confirmed 2026-07-04)
  website:
    consumer:          naics_client
    hero_reference_type: generate
  image_model:         nano_banana
  video_model:         seedance (spec) — clips actually produced on Google Omni Flash, ~10s each; assets locked in Cozy Brown/assets/ 2026-07-04
```

---

# PART 1 — WEBSITE PROMPT MANIFEST

### 1.1 Hero Image Prompt (Nano Banana — generate FIRST, this is the identity reference for every clip)

```
Professional food photography: a rustic woven market basket overflowing with
vibrant fresh produce — ripe red tomatoes, orange carrots with leafy green
tops, deep purple grapes, crisp green lettuce, red apples — on a weathered
wooden farm table, drenched in warm golden-hour sunlight from the left,
fine water mist beading on the produce, soft warm cream background falling
out of focus. Warm, neighborly farmers-market feel. Natural color, high
detail, appetizing, no people, no text. 16:9.
```

*Direction note: the basket contents deliberately mirror the Cozy's Corner logo illustration (tomatoes, carrots, grapes, lettuce, apples) so the photographic identity echoes the brand mark.*

**Producer step (HITL gate 2):** generate 2–3 takes; keep the one where the produce reads most natural and appetizing. This image is attached to EVERY clip generation below. Save as `hero-ref.png` in the assets folder.

### 1.2 Reference Rule (verbatim, opens every clip prompt)

> "Use the attached hero image as the visual reference — same basket, same produce varieties, same warm golden sunlight and rustic wood, so all clips read as the same market on the same morning."

### 1.3 Clip Prompts (Seedance — std mode, 1080p, 16:9, no audio, ~8s each)

**`clip-01-fresh-hero.mp4`**
```
Use the attached hero image as the visual reference — same basket, same
produce varieties, same warm golden sunlight and rustic wood, so all clips
read as the same market on the same morning. Extreme slow-motion macro
glide across the basket: water mist drifting down over the tomatoes and
lettuce, droplets beading and rolling, sunlight flaring softly through the
carrot greens, camera drifting right in one smooth continuous move.
std mode, 1080p, 16:9, no audio, ~8s.
```

**`clip-02-the-bounty.mp4`**
```
Use the attached hero image as the visual reference — same basket, same
produce varieties, same warm golden sunlight and rustic wood, so all clips
read as the same market on the same morning. Slow cinematic dolly along a
market display of wooden bins overflowing with collard greens, sweet
potatoes, watermelon, squash, peppers and citrus, jars of local honey and
preserves catching the light at the end of the move, warm morning sun
streaking across the wood, gentle depth of field. std mode, 1080p, 16:9,
no audio, ~8s.
```

**`clip-03-the-welcome.mp4`**
```
Use the attached hero image as the visual reference — same basket, same
produce varieties, same warm golden sunlight and rustic wood, so all clips
read as the same market on the same morning. Overhead close shot of a pair
of hands gently placing ripe tomatoes and leafy greens into a brown paper
grocery bag on a wooden counter, warm sunlight from the side, steam-soft
morning atmosphere, unhurried and caring pace, no faces visible.
std mode, 1080p, 16:9, no audio, ~8s.
```

### 1.4 Chain Plan

`null` — local_business archetype is not chained. Clips may be generated in any order after the hero image is locked.

### 1.5 Naming Convention & Assets Contract

```
Drop folder:      Cozy Brown/assets/
Expected files:   hero-ref.png
                  clip-01-fresh-hero.mp4
                  clip-02-the-bounty.mp4
                  clip-03-the-welcome.mp4
Brand assets:     logo primary lockup (supplied 2026-07-04) — save as
                  logo-primary.png; secondary badge + CC monogram per
                  DESIGN.md §10 mark system when commissioned
```

---

# PART 2 — SITE BUILD BRIEF

### 2.1 Design Tokens (resolved: Sir's 2026-07-04 project brief > DESIGN.md v0.2 > archetype default)

```
--color-primary:      #2F5E30   (dark forest green — headers, nav, footer)
--color-surface:      #FFFFFF → #f6f3ec  (warm cream range, light mode ONLY)
--color-accent:       terracotta (earthy — CTAs, Daily Special badges)
--color-accent-gold:  gold (highlights, deal flashes)
--type-display:       Fraunces, bold serif (Google Fonts)
--type-body:          Inter / clean sans, high legibility
--grid:               8px spacing grid, Tailwind token conventions
--touch-target:       ≥44px
--contrast:           AA minimum everywhere, esp. image overlays
NOTE (conflict resolved): tomato red #D6462E CTA from DESIGN.md v0.2
superseded by terracotta/gold per Sir's brief. DESIGN.md revision pending
brand-board review (Gate 7) — do not silently back-port.
```

### 2.2 Sections (ordered; Silo 1 hub scope — cluster pages come later via NAICS pipeline)

| # | Section | Content | Bound clip | Scroll binding |
|---|---|---|---|---|
| 1 | **Hero** | Headline exactly: "Market Fresh Produce, Right Around The Corner" — constrained to exactly two lines, ~48px desktop scale. Two CTAs: **Directions** (maps link) + **Hours** (anchor to §7). Logo primary lockup in shared top nav. | clip-01 | `scrub_frame_sequence` desktop; mobile fallback: poster + muted autoplay loop |
| 2 | **New Management story** | "Under new management — come in and say hi." Short, warm, second person. | — | pinned text reveal |
| 3 | **Weekly Deals** | Full-bleed produce photo cards; semi-transparent backdrop-blurred bar at card bottom; item name + description LEFT, price BOTTOM-RIGHT. `SIMULATED — replace with Sir's real weekly items/prices before publish:` Fresh Soursop (Guanabana) — $4.99 ea · Dried Soursop Leaves — $3.49/bag · Soursop Leaf Tea — $5.99/box · Vine-Ripe Tomatoes — $1.99/lb · Sweet Georgia Peaches — $2.49/lb · Collard Greens, bunch — $1.79 | clip-02 | `background_loop` (section backdrop) |
| 4 | **Daily Specials** | High-contrast "Daily Special" badges (terracotta fill, cream text), neighborhood favorites: Conecuh sausage, Joyce's Cheese Straws, local honey, fresh salsa, Amish pickled vegetables & jellies. | — | pinned_reveal |
| 5 | **What's Fresh** | Rotating product highlights from the master list (collards, turnip greens, sweet potatoes, watermelon, fresh corn, citrus…) — **plus new carry line:** fresh Soursop fruit, dried Soursop leaves, Soursop tea. Plain prices per Do's/Don'ts. | clip-03 | `pinned_reveal` |
| 6 | **SNAP/EBT + value strip** | **Confirmed 2026-07-04 — cleared to publish.** Gold badge, dark text, "Fresh doesn't have to be expensive. We accept SNAP/EBT." | — | static |
| 7 | **Visit Us** | Address: 4102 Saint Stephens Rd, Eight Mile, AL 36612 · Phone: (251) 270-5174 · Email: cozybrown1941@gmail.com · Service area: Eight Mile · Whistler · Mobile · Prichard · Map embed. Service options: In-store pickup · In-store shopping · DoorDash delivery. Hours: **Mon–Sat 8 AM–6 PM · Closed Sunday** *(Sir-supplied 2026-08-03)* | — | static + map |
| 8 | **Storage Guide teaser** *(planned)* | One-card teaser linking to future `/produce-storage-guide/` (Silo 4). Marked "coming soon" or omitted at builder's discretion until silo pages exist. | — | static |
| 9 | **Footer** | Shared across screens: nav links (Shop Fresh · Deals · Visit Us), social — [Facebook](https://www.facebook.com/people/Cozys-Corner-Produce-Market/61578280414837/), 1-color logo stamp. | — | static |

**Shared UI:** top nav + mobile bottom bar (sticky **Directions / Hours** actions on mobile per DESIGN.md §8) and footer identical on all screens. Light mode only.

### 2.3 Compression Note

Compress all clips for web after generation (~90% size cut target); decompose clip-01 to a frame sequence for the desktop scrub; serve mobile the compressed mp4 loop instead — scrub frame sequences are too heavy for the mobile-first priority audience.

### 2.4 Verification Checklist

- [ ] Hero headline renders as exactly two lines at ~48px desktop and remains two lines ≥sm breakpoint on mobile scale
- [ ] Hero scrub smooth on desktop; mobile receives loop fallback (no scrub jank)
- [ ] Deal-card overlay bar passes AA contrast over the brightest frame of its background
- [ ] Price sits bottom-right on every deal card without covering the product
- [ ] Sticky Directions/Hours bar present and tappable (≥44px) on mobile
- [x] Store hours shipped as real data — Mon–Sat 8 AM–6 PM, closed Sunday (Sir-supplied 2026-08-03)
- [ ] Weekly Deals `SIMULATED` prices swapped for Sir's real week-1 items/prices before publish
- [ ] Logo lockup ≥120px in header; smaller placements use secondary badge/monogram (DESIGN.md §10)
- [ ] Light mode only; no dark-theme remnants from archetype defaults

### 2.5 HITL Gates (in order)

1. ~~Archetype + clip plan confirmation~~ — **CLEARED 2026-07-04** (Sir's project brief)
2. Hero image generation + take selection (2–3 takes, Nano Banana)
3. Clip generation + take selection (3 clips, Seedance; credits are Sir's)
4. Chain seam approval — **N/A** (not chained)
5. Browser QA pass on built site (checklist §2.4; mobile pass mandatory)
6. Publish/deploy + domain — human only (Gate 6); store hours now supplied (2026-08-03), so this now blocks only on swapping in real weekly-deal prices

---

## OPEN ITEMS FOR SIR

1. ~~**Store hours**~~ — ✅ SUPPLIED 2026-08-03: **Mon–Sat 8 AM–6 PM, closed Sunday** (wired into Hero CTA + Visit Us §2.2 rows 1, 7)
2. ~~SNAP/EBT~~ — **confirmed 2026-07-04**, section 6 cleared to publish
3. **Weekly deals** — currently simulated placeholder data (Soursop fruit/leaves/tea + produce staples); Sir to supply real week-1 items + prices before publish (repeats weekly; candidate for a scheduled refresh workflow later)

---

*Generated by STORYFRAME-V v1.3.0 Mode D paper instantiation · production run #1 of 2 toward the §9.2 Site Assembly Protocol trigger.*
