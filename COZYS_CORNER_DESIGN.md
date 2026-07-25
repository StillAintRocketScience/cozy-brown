---
name: Cozy's Corner Produce Market
description: Warm, neighborly local-produce brand for a single Eight Mile, AL storefront — fresh, affordable, trustworthy, mobile-first. Green badge identity with terracotta CTAs and gold highlights.
dependencies: Google Fonts — Fraunces (display), Inter (body)
id: okf://cozys-corner/design
title: Cozy's Corner — DESIGN.md (Brand Spec)
type: Design Spec
status: draft
version: 0.3
source: uploaded circular logo + Sir brand brief
gate_required: true
---

# Cozy's Corner Produce Market — DESIGN.md

> STATUS: **v0.3 DRAFT — FOR BRAND BOARD REVIEW.** Sections 1–3, 7 and the Logo & Mark
> System below are derived from the uploaded circular logo. Values are proposals, not
> committed brand identity. Approve/adjust before publishing (brand-identity gate).
> Bracketed items still need a decision.

> **CHANGELOG v0.3 (2026-07-24) — ⛩ Sir's ruling, two corrections:**
> 1. **Accent is now TERRACOTTA, not tomato red.** This writes back a ruling made on
>    2026-07-04 during STORYFRAME-V Mode D run #1 (`cozys_corner_moded_output_v1.0.md`),
>    which recorded "tomato red #D6462E superseded by terracotta/gold per Sir's brief —
>    DESIGN.md revision pending." That revision is this one. Until now the governing
>    brand artifact still specified the superseded colour.
> 2. **The v0.2 contrast claim was false and is replaced with measurements.** v0.2 §2
>    asserted that `#D6462E` and `#2F5E30` "both pass AA on `#FBF8F1`/white for buttons
>    and body." Computed (WCAG 2.1 relative luminance, sRGB): tomato `#D6462E` is
>    **4.40:1** on white against a **4.5:1** body-text requirement — it fails for body
>    text. Every pair in §2 is now measured, and the specific role each colour may hold
>    is stated. Values carry a ratio or they do not ship.
> *Note on the replacement: "terracotta" spans a wide range. Classic terracotta
> `#E2725B` measures **3.09:1** with white text — worse than the colour being replaced.
> `#B4482F` was chosen because it is recognisably terracotta AND clears AA both as a
> fill and as text.*

## 1. Visual Theme & Atmosphere
- **Adjectives:** warm, fresh, honest, neighborly, unfussy
- **Atmosphere:** Roadside-market warmth meets a clean modern grocer. Round badge heritage, generous white space, real-produce photography forward. Reads instantly as *local* and *affordable* — never corporate, never sterile.
- **Density:** comfortable

