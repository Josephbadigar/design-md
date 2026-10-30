---
version: alpha
name: Twilio
description: "Dark interface measured from twilio.com: Buffalo type with Whitney SSm, vivid blue accents, tonal surfaces and 50px corners."
colors:
  background: "#000D25"
  surface: "#000D25"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#565B73"
  surface-container-low: "#0D122B"
  overlay: "#140C23A6"
  primary: "#1866EE"
  on-primary: "#FFFFFF"
  secondary: "#DB132A"
  tertiary: "#7688C2"
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
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Whitney SSm
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.29
  headline-sm:
    fontFamily: Whitney SSm
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.6
  body-md:
    fontFamily: Whitney SSm
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Whitney SSm
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.56
  body-sm:
    fontFamily: Whitney-Book
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.75
  label-lg:
    fontFamily: Whitney SSm
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.75
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
  headline-lg-mobile:
    fontFamily: Whitney SSm
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.29
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 10px
  lg: 20px
  xl: 50px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 48px
  gutter: 8px
  section: 111px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.xl}"
    padding: 6px 24px
    height: 36px
  button-primary-hover:
    backgroundColor: "#0E3E92"
  button-outline:
    backgroundColor: "{colors.overlay}"
    textColor: "#000000"
    typography: "{typography.label-lg}"
    padding: 0px
    height: 68px
  button-outline-hover:
    backgroundColor: "#140C23E6"
  button-ghost:
    textColor: "{colors.background}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "#CACDD8"
---

# Twilio Design System

## Overview

Twilio describes itself as: “Build amazing customer experiences on the Twilio platform with APIs for SMS, RCS, voice, and email, plus conversational AI for smarter engagement, and identity verification for trust.” The interface is dark, built on **Deep Blue (#000D25)** with **White (#FFFFFF)** text, and **Vivid Blue (#1866EE)** as the main accent.

Type is set in **Buffalo** and **Whitney SSm**, with **Twilio Sans Mono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 50px.

Measured from [twilio.com/en-us](https://www.twilio.com/en-us) (the site sent our reader to its /en-us version; twilio.com was asked for) on October 29, 2026 at 1440×900 and 390×844 from 392 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Deep Blue (#000D25):** Page background, seen 1 time. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 54 times. Token `on-surface`.
- **Indigo (#565B73):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Deep Indigo (#0D122B):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Deep Violet 65% (#140C23A6):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Vivid Blue (#1866EE):** Primary buttons and calls to action, seen 11 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Red (#DB132A):** Accent in the logo, seen 1 time. Token `secondary`.
- **Blue (#7688C2):** Accent in text, fills and borders, seen 8 times. Token `tertiary`.
- **Vivid Red (#EF223A):** Errors and destructive states, seen 15 times. Token `error`.

## Typography

**Buffalo**, **Whitney SSm**, **Whitney-Book** and **Twilio Sans Mono** (monospace) share the interface. Fallback stack: `Buffalo`.

- **display-hero:** Buffalo 72px at weight 400, line height 0.58, tracking 0.035em. Oversized hero statements.
- **headline-display:** Whitney SSm 56px at weight 700, line height 1.18, tracking -0.03em (34px on mobile). Page title (h1).
- **headline-lg:** Whitney SSm 40px at weight 700, line height 1.3, tracking -0.02em (28px on mobile). Section headings (h2).
- **headline-md:** Whitney SSm 28px at weight 400, line height 1.29. Sub-section headings.
- **headline-sm:** Whitney SSm 20px at weight 700, line height 1.6. Card and feature titles.
- **body-md:** Whitney SSm 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Whitney SSm 18px at weight 600, line height 1.56. Lead paragraphs.
- **body-sm:** Whitney-Book 12px at weight 400, line height 1.75. Secondary and small text.
- **label-lg:** Whitney SSm 16px at weight 400, line height 1.75. Large buttons and tabs.
- **label-md:** Whitney SSm 14px at weight 600, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Whitney SSm 12px at weight 500, line height 1.75. Small labels and badges.
- **code:** Twilio Sans Mono 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 48px.
- **Sections:** 111px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#0D122B):

- `rgb(255, 255, 255) 0px 0px 0px 2px inset`
- `rgb(24, 102, 238) 0px 0px 0px 2px inset`
- `rgb(221, 224, 230) 0px -1px 0px 0px inset`

A few raised panels add a soft drop shadow: `rgba(18, 28, 45, 0.15) 0px 10px 37.5px 0px`.

## Shapes

Most elements use 50px corners. Measured radii, most used first:

- **xl (50px):** 68 elements.
- **sm (4px):** 38 elements.
- **lg (20px):** 12 elements.
- **md (10px):** 4 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #1866EE fill, #FFFFFF text, 16px/500, 50px radius, padding 6px 24px.
- **button-primary-hover:** background #0E3E92, text #FFFFFF on hover.
- **button-outline (“Play full Halloween video”):** #140C23A6 fill, #000000 text, 16px/400, 50% radius, padding 0px, border 1px solid #FFFFFFCC.
- **button-outline-hover:** background #140C23E6, text #000000 on hover.
- **button-ghost (“English”):** transparent fill, #000D25 text, 12px/400, padding 0px.
- **link:** transparent fill, #CACDD8 text, padding 0px.

## Do's and Don'ts

- Do use #000D25 for the page and lift surfaces in small steps: #0D122B.
- Do keep text in 2 levels: #FFFFFF, #565B73.
- Do reserve #1866EE for primary actions and key highlights.
- Do set headlines in Buffalo with tight tracking (-0.03em).
- Do keep spacing on the 4px grid.
- Do use 50px corners on most elements; larger surfaces also use 4px, 20px and 10px.
- Don't use #565B73 for body text; it reaches 2.90:1 on #000D25. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Buffalo, Whitney SSm, Whitney-Book and Twilio Sans Mono.
- Don't use #1866EE for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.18s. Longer ambient animations run 0.7s, 1s.

- **Easing:** `ease-in-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/twilio.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
