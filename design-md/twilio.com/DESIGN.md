---
version: alpha
name: Twilio
description: "Light interface measured from twilio.com: Buffalo type with Whitney SSm, vivid blue accents, flat surfaces and 50px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000D25"
  on-background: "#000D25"
  on-surface-variant: "#7E869C"
  overlay: "#EF223A33"
  primary: "#1866EE"
  on-primary: "#FFFFFF"
  inverse-surface: "#000000"
  secondary: "#DB132A"
  tertiary: "#030B5D"
  error: "#EF223A"
typography:
  display-hero:
    fontFamily: Buffalo
    fontSize: 72px
    fontWeight: 400
    lineHeight: 0.58
    letterSpacing: 0.035em
  headline-display:
    fontFamily: Whitney SSm
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.18
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Whitney SSm
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Whitney SSm
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Whitney SSm
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.29
  title-lg:
    fontFamily: Whitney SSm
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.6
  body-md:
    fontFamily: Whitney SSm
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
  body-lg:
    fontFamily: Whitney SSm
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.56
  body-sm:
    fontFamily: Whitney SSm
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  caption:
    fontFamily: Whitney SSm
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Whitney SSm
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: Whitney SSm
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  label-sm:
    fontFamily: Whitney SSm
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.75
  code:
    fontFamily: Twilio Sans Mono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Whitney SSm
    fontSize: 34px
    fontWeight: 700
    lineHeight: 1.18
    letterSpacing: -0.03em
  headline-md-mobile:
    fontFamily: Whitney SSm
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.29
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 20px
  lg: 50px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 75px
  margin: 100px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 6px 24px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.caption}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "#CACDD8"
---

# Twilio Design System

## Overview

Twilio describes itself as: “Build amazing customer experiences on the Twilio platform with APIs for SMS, RCS, voice, and email, plus conversational AI for smarter engagement, and identity verification for trust.” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#000D25)** text, and **Vivid Blue (#1866EE)** as the main accent.

Type is set in **Buffalo** and **Whitney SSm**, with **Twilio Sans Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 50px.

Measured from [twilio.com](https://www.twilio.com/en-us) on October 21, 2026 at 1440×900 and 390×844 from 408 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`.
- **Deep Blue (#000D25):** Primary text and headings, seen 8 times. Token `on-surface`.
- **Blue (#7E869C):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Vivid Red 20% (#EF223A33):** Translucent fill for cards and controls, seen 5 times. Token `overlay`.
- **Vivid Blue (#1866EE):** Primary buttons and calls to action, seen 10 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#000000):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Vivid Red (#DB132A):** Brand color in the logo, seen 16 times. Token `secondary`.
- **Deep Indigo (#030B5D):** Accent, seen 3 times. Token `tertiary`.
- **Vivid Red (#EF223A):** Errors and destructive states, seen 17 times. Token `error`.

## Typography

**Buffalo**, **Whitney SSm** and **Twilio Sans Mono** (monospace) share the interface. Fallback stack: `Buffalo`. Other loaded fonts: whitney-book, whitney-light, whitney-medium.

- **display-hero:** Buffalo 72px at weight 400, line height 0.58, tracking 0.035em. Oversized hero statements.
- **headline-display:** Whitney SSm 56px at weight 700, line height 1.18, tracking -0.03em (34px on mobile). Page title (h1).
- **headline-lg:** Whitney SSm 48px at weight 700, line height 1.25, tracking -0.03em. Section headings (h2).
- **headline-md:** Whitney SSm 40px at weight 700, line height 1.3, tracking -0.02em (28px on mobile). Sub-section headings.
- **headline-sm:** Whitney SSm 28px at weight 400, line height 1.29. Card and feature titles.
- **title-lg:** Whitney SSm 20px at weight 700, line height 1.6. Small titles.
- **body-md:** Whitney SSm 16px at weight 400, line height 1.75. Body text.
- **body-lg:** Whitney SSm 18px at weight 600, line height 1.56. Lead paragraphs.
- **body-sm:** Whitney SSm 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** Whitney SSm 12px at weight 400, line height 1.5. Captions and fine print.
- **label-lg:** Whitney SSm 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** Whitney SSm 14px at weight 600, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Whitney SSm 12px at weight 500, line height 1.75. Small labels and badges.
- **code:** Twilio Sans Mono 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing follows a 4px grid: 93% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 75px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 100px on each side of full-width sections.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights:

- `rgb(255, 255, 255) 0px 0px 0px 2px inset`
- `rgb(24, 102, 238) 0px 0px 0px 2px inset`
- `rgb(221, 224, 230) 0px -1px 0px 0px inset`

A few raised panels add a soft drop shadow: `rgba(18, 28, 45, 0.15) 0px 10px 37.5px 0px`.

## Shapes

Most elements use 50px corners. Measured radii, most used first:

- **lg (50px):** 84 elements.
- **sm (4px):** 38 elements.
- **md (20px):** 16 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #1866EE fill, #FFFFFF text, 16px/500, 50px radius, padding 6px 24px.
- **button-ghost (“English”):** transparent fill, #000D25 text, 12px/400, padding 0px.
- **link:** transparent fill, #CACDD8 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #000D25, #7E869C.
- Do reserve #1866EE for primary actions and key highlights.
- Do set headlines in Buffalo with tight tracking (-0.03em).
- Do keep spacing on the 4px grid.
- Do use 50px corners on most elements; larger surfaces also use 4px and 20px.
- Don't use #7E869C for body text; it reaches 3.6:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings.
- Don't introduce new font families beyond Buffalo, Whitney SSm and Twilio Sans Mono.
- Don't use #1866EE for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.15s, 0.18s. Longer ambient animations run 0.7s, 1s.

- **Easing:** `ease-in-out`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/twilio.com/), the free DESIGN.md generator.
