---
name: Stratman Family Dentistry
description: Tucson Courtyard — familiar, calm, and grounded in the real practice.
colors:
  crimson: "#bc1647"
  crimson-hover: "#9d113b"
  blue: "#173e59"
  ink: "#183c56"
  muted: "#35546a"
  ivory: "#f5f1e8"
  sand: "#ebe6db"
  line: "#c9c7bd"
  white: "#ffffff"
typography:
  display:
    fontFamily: "Manrope, sans-serif"
    fontSize: "clamp(60px, 5.28vw, 84px)"
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: "-0.039em"
  headline:
    fontFamily: "Manrope, sans-serif"
    fontSize: "clamp(32px, 3.4vw, 52px)"
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "-0.035em"
  body:
    fontFamily: "Manrope, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "Manrope, sans-serif"
    fontSize: "14px"
    fontWeight: 700
    lineHeight: 1.5
rounded:
  square: "0px"
spacing:
  mobile-gutter: "24px"
  section: "112px"
  mobile-section: "64px"
components:
  button-primary:
    backgroundColor: "{colors.crimson}"
    textColor: "{colors.white}"
    rounded: "{rounded.square}"
    padding: "15px 23px"
  button-primary-hover:
    backgroundColor: "{colors.crimson-hover}"
  button-light:
    backgroundColor: "{colors.ivory}"
    textColor: "{colors.blue}"
    rounded: "{rounded.square}"
    padding: "15px 23px"
---

# Design System: Stratman Family Dentistry

## Overview

**Creative North Star: "Tucson Courtyard"**

Calm architectural framing, broad readable typography, and real practice photography make the site feel like a familiar local place. Bryan chose this direction on November 2, 2026. The direction is selected; the completed homepage still awaits his review.

**Key Characteristics:**
- Warm ivory surfaces and deep blue foundations.
- Straight edges, deliberate whitespace, and thin structural rules.
- Original Stratman logo and authentic practice imagery.

## Colors

Crimson marks the primary action. Deep blue anchors major sections, while ink and muted blue carry readable text on ivory and sand. White is reserved for text on strong fills. Keep the original logo colors intact.

**The Action Rule.** Use crimson for meaningful actions and small interactive details, not decorative blocks.

## Typography

Manrope is self-hosted at regular, medium, and bold weights. Medium-weight display type supplies scale without a heavy promotional tone. Body text uses generous line spacing and comfortable measures. Mobile body text is 16px; the display adapts to 31–50px, with a 30px fallback at the narrowest breakpoint.

**The Heading Rule.** Capitalize The First Letter Of Every Word in visible headings and prominent labels. Use normal sentence case in body prose.

## Layout

Containers share a maximum width of 1440px and fluid gutters. Desktop editorial sections use two columns with 7–10% gaps; office information follows a consistent Oracle-first order. Below 700px, content stacks in reading order with 24px gutters (20px below 370px).

The sticky header is 128px on large screens, 104px below 1150px, and 80px on mobile. Anchor offsets leave breathing room beneath it. The mobile office action stays at the bottom, with footer clearance and safe-area padding.

## Elevation & Depth

Depth comes from overlapping ivory planes and contrasting sections, not shadows or gradients. Photo crops and stepped framing belong to the selected homepage composition; later pages should use the same visual grammar without mechanically repeating that hero.

## Shapes

Buttons, photos, panels, and rules have square corners. The existing logo retains its original proportions. Thin separators organize service and office information without enclosing each item in a card.

## Components

Primary buttons are crimson with white text, a 54px minimum height, and optional line arrows. Light buttons sit on blue sections. Text links remain quieter, underline on hover, and have generous click areas. Focus uses a visible crimson ring, switching to white on dark sections.

The service list uses native disclosure controls with plus/minus states. Desktop navigation becomes a native disclosure menu below 900px; selecting a link closes it. Escape restores focus to the menu trigger. Movement is restrained to short color and arrow transitions; reduced-motion preferences disable animation and smooth scrolling.

## Do's and Don'ts

- Do preserve the authentic Stratman logo and real practice photographs.
- Do use whitespace and alignment to make office choice easy.
- Do keep text readable across desktop and mobile.
- Don't add decorative shadows, gradients, or rounded card grids.
- Don't substitute generated people, offices, or clinical results for this practice.


## Local Image Backplate — November 6, 2026

Bryan reviewed this refinement and authorized committing and pushing it for the hosted preview on November 6. This is not whole-site client approval. The older square-corner description above reflects the original release, while the current local draft already has rounded media, panels and controls from the authorized November 6 refinement. This pass preserves those existing choices.

Use one static pale-blue (`--blue-light`, #d7e2e9) rounded backplate behind the Oracle waiting-room image in “Come In. Feel At Ease.” The separate solid block occupies 66% of the image group's width and 64% of its height, exposed at the lower left. Reserve 24px at the left and 28px below the image on desktop, reduced to 16px/20px at 700px and below. Plate corners are 32/32/32/72px, reduced to 24/24/24/48px on phones. Keep the image's existing rounded crop and caption outside the layered composition. The hero stands alone, avoiding repetition on every photo.

This is deliberate flat framing authorized by Bryan's updated dental guidance, not a shadow. Use an empty CSS pseudo-element, pointer-events:none and an isolated stacking context; it has no reading-order or keyboard target. No new motion, photo, copy, color token, dependency or interaction is introduced. Preserve existing reduced-motion behavior.

References inspected: Website Starter's offset-image-backplate.png and staggered-image-composition.png, November 6, 2026. Only their layering principle is used; their people, content and palette are not client assets. Verification: docs/review/2026-11-06-backplates/review.md.


## Local Hero Spacing Follow-Up — November 6, 2026

Bryan authorized bringing the hero photograph closer to the text first. Above 1150px, use .94fr/1.06fr columns with a 4% gap, including wide desktops. This shifts the photo start approximately 69px left at a 1440px viewport, enlarging the image without changing heading size or photo corner/crop rules. Preserve existing columns and gaps at tablet/phone breakpoints. After native desktop and phone inspection, retain the hero without another backplate: the tighter relationship supplies the needed balance. Only the Oracle image has the accent plate. Build and diff whitespace checks passed; Bryan approved this version for the hosted preview on November 6.
