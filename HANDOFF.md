# NOVA BUILDING & DESIGN LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/novaBuildingDesign/ · **Repo:** https://github.com/10elizabethbell/novaBuildingDesign · **Built:** 2026-10-18 from Muse brief 2026-10-18 (found via "CONTRACTORS NJ/PA Conncted" FB group ad)

## What's built
- One page, `index.html`, single file (~430 KB with three embedded photos). Phone first; desktop puts the plan beside the headline.
- **World: a backyard site plan on blueprint blue.** Drafting grid, a hatched house footprint with a door swing, a dashed patio outline, a fire pit, stepping stones, north arrow. Lion gold from their logo is the trim and the one filled button. Headings use condensed heavy caps (Avenir Next Condensed on iPhone, Roboto Condensed on Android), echoing the logo's "BUILDING & DESIGN".
- **Signature element: you lay the patio.** Drag a finger, or move the mouse, across the plan and pavers drop into place in real stone colors with a little settle. Nobody touching? It lays itself row by row from the house out (about 11 s), then the fire-pit ring and the bluestone stepping stones. When the ring is done the fire lights and embers rise and dodge your finger. It holds about 6.5 s, then resets. Lawn tufts sway and part under the pointer. The same lawn strips sit between sections, where the lower section's color rises under the grass along a moving, uneven seam. Vertical drags on the plan lay stones instead of scrolling (`touch-action:none`, pull-to-refresh off).
- Sections: header (lion + NOVA, 732-328-0507 top-right as tap-to-call), hero ("Your backyard, built to last." + Text us / Free estimate), What we build (6 rows from the ad; each row opens a pre-filled text naming that service), Recent work (3 photos + "See more of our work on Facebook"), Get a free estimate (3 steps + a form that composes a text to Jeff), close (Jeff named as who you'll talk to, the 10% seasonal cleanup offer, area and hours), footer (address, phone, email, Facebook).
- Contact: `sms:+17323280507?&body=…` everywhere (the ad says call **or text**), `tel:` in the header top-right and the footer (once per screen). Email only in the footer.
- Favicon and home-screen icon: the lion mark from their logo, gold on blueprint blue. `og.jpg` (1200×630) for the Facebook link preview.

## Assumptions I made
- **The three photos are their work.** They came from their own Wix site (uploads under their account), not from Muse. The kitchen and tool-belt images on that site look like stock, so I left them out.
- **Colors:** the logo is an olive-to-gold gradient lion. I carried the gold as trim and chose blueprint blue (#173a66) as the ground, since the world is a plan drawing and black grounds are out.
- **Voice:** "we" for the crew, with Jeff named as the person you text. The ad speaks as "we".
- **Services:** only the six from the 2026-10-18 ad, as Muse advised. Not the Wix template list, and not the flyer's "outdoor kitchens / carpentry", which I couldn't fetch to verify.
- **"Free estimate":** their Wix site says "Call me today for your free estimate." The steps say "We walk the space with you", which is inferred.
- **"Since 2015"** (Wix) is in the footer. I left out the ad's "over 15 years of experience" because the two claims conflict.
- **Offer line** "Right now: 10% off seasonal cleanup." comes from the 2026-10-18 ad (plain text, not a button). It's time-bound, so remove it when the promo ends.
- **Audience:** I treated it as general homeowners and kept the motion. If Jeff's customers skew 50+, switch to the still-picture rules in `older-audience.md`.

## Placeholders and gaps
- No reviews anywhere, so none on the page.
- No license or insurance numbers published, so none claimed.
- No business Facebook page. The "See more of our work" link goes to Jeff's **personal** profile (profile.php?id=502752112). Confirm he's fine with that, or get a business page.
- Only three job photos, one of them 640×480 (the backyard; slightly soft at phone 2x). No before/after pairs.
- The promo flyer from the FB post couldn't be fetched (Facebook blocks it).
- Shipped photos are base64 inside `index.html`. Provenance for those is in `src-assets/*.json` sidecars (local only, gitignored); the icons and `og.jpg` carry it embedded.
- Fonts are system condensed faces; a desktop Windows visitor gets Arial Narrow.

## Questions for the owner
- Are the three Wix photos his jobs? Can he send 6–10 more, especially patios, retaining walls and before/afters?
- Which services matter most this season, and are outdoor kitchens or carpentry worth listing?
- Towns he covers (the page only says "Central New Jersey").
- Is he licensed/insured (NJ HIC number)? Worth showing if so.
- OK to show the street address (207 Elizabeth St) in the footer?
- When does the 10% seasonal cleanup offer end?

## Ideas not built (yours to pick)
- **Runner-up world: dusk patio with fire-pit embers.** Their night fire-pit photo as the mood; a warm-lit paver field you light up with your finger, embers as the ambient motion.
- Before/after slider once pairs exist (plan drawing on one side, finished photo on the other would suit this world).
- Let the visitor pick a paver color blend in the hero before laying.
- A real `book.html` with the same plan motion.
- Swap the system condensed face for a self-hosted condensed face that matches the logo more closely, if Ellie wants it over the system stack.

## Review record
- Impeccable finish reviewer, 2 rounds (the unattended ceiling). Round 1: 7 fixes, all applied. Round 2: the fire-pit icon redraw was scored resolved; the desktop photo grid was scored partial (columns ended 18px apart). I fixed the grid after round 2 by solving the column widths (`1fr calc((100% - 38.67px)/3)`) and measured equal bottoms at 1440 and 1100. The reviewer didn't re-score that last fix, and it never gave a ship verdict.
- Detector ignores I added (`.impeccable/config.json`): `broken-image` (lazy data-block images), `overused-font roboto` (system stack, house style), `cramped-padding` (list rule above padded rows). `design-system-*` one-offs the documenter left out of DESIGN.md (1 radius, 2 colors, 8 font sizes), and `all-caps-body` scoped to `index.html`: it only fires on two one-line labels (the drag hint and the Facebook link, 32 and 37 characters). Remove that ignore if you'd rather set those two in sentence case.
- Impeccable modes beyond the finish review (audit, harden, clarify, adapt, optimize) were done in-thread, not as separate runs: contrast checked by value, form harden (fields read by id, validation tested), overflow at 360/390/520/1440, text-body encoding tested.

## Not verified
- Real-device touch on iPhone/Android, inside Facebook's in-app browser.
- The SMS handoff on a real phone (the body is URL-encoded and decodes correctly in tests).
- Frame rate on older phones (phone draws ~400 lawn tufts plus ~300 pavers baked into a layer).
