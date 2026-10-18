---
name: NOVA BUILDING & DESIGN LLC
description: A backyard site plan on blueprint blue, where the visitor lays the patio by hand and texts Jeff for a free estimate.
colors:
  blueprint-blue: "#173a66"
  blueprint-blue-2: "#14335b"
  blueprint-blue-3: "#10294b"
  drafting-white: "#f2f6fb"
  drafting-white-2: "#bfd0e6"
  drafting-line: "rgba(196,218,244,.28)"
  drafting-line-soft: "rgba(196,218,244,.12)"
  lion-gold: "#d9cf45"
  lion-gold-hi: "#e8df63"
  on-gold: "#10264a"
  plan-cyan: "#7fd1ff"
  lawn-green: "#9fd4a6"
  error-coral: "#ffb4a8"
typography:
  display:
    fontFamily: "Avenir Next Condensed, Roboto Condensed, Arial Narrow, sans-serif-condensed, system-ui, sans-serif"
    fontSize: "clamp(46px, 13.2vw, 96px)"
    fontWeight: 800
    lineHeight: 0.98
    letterSpacing: "0.005em"
  headline:
    fontFamily: "Avenir Next Condensed, Roboto Condensed, Arial Narrow, sans-serif-condensed, system-ui, sans-serif"
    fontSize: "clamp(38px, 9vw, 64px)"
    fontWeight: 800
    lineHeight: 0.98
    letterSpacing: "0.005em"
  title:
    fontFamily: "Avenir Next Condensed, Roboto Condensed, Arial Narrow, sans-serif-condensed, system-ui, sans-serif"
    fontSize: "clamp(22px, 6vw, 28px)"
    fontWeight: 800
    lineHeight: 1.05
    letterSpacing: "0.01em"
  body:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Avenir Next Condensed, Roboto Condensed, Arial Narrow, sans-serif-condensed, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "0.04em"
rounded:
  control: "8px"
  button: "10px"
  sheet: "12px"
  round: "50%"
spacing:
  gutter: "20px"
  gutter-wide: "32px"
  gutter-desk: "48px"
  section: "56px"
  column-gap: "64px"
components:
  button-gold:
    backgroundColor: "{colors.lion-gold}"
    textColor: "{colors.on-gold}"
    typography: "{typography.label}"
    rounded: "{rounded.button}"
    padding: "0 18px"
    height: "56px"
  button-gold-hover:
    backgroundColor: "{colors.lion-gold-hi}"
    textColor: "{colors.on-gold}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.drafting-white}"
    typography: "{typography.label}"
    rounded: "{rounded.button}"
    padding: "0 18px"
    height: "56px"
  button-line-hover:
    textColor: "{colors.lion-gold-hi}"
  input-text:
    backgroundColor: "{colors.blueprint-blue-3}"
    textColor: "{colors.drafting-white}"
    typography: "{typography.body}"
    rounded: "{rounded.control}"
    padding: "12px 14px"
    height: "52px"
  chip:
    backgroundColor: "transparent"
    textColor: "{colors.drafting-white}"
    rounded: "{rounded.control}"
    padding: "0 15px"
    height: "46px"
  chip-checked:
    backgroundColor: "{colors.lion-gold}"
    textColor: "{colors.on-gold}"
  service-row:
    backgroundColor: "transparent"
    textColor: "{colors.drafting-white}"
    typography: "{typography.title}"
    padding: "12px 2px"
    height: "72px"
  service-row-arrow-hover:
    backgroundColor: "{colors.lion-gold}"
    textColor: "{colors.on-gold}"
    rounded: "{rounded.round}"
    size: "42px"
  form-sheet:
    backgroundColor: "{colors.blueprint-blue}"
    rounded: "{rounded.sheet}"
    padding: "22px 18px 24px"
---

# Design System: NOVA BUILDING & DESIGN LLC

## Overview

**Creative North Star: "Jeff's Backyard Plan"**

The whole site is a landscape site-plan sheet. Every surface is blueprint blue with white drafting linework, and the hero is a live plan drawing: a hatched house footprint, a door swing, a dashed patio outline, a fire-pit ring, stepping-stone outlines and a north arrow. The visitor drags a finger or mouse across it and pavers drop into the patio. "Building & Design" is something the visitor does on the page. Real stone colors show up only where something gets built. Everything else stays blue, white and line.

Density is phone-first and generous. Headlines are huge condensed caps, there is one promise line, and the actions are big tap targets. The page reads as a stack of sheets (blue, second blue, blue) separated by strips of drawn lawn whose tufts sway. A wavy color seam moves underneath them, so the lower sheet's color rises up under the grass. Lion gold is the trim color from the logo. Cyan is the drafting-pen color of interaction and only appears when something is hovered or focused.