## 2. Color Palette & Roles
*Sampled from the logo; accent chosen intentionally (green alone can't carry a UI or meet contrast on CTAs).*
| Role | Token | Hex | Notes |
|---|---|---|---|
| Primary | `--color-primary` | `#2F5E30` | Forest green — ring & wordmark |
| Primary dark | `--color-primary-dark` | `#234A26` | Hover/pressed, footers |
| Accent / CTA | `--color-accent` | `#B4482F` | **Deep terracotta** — buttons, "On Sale" *(supersedes tomato `#D6462E`, v0.3)* |
| Accent gold | `--color-accent-gold` | `#E7B23C` | Gold — highlights, SNAP badge *(same value as v0.2's "accent warm", renamed to the ruled role)* |
| Texture | `--color-texture` | `#C08A3E` | Basket tan — dividers, illustration only (not text) |
| Leaf | `--color-leaf` | `#5FA23C` | "Local"/"Organic" badges — **fill only, dark text** |
| Background | `--color-bg` | `#FBF8F1` | Warm off-white (not pure white) |
| Surface | `--color-surface` | `#FFFFFF` | Cards |
| Text | `--color-text` | `#1E2A1E` | Near-black green-tinted |
| Muted text | `--color-text-muted` | `#5C6657` | |

### 2.1 Contrast — measured, not claimed  *(WCAG 2.1 AA · computed 2026-07-24)*
AA bar: **4.5:1** body text · **3:1** large text (≥18.66px bold / ≥24px) and UI components.

| Pair | Ratio | Verdict |
|---|---|---|
| White text on terracotta `#B4482F` | **5.37:1** | ✅ button fills, any label size |
| Terracotta `#B4482F` text on `#FBF8F1` | **5.07:1** | ✅ usable as text (error text, prices) |
| Dark text `#1E2A1E` on terracotta | 2.78:1 | ❌ terracotta fills take **white** text only |
| Forest `#2F5E30` text on `#FBF8F1` | **7.16:1** | ✅ safe everywhere |
| White text on forest `#2F5E30` | **7.60:1** | ✅ green header, reversed marks |
| Dark text `#1E2A1E` on gold `#E7B23C` | **7.71:1** | ✅ SNAP/EBT badge as specified |
| Gold `#E7B23C` text on white | 1.94:1 | ❌ **never** as text — fill only |
| Dark text `#1E2A1E` on leaf `#5FA23C` | **4.78:1** | ✅ Local/Organic badges with dark text |
| Leaf `#5FA23C` text on `#FBF8F1` | 2.95:1 | ❌ **never** as text — fails even the large-text bar |
| Body `#1E2A1E` on `#FBF8F1` | **14.09:1** | ✅ |
| Muted `#5C6657` on `#FBF8F1` | **5.67:1** | ✅ |
| Basket tan `#C08A3E` on white | 3.02:1 | ❌ illustration/divider only, as v0.2 said |

**Rule:** no colour pair enters this spec without a computed ratio next to it. A claim
that something "passes AA" is not a measurement — v0.2 made that mistake by 0.1 of a
point, which is invisible to the eye and would have shipped.

## 3. Typography Rules
*Echoes the logo's warm slab/serif in caps; pairs with a clean humanist sans for body.*
- **Display / Headings:** **Fraunces** (warm high-contrast serif) — caps for badges/section titles to nod to the logo. Fallback: Google Font, or Zilla Slab for a slabbier match.
- **Body / UI:** **Inter** — highly legible, mobile-friendly. Fallback: system-ui.
- **Type scale (px):** 12 / 14 / 16 / 20 / 28 / 40 / 56
- **Weights:** 400 body · 600 subhead · 800 display
- **Copy tone:** friendly, plain-spoken, second person ("Come see what's fresh today").

## 4. Component Stylings
- **Buttons:** radius 8px; **Primary** = terracotta `#B4482F` fill with **white** text (5.37:1), darkens on hover; **Secondary** = green outline on transparent; disabled = muted tan. Min height 44px. *Never dark text on terracotta — 2.78:1.*
- **Inputs:** 1px `#C7CDBF` border, green focus ring, terracotta `#B4482F` error text (5.07:1 on background).
- **Cards (product / deal):** radius 12px, soft shadow (§6), 4:3 image top, price bold, badge top-left.
- **Navigation:** green header, white wordmark; links — Shop Fresh · Deals & SNAP · Organic · Storage Guide · Visit Us; hamburger on mobile.
- **Badges:** SNAP/EBT (gold fill, dark text — 7.71:1) · On Sale (terracotta fill, white text) · Local / Organic (leaf green fill, **dark** text — 4.78:1; white on leaf is only 3.13:1).

## 5. Layout Principles
- **Spacing scale:** 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64
- **Grid:** 12-col desktop, 4-col mobile, max-width 1200px
- **Rhythm:** section padding 48–64px desktop / 32px mobile; imagery given room to breathe.

## 6. Depth & Elevation
- **Elevation 0:** flat page surfaces. **1:** cards `--shadow-sm: 0 1px 3px rgba(30,42,30,.10)`. **2:** modals/sticky `--shadow-md: 0 6px 20px rgba(30,42,30,.15)`.
- **Surface hierarchy:** `--color-bg` < `--color-surface` (white cards) < raised.

## 7. Do's and Don'ts
- **Do:** lead with real produce photography; show prices plainly; surface SNAP/EBT prominently; keep hours + location one tap away; keep the green/terracotta pairing consistent.
- **Don't:** stocky corporate gradients; hidden pricing; industry jargon ("perishable merchandising" stays backstage); **tan, gold, or leaf green as text of any size** (all three are fill-only — see §2.1); the full detailed logo below ~120px (see mark system).

## 8. Responsive Behavior
*Mobile-first — the demand is "near me" on phones.*
- **Breakpoints:** sm 640 / md 768 / lg 1024
- **Touch targets:** ≥44px
- **Collapse:** nav → hamburger below md; product/deal cards stack to 1-col on mobile; sticky "Directions" + "Hours" bar on mobile store pages.

## 9. Agent Prompt Guide
- "Create a homepage hero for a local produce market emphasizing fresh + affordable + near me, green badge brand with terracotta CTA."
- "Build a Weekly Deals page with a gold SNAP/EBT badge and price-per-pound cards."
- "Design a Visit Us page with hours, map, and service area (Eight Mile, Mobile, Whistler, Prichard)."
- "Make an Organic Produce landing page in the Cozy's Corner system."

---

## 10. Logo & Mark System  *(DRAFT spec — addresses small-size legibility)*

The uploaded circular badge is the **Primary Lockup**. It's detail-dense and only holds up at large sizes. This system adds simplified marks so the brand survives at favicon / app-icon / map-pin scale.

| Tier | Use at | What it is |
|---|---|---|
| **Primary Lockup** | ≥ 120px | Full circular badge: ring + "COZY'S CORNER / PRODUCE MARKET" + full produce basket. Website header (large), signage, packaging, print. |
| **Secondary Badge** | 48–120px | Same green ring + dot border, but a **simplified flat basket silhouette** (2–3 shapes: basket + a couple of produce blobs), no fine highlights, drop "PRODUCE MARKET" or keep only "COZY'S CORNER." Social avatars, section headers. |
| **App / Favicon Monogram** | ≤ 32px | Green circle, white **"CC"** monogram *or* a single flat carrot/leaf glyph. No text ring. Browser tab, app icon, map pin. |
| **1-Color Stamp** | any | Solid green-on-white **and** reversed white-on-green versions of the Secondary Badge, plus a single-ink version for receipts, bags, rubber stamp. |

**Rules**
- **Clear space:** keep ≥ 25% of the badge diameter clear on all sides.
- **Min size:** Primary Lockup never below 120px / 1.25in print; use Secondary/Monogram below that.
- **Backgrounds:** on photos, place the mark on a solid white or green disc — never directly on busy produce imagery.
- **Weight fix:** in any redraw, bump "PRODUCE MARKET" to match "COZY'S CORNER" weight so it doesn't drop out when scaled.
- **Fix before production:** get a clean **vector (SVG)** redraw of all tiers, and reconcile the illustration style (flat/lightly-textured) with the flat ring. Do not send the current raster to signage.

**Deliverable set to commission (once brand board signs off):**
SVG + PNG (transparent, @1x/@2x/@3x) for each of the 4 tiers · favicon.ico + 180px apple-touch-icon · white-on-green & green-on-white variants.
