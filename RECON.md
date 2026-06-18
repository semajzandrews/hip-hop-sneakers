# RECON · Hip Hop Sneakers

**Slug:** hip-hop-sneakers
**Stage:** REVIEW (no deploy)
**Built:** 06-17-2026

---

## Verified facts

- **Name:** Hip Hop Sneakers
- **Category:** Sneaker boutique / streetwear (shoe store + general store)
- **Address:** 211 S Main St #1, City of Orange, NJ 07050
- **Phone:** (973) 677-1260  ·  CONFIRMED
- **PIN (last 6 of phone):** 771260  ·  CONFIRMED (matches facts file)
- **Existing website:** NONE owned. Only directory aggregator pages exist
  (Yelp, businessyab, locally.com, manta, yellowpages, a localsearch.com
  auto-generated stub). No real first-party site. Premise holds.
- **Rating:** 3.7 (soft). Per kit note: soft-pedaled. Reviews are NOT a
  star-count section; one organic product-truth quote used instead
  ("Copped my Bred 13s right here"), drawn from a real review mentioning
  buying Bred 13s at this location.

### Hours (12-hour, America/New_York)
Two sources differed slightly. Used the more detailed per-day listing
(businessyab) as primary:

- Mon to Sat · 9:30 AM to 8 PM
- Sunday · 10 AM to 7 PM

(Alt source Yelp-derived suggested Mon-Sat 8 AM-7 PM / Sun 10 AM-6 PM. If the
owner confirms different hours at the door, swap the HOURS object in the JS and
the two hours lists. The live Open/Closed pill is computed from the JS HOURS
map, so it stays correct automatically.)

### Products / services (verified from listings + reviews)
- Sneakers (Jordans incl. Bred 13s, Air Force 1, runners, classics)
- Hats (fitteds, snapbacks)
- Tees / streetwear / blanks
- Activewear
- Sizes span kids through men's. Cash and card both taken. Walk-in retail.

### Social
No owner-verified handle found that is provably THIS exact store (a generic
"Hip Hop Sneaker" Instagram location tag exists but is not a confirmed
first-party business account). Per the verified-socials rule: OMITTED. None shown.

### Upsell intel (one line, for admin)
No e-commerce, no online inventory, no booking/ordering platform, no Linktree.
Clean upsell lane: a simple "what dropped this week" inventory feed or a
text-to-reserve-a-size flow, plus first-party social. They lean on nothing,
so the whole web presence is greenfield.

---

## Art-direction notes (locked kit honored)

- **Accent:** #E8552D  ·  **Base:** #111111  ·  **Paper:** warm bone #f4f1ea
- **Display:** Tanker (Fontshare)  ·  **Body:** Satoshi (Fontshare)
- **Archetype:** editorial-split, bold streetwear, drop ticker on #111.
- **Mood:** bold-street.
- **Hero:** editorial split. Left = oversized Tanker headline "COP THE HEAT ON
  THE BLOCK" with the word HEAT as an outlined (text-stroke accent) cut. Right
  = the floating Air Max grail shot on a dark studio ground with an accent
  screen-blend wash and a giant ghost "HHS" wordmark behind.
- **Signature interaction (mine alone this sprint):**
  1. **Hot-drops horizontal ticker** on #111 across the very top, auto-
     scrolling, pauses on hover, accent glow dots, seamless 50% loop (JS
     duplicates the track). Real drop copy (Bred 13s, AF1 restock, fitteds).
  2. **Sneaker hover that tilts / spins on the grid** in the Drops section.
     Each card tilts and scales on hover, and the assigned `.spin` cards run a
     360-degree spin keyframe on the shoe image. Honors the "tilt/spin on the
     grid" brief and is NOT a generic horizontal strip. Both respect
     prefers-reduced-motion.
- **Status pill:** live Open now / Closed now computed in America/New_York from
  the JS HOURS map, with "til 8 PM today" / "opens tomorrow at 9:30 AM"
  subtext, plus today's row highlighted in the hours list.
- **Furniture:** per-brand nav (rotated accent "H" mark + section links +
  persistent call CTA, collapses to a 46px round call icon under 880px),
  floating mobile tap-call FAB, keyless Google Maps embed (Ramos pattern),
  bysemaj.com footer credit styled into the dark footer with an accent
  underline.
- **No em dashes** in body copy (only the allowed `— A regular off South Main`
  review attribution). **12-hour time everywhere.**

---

## Images used (Pexels IDs, each appears exactly once)

| ID | Where | Alt-described as |
|----|-------|------------------|
| 2529148 | Hero | Floating Nike Air Max, upper + outsole, studio |
| 1124466 | Drop 01 | Black/white Nike on a city rooftop ledge |
| 1240892 | Drop 02 | Red canvas Converse on a sidewalk |
| 1598508 | Drop 03 | Top-down mustard Vans on dark grey |
| 1456736 | Drop 04 | Mint/grey knit Adidas runners |
| 6046183 | Drop 05 (grail wall) | Three white sneakers, neon/red/orange soles, boutique shelf |
| 9558590 | Drop 06 (fits/tees) | Person in plain oversized white tee |
| 5868722 | Street feature | Man with shopping bags + phone, red backdrop |
| 5239819 | Apparel / checkout band | Customer tapping phone on a card terminal |

No image repeats on the page. None collide with the used_images.json ledger
(all 9 IDs are new). Orchestrator should append these 9 IDs to
`.orchestrator/used_images.json` under `hip-hop-sneakers` / City of Orange.

---

## Self-verification performed

- Served at http://localhost:8080/hip-hop-sneakers/ and screenshotted via
  headed Chrome at 1280px and at 375px.
- All 9 image URLs return HTTP 200.
- Nav collapses cleanly to a 46px call icon at 375px, nothing overflows.
- Drop ticker scrolls and pauses on hover; grid tilt/spin works.
- Status pill computes from hours (showed "Closed now · opens ..." correctly at
  build time, which was after-hours).
- Maps embed URL is the keyless Ramos pattern; the endpoint returns
  "must be used in an iframe" when hit top-level (expected), and renders inside
  the page iframe.
- No em dashes in visible copy (one allowed cite attribution). 12-hour time
  throughout. No 24-hour time anywhere.