The build rejects the contractor defaults it was made against: a stock patio photo as the hero, a gold-and-black banner, and grids of icon cards. Black grounds are out entirely. The darkest surface is still blue.

**Key Characteristics:**
- Blueprint-blue sheets only, with a drafting grid and white linework. No black or neutral-gray grounds.
- Condensed heavy uppercase for display, drawn from the system font stack to match the logo's "BUILDING & DESIGN".
- Lion gold as trim and as the single filled action. Plan cyan only for hover and focus.
- Signature motion: the visitor lays pavers in the hero, and lawn tufts sway with a moving seam between sections.
- With reduced motion, the plan shows as a finished still drawing.

## Colors

The palette is restrained: three tones of blueprint blue, drafting white for ink, one gold trim and one cyan interaction color. Stone and lawn colors live only inside the drawings.

### Primary
- **Lion Gold** (lion-gold): the logo's gold. Used for the filled Text button, the gold half of the headline, service-row icons, the step-number rings, the corner brackets on photo frames, the Facebook link's border, the wordmark "NOVA" and text selection. It is trim and the one filled button. It never fills a whole panel.
- **Lion Gold High** (lion-gold-hi): the hover state of gold, used on the filled button, the phone link and footer links.
- **Ink on Gold** (on-gold): a blue-black navy for text and icons on any gold fill. It is never plain black.

### Secondary
- **Plan Cyan** (plan-cyan): the interaction pen. Used for input and chip outlines on hover, focus outlines across the site (3px with a 3px offset), and the focus ring on the submit button. It never appears at rest.

### Tertiary
- **Lawn Green** (lawn-green): the color of the drawn grass tufts (stroked at about .48–.62 alpha) and the tint behind the form's sent confirmation. It belongs to the drawing, not to the interface.

### Neutral
- **Blueprint Blue** (blueprint-blue): the main sheet. Used for the body, the hero, Recent work, the closing section and the form card. It is also the theme color.
- **Second Sheet** (blueprint-blue-2): a slightly deeper blue for alternating sections (What we build, Get a free estimate), which reads as the next drawing in the set.
- **Footer Sheet** (blueprint-blue-3): the deepest blue. Used for the footer, the html overscroll ground and text-input wells.
- **Drafting White** (drafting-white): primary text and the plan's linework.
- **Secondary Ink** (drafting-white-2): body copy under headlines, the promise line, the plan hint, option labels and footer text.
- **Drafting Line / Soft Line** (drafting-line, drafting-line-soft): hairline rules between service rows, photo frames, the form card border, the resting borders of controls and the plan-box edges.

### Named Rules
**The Blue Ground Rule.** Every surface is one of the three blueprint blues. No black, near-black or neutral-gray ground, including the footer and overscroll.

**The Built-Things-Only Rule.** Stone, sand, bluestone and fire colors appear only where something is constructed in a drawing. Interface chrome never borrows them.

**The Hover-Only Accent Rule.** Plan cyan, and the gold fill on row arrows and the Facebook link, appear only in response to hover or focus. At rest, gold is limited to trim and the single filled Text button.

## Typography

**Display Font:** Avenir Next Condensed (with Roboto Condensed, Arial Narrow, sans-serif-condensed, system-ui)
**Body Font:** system-ui (with -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial)

**Character:** Tall, heavy condensed caps, like lettering on a contractor's plan set or the logo's "BUILDING & DESIGN", paired with the device's native sans for plain, friendly reading. Both come from the system stack. No webfont is loaded.

### Hierarchy
- **Display** (800, clamp(46px, 13.2vw, 96px), 0.98; clamp(72px, 6.6vw, 96px) at 1024px and up): the hero headline only, uppercase, balanced. One phrase is set in gold through an un-italicized emphasis.
- **Headline** (800, clamp(38px, 9vw, 64px), 0.98): section titles, uppercase.
- **Title** (800, clamp(22px, 6vw, 28px), 1.05): service-row names. Step titles use the same face at 24px/1.1.
- **Body** (400, 17px, 1.55): all reading copy. The promise and lede lines run 17–20px with a 30em max width.
- **Label** (800, 18px, 0.04em, uppercase): button text and form field labels and legends. Smaller plan annotations (12px/700, 0.12em tracking) caption the drawing itself.
- **Wordmark**: "NOVA" in the body face at 800 weight, 21px, with wide 0.32em tracking in gold, over "BUILDING & DESIGN LLC" in display caps at 11.5px. This mirrors the logo and is not a reusable type role.

### Named Rules
**The System Stack Rule.** Display and body both come from the system font stack. The condensed heavy caps come from Avenir Next Condensed, Roboto Condensed or Arial Narrow. Don't load webfonts.

