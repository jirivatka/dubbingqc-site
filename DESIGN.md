---
name: Dubbing QC
description: The line-up at the head of a delivery master. Seven bars, a slate, burnt-in timecode, then the dub lined up against the original.
colors:
  ground: "#0b0d0c"
  panel: "#131614"
  rule: "#2a2e2b"
  ink: "#ecece6"
  muted: "#a9ada7"
  bar-white: "#dcdcd5"
  bar-yellow: "#c4b43c"
  bar-cyan: "#19aab5"
  bar-green: "#1f9d5c"
  bar-magenta: "#b8378f"
  bar-red: "#cf3a2e"
  bar-blue: "#2f48c4"
  flag: "#f5d000"
  gap: "#e0483b"
  button-green: "#127a52"
  button-green-hover: "#0e6845"
typography:
  display:
    fontFamily: "Slate, Arial Narrow, sans-serif"
    fontSize: "clamp(52px, 5.6vw, 84px)"
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: "0.005em"
  headline:
    fontFamily: "Slate, Arial Narrow, sans-serif"
    fontSize: "clamp(44px, 6vw, 76px)"
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: "0.005em"
  title:
    fontFamily: "Slate, Arial Narrow, sans-serif"
    fontSize: "28px"
    fontWeight: 800
    lineHeight: 0.95
  body:
    fontFamily: "Body, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Slate, Arial Narrow, sans-serif"
    fontSize: "16px"
    fontWeight: 800
    letterSpacing: "0.08em"
  timecode:
    fontFamily: "TC, ui-monospace, monospace"
    fontSize: "14px"
    fontWeight: 500
    letterSpacing: "0.01em"
rounded:
  none: "0px"
  dial: "50%"
spacing:
  xs: "10px"
  sm: "14px"
  md: "28px"
  lg: "48px"
  section: "104px"
  gutter: "32px"
components:
  button-go:
    backgroundColor: "{colors.button-green}"
    textColor: "#ffffff"
    rounded: "{rounded.none}"
    padding: "16px 22px"
    typography: "{typography.title}"
  button-go-hover:
    backgroundColor: "{colors.button-green-hover}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "16px 22px"
  button-line-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.ground}"
  slate:
    backgroundColor: "{colors.ground}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "40px 44px 36px"
    width: "700px"
  burnin:
    backgroundColor: "#000000"
    textColor: "#ffffff"
    padding: "6px 14px"
  lane:
    backgroundColor: "{colors.panel}"
    height: "92px"
  switch-active:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.ground}"
---

# Design System: Dubbing QC

## Overview

**Creative North Star: "The Line-Up"**

The page is the head of a delivery master: colour bars, a slate, burnt-in timecode, then the dub lined up against the original. Everything is built from that material. The ground is near-black, the corners are square, the display type is a condensed character-generator face in capitals, and every measurement is set in a mono. There is no dark-SaaS hero with a screenshot and no feature-card grid; sections are separated by rules, PLUGE strips and tonal panels, not boxes.

Each of the seven 75% bars owns one check family as a named colour role. The yellow flag from the app icon is reserved for findings. Dropped audio is drawn as an honest dashed gap rather than a hidden defect.

**Key Characteristics:**
- Black ground, square corners, 1px rules and 2px ink borders; depth by tonal panel, not shadow.
- Seven bars = seven families; colour carries meaning, never decoration.
- Caps condensed display, proportional humanist body, tabular mono for time and measurements.
- One clock drives timecode, playhead and flag highlight.

## Colors

Broadcast 75% bars on a black ground; neutrals are warm-green-tinted blacks and paper-grey ink.

