---
name: Cozy's Corner Produce Market
description: Warm, neighborly local-produce brand for a single Eight Mile, AL storefront — fresh, affordable, trustworthy, mobile-first. Green badge identity with tomato-red CTAs.
dependencies: Google Fonts — Fraunces (display), Inter (body)
id: okf://cozys-corner/design
title: Cozy's Corner — DESIGN.md (Brand Spec)
type: Design Spec
status: draft
version: 0.2
source: uploaded circular logo + Sir brand brief
gate_required: true
---

# Cozy's Corner Produce Market — DESIGN.md

> STATUS: **v0.2 DRAFT — FOR BRAND BOARD REVIEW.** Sections 1–3, 7 and the Logo & Mark
> System below are derived from the uploaded circular logo. Values are proposals, not
> committed brand identity. Approve/adjust before publishing (brand-identity gate).
> Bracketed items still need a decision.

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
| Accent / CTA | `--color-accent` | `#D6462E` | Tomato red — buttons, "On Sale" |
| Accent warm | `--color-accent-warm` | `#E7B23C` | Sunny yellow — highlights, SNAP badge |
| Texture | `--color-texture` | `#C08A3E` | Basket tan — dividers, illustration only (not text) |
| Leaf | `--color-leaf` | `#5FA23C` | "Local"/"Organic" badges |
| Background | `--color-bg` | `#FBF8F1` | Warm off-white (not pure white) |
| Surface | `--color-surface` | `#FFFFFF` | Cards |
| Text | `--color-text` | `#1E2A1E` | Near-black green-tinted |
| Muted text | `--color-text-muted` | `#5C6657` | |
> Contrast check: `#D6462E` and `#2F5E30` both pass AA on `#FBF8F1`/white for buttons and body. `#E7B23C` yellow fails on white for text — use it as a fill/badge with dark text only. [confirm at build]

## 3. Typography Rules
*Echoes the logo's warm slab/serif in caps; pairs with a clean humanist sans for body.*
- **Display / Headings:** **Fraunces** (warm high-contrast serif) — caps for badges/section titles to nod to the logo. Fallback: Google Font, or Zilla Slab for a slabbier match.
- **Body / UI:** **Inter** — highly legible, mobile-friendly. Fallback: system-ui.
- **Type scale (px):** 12 / 14 / 16 / 20 / 28 / 40 / 56
- **Weights:** 400 body · 600 subhead · 800 display
- **Copy tone:** friendly, plain-spoken, second person ("Come see what's fresh today").

## 4. Component Stylings
- **Buttons:** radius 8px; **Primary** = tomato `#D6462E` fill, white text, darkens on hover; **Secondary** = green outline on transparent; disabled = muted tan. Min height 44px.
- **Inputs:** 1px `#C7CDBF` border, green focus ring, tomato error text.
- **Cards (product / deal):** radius 12px, soft shadow (§6), 4:3 image top, price bold, badge top-left.
- **Navigation:** green header, white wordmark; links — Shop Fresh · Deals & SNAP · Organic · Storage Guide · Visit Us; hamburger on mobile.
- **Badges:** SNAP/EBT (yellow fill, dark text) · On Sale (tomato) · Local / Organic (leaf green).

## 5. Layout Principles
- **Spacing scale:** 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64
- **Grid:** 12-col desktop, 4-col mobile, max-width 1200px
- **Rhythm:** section padding 48–64px desktop / 32px mobile; imagery given room to breathe.

## 6. Depth & Elevation
- **Elevation 0:** flat page surfaces. **1:** cards `--shadow-sm: 0 1px 3px rgba(30,42,30,.10)`. **2:** modals/sticky `--shadow-md: 0 6px 20px rgba(30,42,30,.15)`.
- **Surface hierarchy:** `--color-bg` < `--color-surface` (white cards) < raised.

## 7. Do's and Don'ts
- **Do:** lead with real produce photography; show prices plainly; surface SNAP/EBT prominently; keep hours + location one tap away; keep the green/tomato pairing consistent.
- **Don't:** stocky corporate gradients; hidden pricing; industry jargon ("perishable merchandising" stays backstage); tan or yellow as body text; the full detailed logo below ~120px (see mark system).

## 8. Responsive Behavior
*Mobile-first — the demand is "near me" on phones.*
- **Breakpoints:** sm 640 / md 768 / lg 1024
- **Touch targets:** ≥44px
- **Collapse:** nav → hamburger below md; product/deal cards stack to 1-col on mobile; sticky "Directions" + "Hours" bar on mobile store pages.

## 9. Agent Prompt Guide
- "Create a homepage hero for a local produce market emphasizing fresh + affordable + near me, green badge brand with tomato-red CTA."
- "Build a Weekly Deals page with a yellow SNAP/EBT badge and price-per-pound cards."
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