**The Caps Are Display Rule.** Uppercase condensed type is for headlines, row names, button text, field labels and plan annotations. Reading copy is always sentence case in the body face.

## Layout

The layout is one column on phones and two-up on desktop. Content sits in a 1200px wrap. The header and hero widen to 1440px. Side padding is 20px on phones, 32px from 700px and 48px for the desktop header and hero. Sections use 56px top and 60px bottom padding. Section headlines sit 26px above their content.

- **First viewport (phone):** the lion and wordmark sit top-left and the phone number top-right. Below them come the huge headline, one promise line and two equal side-by-side buttons (a 1fr 1fr grid, max 440px wide). The live plan fills the rest, at clamp(300px, 46svh, 440px) tall.
- **First viewport (desktop, 1024px and up):** text on the left and the plan on the right (1fr / 1.1fr), spanning the full height (min(820px, 100svh − 72px)). The plan is split off by a single hairline.
- **Desktop grids:** service rows go to two columns with a 48px column gap. Photos become one tall lead image plus a stacked column. The estimate area goes to a .85fr / 1fr split and the closing section to 1.2fr / 1fr, both with a 64px gap. The footer goes to a flex row.
- **Section seams:** sections never meet edge to edge. A 56px lawn strip sits between each pair of sheets of different color.
- **Small phones (379px and below):** the wordmark tracking, phone size and button padding tighten so the header and the two buttons still fit on one line.
- **Tap targets:** at least 44px everywhere (links in the header and footer). Buttons are 56px, inputs 52px, chips 46px and service rows 72px.

### Named Rules
**The Phone Top-Right Rule.** On the first screen, the phone number appears only as the top-right header link. Email appears only in the footer. There is no sticky bottom bar or floating call button.

## Elevation & Depth

The system is flat, like paper. Depth comes from the change between sheet tones and from hairline borders, not from shadows. Only two shadows exist. The filled gold button carries a soft dark-navy drop, as if it sits on the plan. Pavers in the hero cast a lift shadow while they drop, and it fades to nothing as they settle.

### Shadow Vocabulary
- **Button rest** (`box-shadow: 0 6px 18px -8px rgba(5,14,30,.7)`): only on the filled gold button.
- **Stone lift** (canvas fill `rgba(6,18,38,.38–.4)`, offset 2–6px, scaled by the remaining lift): only on pieces mid-drop in the plan drawing.

### Named Rules
**The Flat Sheet Rule.** Cards, rows, photos and the form sit flat on the sheet, framed by hairlines. Depth means a deeper blue or a drawn object, never a floating panel.

## Shapes

The geometry is drafted. Rectangles have soft, practical corners: 8px for controls, 10px for buttons, 12px for the form sheet. Circles are reserved for plan-symbol elements: the service-row arrow and the numbered step rings. Photos sit in square hairline frames with 8px of inset and two gold corner brackets (14px, 2px stroke, top-left and bottom-right), like registration marks on a drawing. Inside the plan, dashed strokes mean "planned" (patio 7/5, fire ring and stones 4/4, door swing 3/3) and fills mean "built".

## Components

### Buttons
Buttons feel solid and decisive, like a stamped approval on the plan.
- **Shape:** gently rounded (10px), 56px tall, with a 2px gold border on every variant.
- **Gold (filled):** gold fill with navy-ink label text in condensed caps at 18px/800 and 0.04em tracking, plus an optional 19px stroke icon. The resting shadow is described under Elevation. Only one filled gold button is offered at each decision point.
- **Line:** transparent fill with drafting-white text and the gold border. On hover it takes a 12% gold tint and gold-high text.
- **Hover / Focus:** the gold button shifts to gold-high. The site-wide focus ring is 3px cyan with a 3px offset. The submit button also shows the cyan ring on hover. On press the button moves down 1px. Transitions run .2s on color and .12s on transform, and are removed under reduced motion.
- **Facebook link:** a 64px full-width bar with a gold border, an 8% gold tint and 20px caps. On hover it fills gold with navy ink.

### Chips
- **Style:** transparent with a 1.5px hairline border, 8px radius, 46px tall and body text at 600/15.5px. They act as checkboxes and radios.
- **State:** hover turns the border cyan. Checked fills gold with navy ink, and a checked chip still turns its border cyan on hover. Keyboard focus shows a cyan border plus a 2px cyan outline.

### Cards / Containers
- **Corner Style:** the form sheet uses a 12px radius. Photo frames have square corners.
- **Background:** the form sheet is blueprint blue placed on the second-sheet section, so it reads as a sheet laid on a sheet.
- **Shadow Strategy:** none (see Flat Sheet Rule).
- **Border:** a 1px drafting line.
- **Internal Padding:** 22px 18px 24px, with a 20px gap between fields.

