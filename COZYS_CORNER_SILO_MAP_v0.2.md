---
id: okf://cozys-corner/silo-map
title: Cozy's Corner — Silo Site Map & Master Keyword Map
type: Reference
status: draft
version: 0.2
source: NAICS 445230 analysis dataset (re-scoped to local storefront)
relations:
  - {predicate: GOVERNED_BY, target: okf://cozys-corner/design}
---

# COZY'S CORNER PRODUCE MARKET — SILO SITE MAP & MASTER KEYWORD MAP

```
[ARTIFACT: Cozy's Corner Produce Market — Website SILO Architecture]
[VERSION: 0.2 — DRAFT]
[PIPELINE: NAICS 445230 (Mode A+B) → SEO #2 (clustering) → SEO #3 (SiteArchitect Pro)]
[KEYWORD SOURCE: Supplied — 445230 analysis dataset, re-scoped to local storefront]
[METRICS STATUS: ESTIMATE — pending Ahrefs/Semrush validation pass]
[DATE: 2026-06-30]
```

**Top-line (what it is / what's new / what needs your decision):**
- **What it is:** A single-storefront SILO website blueprint for Cozy's Corner — pillars, cluster pages, URLs, internal linking, navigation, and a master keyword→page map — built by running SEO Prompt #3 logic on the supplied 445230 keyword data.
- **What's new vs. the 445230 doc:** The national/publisher keyword universe was filtered down to the **local-business slice**. Wholesale-at-scale, B2G, and programmatic-SKU plays were dropped or flagged optional (delivery was also dropped in v0.1 — **corrected in v0.2**, see §0.1); SNAP/EBT and service-area pages were added because they fit Eight Mile / Prichard demographics.
- **Needs your decision:** (1) Keep or cut the **optional B2B/restaurant silo** (SILO 5); (2) confirm the **5-pillar scope** before I draft page content (#4/#5); (3) green-light the Ahrefs validation pass when the connector goes live; (4) **new in v0.2** — does DoorDash delivery earn its own cluster page, or stay a service-option line on Home + Visit Us? (see §0.1).

> **CHANGELOG v0.2 (2026-07-24) — ⛩ Sir's ruling: DELIVERY IS BACK.**
> v0.1 dropped delivery on the stated fact "they do in-store pickup, not delivery," and
> instructed "flag if added." Cozy's **does** offer DoorDash delivery — confirmed by Sir
> 2026-07-24. This document was the stale one: STORYFRAME-V Mode D run #1 (2026-07-04)
> already listed "In-store pickup · In-store shopping · DoorDash delivery" in its Visit
> Us section, and neither artifact flagged the other for ~3 weeks. Corrected below in
> §0, §0.1, the segment table, SILO 1, and the Visit Us cluster.
> **Knock-on effect worth naming:** v0.1's reasoning excluded the home-delivery shopper
> as a persona. That exclusion is void — delivery buyers are a real segment with a
> different intent (convenience-first, basket-building, no store visit) and any
> persona/UX work built on v0.1 needs re-checking on this point.

---

## 0. LOCAL RE-SCOPING — ASSUMPTIONS (flagged inline)

Business facts used (from `Cozy Brown.txt`): single brick-and-mortar market, **4102 Saint Stephens Rd, Eight Mile, AL 36612**; service area **Whistler, Mobile, Eight Mile, Prichard**; **in-store pickup + in-store shopping + DoorDash delivery** *(delivery confirmed 2026-07-24 — v0.1 wrongly recorded "no delivery")*; price range **$**; new management; categorized "Grocery Store" (true NAICS = **445230 Fruit & Vegetable Retailers**).

### 0.1 · DELIVERY — CONFIRMED, SCOPE OPEN
Cozy's offers **DoorDash delivery**. What that settles and what it does not:
- **SETTLED:** delivery is a real service option and must appear where a shopper decides
  whether to make the trip — the Home pillar and the Visit Us cluster, at minimum. It is
  no longer an excluded use-case, and the home-delivery shopper is no longer an excluded
  persona.
- **STILL OPEN (decision 4 above):** whether it earns its own cluster page. Third-party
  delivery is a different SEO play from the rest of this map — the transactional keywords
  ("produce delivery near me", "grocery delivery Eight Mile") point at DoorDash's own
  ranking surface, not at this site, and the site cannot take the order. A page is
  justified if it converts *awareness* ("you can get us delivered") rather than chasing
  the delivery query itself. Recommend: **service-option line now, page only if the
  keyword pass shows local delivery demand this site can actually capture.**
- **NOT a wholesale/D2C pivot:** DoorDash is a delivery channel over the same in-store
  inventory. The dropped items below stay dropped for their own reasons.

| Supplied segment (445230) | Local fit | Decision |
|---|---|---|
| Instant Proximity & Convenience | ★★★ Cash cow | **KEEP** — core of site |
| Localist Sourcing Advocate (locavore) | ★★★ | **KEEP** |
| Budget / Value Shopper | ★★★ (matches "$" + local demographics) | **KEEP** + add SNAP/EBT |
| Culinary Explorer / Organic | ★★ (premium subset) | **KEEP, lean** |
| Home Preservationist (storage) | ★★ (authority content) | **KEEP** as info silo |
| Recipe / Small-Basket (seasonal) | ★★ | **KEEP** (folded under Local) |
| B2B Commercial / Wholesale | ★ (only if selling to local restaurants) | **OPTIONAL — your call** |
| Delivery (3rd-party / DoorDash) | ★★ **CORRECTED v0.2** — they DO deliver via DoorDash | **IN SCOPE** as a service option; own page = open decision (§0.1) |
| D2C own-fleet home delivery | ✗ (not offered — DoorDash is the channel) | **DROPPED** |
| B2G procurement, SQF/lab, programmatic SKUs | ✗ (publisher/enterprise play) | **DROPPED** |

> ⚠ **Metrics flag:** All Vol/CPC/Competition figures below are the **supplied national-flavored estimates** from the 445230 dataset. They set *relative* priority correctly but are not Eight Mile-specific. Local "near me" volumes for a town this size will be far smaller in absolute terms; the *ranking* between terms should hold. Numbers get refreshed in the Ahrefs pass.

---

## Proposed SILO Structure for Cozy's Corner Produce Market

### SILO 1 — Fresh Produce Near Me (Core / Home Hub)
- **Pillar Page Primary Target Keyword:** `fresh produce near me` *(Est. Vol 50,000 | CPC $4.12 | Comp 39)*
- **Geo-anchor secondary:** `produce market in Eight Mile AL`, `produce near me`, `fruit and veg near me`
- **Core Pillar Content / Sections:** Who we are (new management) · what's fresh this week · the local promise · store hours & location map · service area · **how to get it: in-store · in-store pickup · DoorDash delivery** *(added v0.2)* · links to every other silo.
- **Proposed URL:** `/` (home)
- **Supporting Cluster Pages:**
  1. **Local & Farm-Fresh Produce** — KW `local produce near me` *(5,000 | $4.15 | 48)*; supporting: `farm fresh produce near me`, `locally grown produce near me`, `local produce`. **URL** `/local-produce/`
  2. **Seasonal & Local Favorites** — KW `fresh local tomatoes near me`; supporting: `seedless cucumbers near me`, `fresh local corn near me`, `limes near me`. **URL** `/seasonal-produce/`
  3. **Visit Us — Hours, Location & Service Area** — KW `produce market open now near me`; supporting: Eight Mile / Whistler / Mobile / Prichard. **Must carry the full service-options block: in-store shopping · in-store pickup · DoorDash delivery** *(v0.2)*. **URL** `/visit/` (+ optional `/locations/eight-mile/` etc.)

### SILO 2 — Affordable Produce & SNAP/EBT (Budget / Value)
- **Pillar Page Primary Target Keyword:** `cheap fresh produce near me` *(Est. 50–500 | CPC ~$2.45–$4.56 | Comp 53–97)*
- **Core Pillar Content / Sections:** Why fresh doesn't have to be expensive · this week's deals · we accept SNAP/EBT (and WIC if applicable) · price-per-pound value vs. chain grocers.
- **Proposed URL:** `/affordable-produce/`
- **Supporting Cluster Pages:**
  1. **Weekly Produce Deals** — KW `produce on sale near me` *(50 | $2.45 | 97)*; supporting: `cheapest fruits and vegetables near me`. **URL** `/affordable-produce/weekly-deals/`
  2. **SNAP / EBT Accepted Here** — KW `stores that accept EBT near me` / `SNAP produce near me` *(local civic-intent; high trust value — added, not in national dataset)*. **URL** `/affordable-produce/snap-ebt/`

### SILO 3 — Organic & Specialty Produce (Culinary / Health)
- **Pillar Page Primary Target Keyword:** `organic produce near me` *(Est. 5,000 | CPC $5.06 | Comp 96)*
- **Core Pillar Content / Sections:** Our organic & chemical-free picks · fresh herbs · specialty cultivars · what "local + organic" means here.
- **Proposed URL:** `/organic-produce/`
- **Supporting Cluster Pages:**
  1. **Organic Fruits & Vegetables** — KW `organic fruits and vegetables near me` *(500 | $5.02 | 100)*. **URL** `/organic-produce/fruits-vegetables/`
  2. **Fresh Herbs** — KW `organic fresh herbs` *(50 | $3.51 | 54)*; supporting: `organic basil`. **URL** `/organic-produce/fresh-herbs/`

### SILO 4 — Produce Storage & Freshness Guide (Authority / Informational)
- **Pillar Page Primary Target Keyword:** `how to keep produce fresh` / `best way to store produce` *(Est. 500 | CPC $0.47 | Comp 94 — low CPC, topical-authority play)*
- **Core Pillar Content / Sections:** Master storage guide · fridge vs. counter · reducing waste · links out to item-specific guides; pulls authority from the 445230 cold-chain knowledge.
- **Proposed URL:** `/produce-storage-guide/`
- **Supporting Cluster Pages:**
  1. **How to Store Vegetables** — KW `best way to store vegetables`; supporting: `keeping vegetables fresh in fridge`. **URL** `/produce-storage-guide/storing-vegetables/`
  2. **Keeping Produce Fresh Longer** — KW `keeping produce fresh longer`; supporting: `ball fruit fresh produce protector`. **URL** `/produce-storage-guide/keep-produce-fresh-longer/`

### SILO 5 *(OPTIONAL — your call)* — For Restaurants & Bulk Buyers (Local B2B)
- **Pillar Page Primary Target Keyword:** `produce wholesale near me` *(Est. 5,000 | CPC $5.76 | Comp 40)*
- **Rationale / flag:** Only worth building if Cozy's wants to supply local soul-food/catering kitchens in Mobile/Prichard. Adds a distinct buyer with its own intent. **If you say no, this silo is removed entirely.**
- **Proposed URL:** `/wholesale/`
- **Supporting Cluster Pages:** Bulk & case pricing (`fruit and veg wholesalers`); Restaurant sourcing (`local produce wholesale near me`).

---

## Internal Linking Strategy Overview
- **Home (SILO 1 pillar)** links down to all pillar pages and to its three clusters; every pillar links back to Home.
- **Pillar → Cluster / Cluster → Pillar** within each silo (standard SILO siloing) to concentrate topical authority; avoid cross-silo links *except* the deliberate bridges below.
- **Authority bridges (cross-silo, justified):** each `/produce-storage-guide/` cluster links to the matching product silo (e.g., *Storing Vegetables* → *Seasonal & Local Favorites*; *Keep Produce Fresh Longer* → *Local Produce*). This routes informational traffic toward transactional pages.
- **SNAP/EBT** and **Weekly Deals** cluster-link to each other and up to the Affordable pillar (shared budget intent).
- Keep the **organic** silo siloed from the generic "fresh produce" silo to prevent cannibalization (see flags).

## Main Navigation Suggestions
`Home` · `Shop Fresh` (SILO 1) · `Deals & SNAP` (SILO 2) · `Organic` (SILO 3) · `Storage Guide` (SILO 4) · `Visit Us` (hours/location) · *[optional]* `Wholesale` (SILO 5)

## Cannibalization Flags & Resolutions
- `fresh produce near me` (Home) vs `organic produce near me` (SILO 3) → **Differentiate** by the organic modifier; never optimize Home for organic terms.
- `fresh produce near me` (Home) vs `cheap fresh produce near me` (SILO 2) → **Differentiate** by price/deal intent; SILO 2 owns all "cheap/sale/affordable/EBT" modifiers.
- Synonym sprawl — `veggies near me`, `fresh veggies near me`, `fruit and veg near me`, `fresh vegetables near me` → **Consolidate** onto the Home pillar (one page, listed as secondary keywords). Do **not** build a page per synonym.
- `best store for produce` / `best produce grocery store` → assign to **Home** as a secondary/"why us" angle, not a standalone page.

---

## Consolidated Master Keyword & Page Mapping List

- **Pillar — SILO 1: Home / Fresh Produce Near Me** — `/`
  - **Primary:** `fresh produce near me`
  - **Supporting:** `produce near me`, `produce market in Eight Mile AL`, `fruit and veg near me`, `best store for produce`
- **Cluster — Local & Farm-Fresh Produce** — `/local-produce/`
  - **Primary:** `local produce near me`
  - **Supporting:** `farm fresh produce near me`, `locally grown produce near me`, `local produce`
- **Cluster — Seasonal & Local Favorites** — `/seasonal-produce/`
  - **Primary:** `fresh local tomatoes near me`
  - **Supporting:** `seedless cucumbers near me`, `fresh local corn near me`, `limes near me`
- **Cluster — Visit Us (Hours / Location / Service Area)** — `/visit/`
  - **Primary:** `produce market open now near me`
  - **Supporting:** `produce market Eight Mile AL`, `produce market Prichard AL`, `produce market Mobile AL`
- **Pillar — SILO 2: Affordable Produce & SNAP/EBT** — `/affordable-produce/`
  - **Primary:** `cheap fresh produce near me`
  - **Supporting:** `cheapest fruits and vegetables near me`, `affordable produce near me`
- **Cluster — Weekly Produce Deals** — `/affordable-produce/weekly-deals/`
  - **Primary:** `produce on sale near me`
  - **Supporting:** `cheapest fresh produce near me`, `produce specials`
- **Cluster — SNAP / EBT Accepted** — `/affordable-produce/snap-ebt/`
  - **Primary:** `stores that accept EBT near me`
  - **Supporting:** `SNAP produce near me`, `WIC produce near me`, `EBT grocery Eight Mile`
- **Pillar — SILO 3: Organic & Specialty Produce** — `/organic-produce/`
  - **Primary:** `organic produce near me`
  - **Supporting:** `organic food market near me`, `fresh organic produce`
- **Cluster — Organic Fruits & Vegetables** — `/organic-produce/fruits-vegetables/`
  - **Primary:** `organic fruits and vegetables near me`
  - **Supporting:** `organic vegetables near me`, `fresh organic fruit near me`
- **Cluster — Fresh Herbs** — `/organic-produce/fresh-herbs/`
  - **Primary:** `organic fresh herbs`
  - **Supporting:** `organic basil`, `fresh herbs near me`
- **Pillar — SILO 4: Produce Storage & Freshness Guide** — `/produce-storage-guide/`
  - **Primary:** `how to keep produce fresh`
  - **Supporting:** `best way to store produce`, `reduce food waste produce`
- **Cluster — How to Store Vegetables** — `/produce-storage-guide/storing-vegetables/`
  - **Primary:** `best way to store vegetables`
  - **Supporting:** `keeping vegetables fresh in fridge`, `how to store leafy greens`
- **Cluster — Keeping Produce Fresh Longer** — `/produce-storage-guide/keep-produce-fresh-longer/`
  - **Primary:** `keeping produce fresh longer`
  - **Supporting:** `ball fruit fresh produce protector`, `store fruit and vegetables`
- **Pillar — SILO 5 (OPTIONAL): For Restaurants & Bulk Buyers** — `/wholesale/`
  - **Primary:** `produce wholesale near me`
  - **Supporting:** `fruit and veg wholesalers`, `local produce wholesale near me`, `produce warehouses near me`

---

## Build-Order Priority (from supplied metrics)
1. **SILO 1 Home + Local cluster** — captures the 50,000-volume proximity cash cow. Build first.
2. **SILO 2 Affordable + SNAP/EBT** — high local relevance, low competition on EBT terms, matches "$" positioning.
3. **SILO 4 Storage Guide** — low-CPC topical-authority engine that feeds transactional silos via internal links.
4. **SILO 3 Organic** — smaller but higher-CPC premium traffic.
5. **SILO 5 Wholesale** — only if you opt in.

## Validation Pass (deferred per your direction)
When Ahrefs/Semrush is connected: pull Eight Mile / Mobile-AL local volumes for every Primary keyword above, re-rank build order on real numbers, and confirm SNAP/EBT + service-area terms (not in the supplied set) carry local demand. Architecture is not expected to change materially.
```
[END ARTIFACT v0.1]
```