### Primary
- **Bar Green** (#1f9d5c): the brand bar; the Sync family, "ok" figures in the ledger, the free-trial heading.
- **Go Green** (#127a52, hover #0e6845): button fill only, chosen so white text clears contrast. It is not the bar green and is not interchangeable with it.

### Secondary (check-family bars)
- **Bar White** (#dcdcd5): Lines, and the waveform fill.
- **Bar Yellow** (#c4b43c): Laughs and walla.
- **Bar Cyan** (#19aab5): Reverb and pan.
- **Bar Magenta** (#b8378f): Voice.
- **Bar Red** (#cf3a2e): Signal.
- **Bar Blue** (#2f48c4): Files.

### Tertiary
- **Finding Flag** (#f5d000): means "finding" and nothing else: flags, shifted-sync dashes, selection, focus ring.
- **Dropped Red** (#e0483b): the dashed gap box for dropped audio.

### Neutral
- **Ground** (#0b0d0c): page, slate, PLUGE black steps.
- **Panel** (#131614): alternating sections, lanes, FAQ.
- **Rule** (#2a2e2b): all hairlines and field dividers.
- **Ink** (#ecece6): text, strong borders, switch fill.
- **Muted** (#a9ada7): secondary copy, labels, timecode captions.

### Named Rules
**The One Flag Rule.** Yellow #f5d000 marks a finding. Never use it for buttons, links, decoration or brand emphasis.
**The Bar Owns Its Family Rule.** A family's colour appears on its bar, its contents marker and nowhere that implies another family.
**The Contrast Green Rule.** Text on green uses #127a52; the lighter bar green is for fills without text weight.

## Typography

**Display Font:** Slate (Sofia Sans Extra Condensed, variable 100-900; fallback Arial Narrow)
**Body Font:** Body (Sofia Sans, variable; fallback system-ui)
**Label/Mono Font:** TC (JetBrains Mono 500; fallback ui-monospace)

**Character:** A character-generator caption face against a plain reading face, with a mono that reads as burnt-in timecode.

### Hierarchy
- **Display** (800, clamp(52px, 5.6vw, 84px), 0.95): the slate h1, caps; 44px under 560px.
- **Headline** (800, clamp(44px, 6vw, 76px), 0.95): h2 per section, caps, balanced wrap.
- **Title** (800, 28px; 30-34px for family and rate headings; 28px FAQ summary): h3, caps.
- **Body** (400, 18px/1.55; 17px under 560px): copy, 52-70ch measure; promise 21px.
- **Label** (800, 16px, 0.08em, caps): lane labels, field keys; buttons are 22px caps at 0.04em.
- **Timecode** (500, 13-16px, tabular numerals): flags, captions, amounts' sub-lines; burn-in is 34px.

### Named Rules
**The Mono Means Measured Rule.** Anything that is a time, length or measurement is mono with tabular numerals; prose never is.
**The Caps Are Display Only Rule.** Capitals belong to the Slate face; body copy stays sentence case.

## Layout

Wrapper max 1200px with 32px gutters (20px under 560px); the header is full-width at 64px tall and sticky. Vertical rhythm: sections pad 104px (tracks 88/96, FAQ 96/104), stacked in alternating ground and panel. Content blocks sit on 1.65fr/1fr (proof), 1fr/1fr (export, pair) and 3-up (countdown) grids with 28-48px gaps, separated by 1px rules, not boxes.

The line-up is a single CSS grid: seven equal bars at min 640px height with the slate overlaid top-left (700px wide, 48px margin) and the burn-in timecode bottom-right, then a 34px PLUGE strip.

Responsive: at 980px nav links drop to the button only, bars shrink to 104px tall with vertical-rl labels, the slate moves below the PLUGE and loses its border, and proof, export, pair, family and countdown grids collapse to one column; rate rows keep price beside title with copy on its own row. At 560px body is 17px, h1 44px, slate fields stack, flag labels hide and a legend list appears instead.

## Elevation & Depth

Flat. Depth is tonal (ground, panel, #1c1f1d dial) and by 1px rules. The only shadows are on screenshots and the lightbox image (`0 24px 60px rgba(0,0,0,.55)`, lightbox `0 30px 90px rgba(0,0,0,.6)`), plus a yellow glow on the hot flag (`drop-shadow(0 2px 10px rgba(245,208,0,.55))`).

### Named Rules
**The Flat Unless Evidence Rule.** Shadows exist only to lift a real screenshot off black or to light an active finding.

## Shapes

Square. Radius is 0 everywhere except the countdown rings (50%). Borders are 1px rule, 2px ink for strong edges (slate, switch, section lead rules). The flag is a pennant clipped with `polygon(0 0,100% 0,78% 50%,100% 100%,0 100%)` on a 3px pole. The PLUGE strip alternates seven steps with ground. The FAQ chevron is a rotated 12px corner border.

## Components

### Buttons
- **Shape:** square, 2px border in currentColor, caps Slate 22px, padding 16px 22px, optional 20px SVG icon at 10px gap.
- **Go (primary):** fill #127a52, white text; hover #0e6845 and 1px lift.
- **Line (secondary):** ink border and text; hover fills ink with ground text.
- **Focus:** 3px yellow outline, 3px offset, on links, buttons and summaries.
- Header button shrinks to 18px / 10px 14px.

### Bars and PLUGE
Seven links, label (Slate 26px caps) over a mono 14px value, bottom-aligned, ground text (white on the blue and dark bars); hover brightness 1.12. PLUGE: seven 34px steps alternating ground and the bar colours; the footer repeats it at 14px.

### Slate
Ground box, 2px ink border, h1, promise, a three-up key/value field row between rules (Slate 20px values, 15px muted keys, 22px dividers), then the actions row.

### Switch
Two or three caps buttons in a 2px ink frame; the pressed one inverts to ink fill with ground text (Original / Dub / Both).

### Lanes, flags, gaps
Lane: 92px panel with a muted caps label and a #cfd3cc waveform. Gap: 2px dashed red box with 8% red fill. Shift: 2px dashed yellow box. Flag: yellow pennant with a mono 13px label on a ground chip; flips left near the edge; hot flags glow. Playhead: 2px white line. In single-view modes the unselected lane drops to 0.28 opacity and findings to 0.2.

### Ledger and rate rows
Rule-separated rows under a 2px ink top border. Ledger figure is Slate 46px (green for ok). Rate row is a 1.1fr / 2fr / auto grid; amount Slate 48px right-aligned with a mono 13px sub-line; the free-trial heading is bar green.

### Family map
Each family is a 220px heading column with an 18x42px bar-colour chip, and a numbered list (54px mono index, 600 title, 16px muted description) behind a 1px rule.

### Countdown dial
4:3 #1c1f1d field with a crosshair of 2px #3b403c lines, two concentric rings (#d9dbd4 at 62%, #6b706c at 74%) and a Slate numeral at clamp(90px, 11vw, 150px).

### FAQ
Native details; Slate 28px caps summary, 2px ink top rule, rotated-corner chevron that flips when open.

### Lightbox
Fixed overlay rgba(5,6,6,.94), zoom-out cursor, image up to 96vw / 84vh, centred 15px caption.

### Motion
One clock only: a 24 s loop drives the burn-in timecode, the playhead and the hot-flag state, running only while the line-up or tracks are on screen and the tab is visible. Transitions use `cubic-bezier(.16, 1, .3, 1)` at 0.2-0.35s (chevron 0.25s). Reduced motion: smooth scroll off, all transitions removed, and the clock is frozen on a fixed frame (10:43.2).

## Do's and Don'ts

### Do:
- **Do** give every check family its own bar colour and use it only for that family.
- **Do** set times and measurements in the TC mono with tabular numerals.
- **Do** draw dropped audio as a dashed red gap and shifted sync as a dashed yellow box.
- **Do** keep text on green at #127a52 with white.
- **Do** keep the focus ring yellow, 3px, offset 3px.

### Don't:
- **Don't** use #f5d000 for anything but a finding (and focus/selection, which are the same flag).
- **Don't** add rounded corners, cards, or glow outside the hot flag.
- **Don't** swap the button green for the bar green or the reverse.
- **Don't** run a second animation clock or any motion that survives reduced-motion.

Not canonized: none carried forward as rules; the sub-14px mono flag labels (13px) are legibility-tight and are recorded as a build value, not a floor for new surfaces.