### Inputs / Fields
- **Style:** a deepest-blue well with a 1.5px hairline border, 8px radius, 52px minimum height (104px for the textarea), body text at 17px and a gold caret.
- **Hover / Focus:** hover turns the border cyan. Focus adds a 2px cyan outline (1px offset) on top of the cyan border.
- **Error:** the border turns coral and a 15px coral message appears below the field. The message speaks to the person directly ("so Jeff knows who's texting").
- **Labels:** condensed caps at 18px. An "(optional)" marker sits inline in 14px sentence-case body text.

### Navigation
- **Header:** a single row, not sticky. The lion mark (42px, gold gradient through a mask) and the two-line wordmark sit left. The phone link sits right: a 17px gold handset icon and the number in 16px/700 drafting white, turning gold-high on hover. The header has no menu. The page is short and read top to bottom.
- **Footer:** deepest blue. The brand repeats with the address, followed by a link list (phone, email, Facebook, Free estimate) at 44px tall. Links turn gold-high and underline on hover.

### Service Row (signature)
A list of what Jeff builds, written as rows on a schedule rather than as cards. Each row is 72px tall and divided from the next by a hairline. It has a 34px gold line icon drawn in the same plan language (paver bond, wall courses, sun, stones), the service name in title caps, and a 42px circular arrow at the end.
- **Hover / Focus:** only the arrow changes. It fills gold with navy ink. The row itself gets no background, outline or shadow. On keyboard focus the arrow also takes the cyan ring.

### Numbered Steps
A three-step ordered list. Each step's counter sits in a 44px gold hairline circle and is set in 22px display numerals, followed by a 24px caps title and secondary-ink body text.

### Hero Plan Drawing (signature)
A live canvas site plan. It shows a drafting grid (16px minor lines, 80px major), a hatched house footprint along the top labeled HOUSE, a door with a dashed swing, a squircle paver patio with a dashed outline over stippled base, a fire-pit ring, bluestone stepping stones out to the lawn, a north arrow and lawn tufts everywhere else.
- **Laying:** the pointer lays any paver within 26px of it. Each stone drops and settles over 380ms, scaling down from 1.28× with a fading lift shadow. On touch, a gold ring marks the laying radius. Pavers are laid in random-length running bond, row by row from the house outward. Stone colors are warm tans, sand joints, gray block for the fire ring and blue-gray bluestone.
- **Idle:** 2.6s after the last touch, the patio starts laying itself (about 11s for the whole patio). Once the ring is complete the fire lights, and its embers drift up and dodge the pointer. The finished patio holds for 6.5s, fades over 900ms and starts again.
- **Lawn:** tufts sway on two sine waves and part away from the pointer on a damped spring.
- **Reduced motion:** every piece is drawn already laid with the fire lit. The visitor gets one finished still frame and no animation loop.

### Lawn Strip (signature)
A 56px canvas divider between sections of different blue. The upper sheet's color fills the strip. A wavy seam, made of two sine waves of 5px and 3px moving in opposite directions, is filled with the lower sheet's color, so the next sheet rises up under the grass. Tufts are planted along the seam every 7px and sway and part under the pointer, the same way as in the hero. With reduced motion, the strip is painted once as a still frame. Animation runs only while the strip is on screen.

## Do's and Don'ts

### Do:
- **Do** keep every ground on blueprint blue, second sheet or footer sheet, and switch between them only with a lawn strip.
- **Do** set headlines, row names, buttons and field labels in the condensed heavy caps from the system stack (Avenir Next Condensed / Roboto Condensed / Arial Narrow) at weight 800.
- **Do** keep lion gold to trim plus the one filled button per decision, with navy ink on any gold fill.
- **Do** outline form controls in plan cyan on hover and focus, and use the 3px cyan focus ring everywhere else.
- **Do** draw new illustration as plan symbols: dashed means planned, filled stone means built, white linework on the drafting grid.
- **Do** give every animated drawing a finished still frame under reduced motion, and run animation only while it is on screen.

### Don't:
- **Don't** use black, near-black or neutral-gray grounds anywhere, including the footer.
- **Don't** put the phone number anywhere on the first screen except the top-right header link. Don't show email outside the footer, and don't add a sticky bottom bar or floating call button.
- **Don't** highlight a whole service row on hover. Only its arrow fills gold.
- **Don't** show cyan, or gold fills on rows and links, at rest. The accent appears on hover and focus only.
- **Don't** use a stock patio photo as the hero, a gold-and-black banner, or icon-card grids for services.
- **Don't** load webfonts, and don't set reading copy in caps.
- **Don't** use stone, sand or fire colors in interface chrome.
