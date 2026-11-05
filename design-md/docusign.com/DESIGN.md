---
version: alpha
name: Docusign
description: "Light interface measured from docusign.com: DSIndigo type, deep violet accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#130032"
  on-background: "#130032"
  on-surface-strong: "#000000"
  on-surface-variant: "#4E4065"
  surface-container-low: "#F8F3F0"
  surface-container: "#EDE9E4"
  overlay: "#13003240"
  overlay-strong: "#1300321A"
  outline: "#CBC2FF"
  outline-variant: "#13003226"
  primary: "#26065D"
  on-primary: "#FFFFFF"
  secondary: "#4C00FF"
  tertiary: "#2C0578"
typography:
  headline-display:
    fontFamily: DSIndigo
    fontSize: 80px
    fontWeight: 300
    lineHeight: 1.08
    letterSpacing: -0.019em
  headline-lg:
    fontFamily: DSIndigo
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.013em
  headline-md:
    fontFamily: DSIndigo
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.24
    letterSpacing: -0.01em
  body-md:
    fontFamily: DSIndigo
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: DSIndigo
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: DSIndigo
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.014em
  caption:
    fontFamily: DSIndigo
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.017em
  label-lg:
    fontFamily: DSIndigo
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.013em
  label-md:
    fontFamily: DSIndigo
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.014em
  label-sm:
    fontFamily: DSIndigo
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0.067em
  headline-display-mobile:
    fontFamily: DSIndigo
    fontSize: 58px
    fontWeight: 300
    lineHeight: 1.08
    letterSpacing: -0.022em
  headline-lg-mobile:
    fontFamily: DSIndigo
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.24
    letterSpacing: -0.008em
  headline-md-mobile:
    fontFamily: DSIndigo
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.24
rounded:
  sm: 4px
  md: 8px
  lg: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 24px
  xl: 40px
  section: 96px
  margin: 80px
  container: 600px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 12px 16px
    height: 61px
  button-primary-hover:
    backgroundColor: "#291B45"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 45px
  button-secondary-hover:
    backgroundColor: "#4000CC"
  button-tertiary:
    backgroundColor: "{colors.outline}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 45px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.caption}"
    rounded: "{rounded.sm}"
    padding: 0px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 24px 16px 8px 16px
  link:
    textColor: "{colors.on-surface}"
---

# Docusign Design System

## Overview

Docusign describes itself as: “Create, commit to, and manage your agreements all in one platform with Docusign IAM. Electronically sign for free.” The interface is light, built on **White (#FFFFFF)** with **Deep Violet (#130032)** text, and **Deep Violet (#26065D)** as the main accent.

Type is set in **DSIndigo**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [docusign.com](https://www.docusign.com/) on November 4, 2026 at 1440×900 and 390×844 from 429 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #4C00FF, #26065D, #FF5252.

- **White (#FFFFFF):** Page background, seen 16 times. Token `background`.
- **Deep Violet (#130032):** Primary text and headings, seen 66 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 2 times. Token `on-surface-strong`.
- **Dark Violet (#4E4065):** Secondary text, seen 12 times. Token `on-surface-variant`.
- **Warm Snow (#F8F3F0):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Warm Mist (#EDE9E4):** Cards and panels, seen 1 time. Token `surface-container`.
- **Deep Violet 25% (#13003240):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Deep Violet 10% (#1300321A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Pale Indigo (#CBC2FF):** Borders and dividers, seen 1 time. Token `outline`.
- **Deep Violet 15% (#13003226):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Deep Violet (#26065D):** Brand color in the header, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Violet (#4C00FF):** Secondary buttons, seen 52 times. Token `secondary`.
- **Dark Violet (#2C0578):** Accent in logos and imagery. Token `tertiary`.

## Typography

**DSIndigo** carries the whole interface. Fallback stack: `DSIndigo, Helvetica, Arial, sans-serif`.

- **headline-display:** DSIndigo 80px at weight 300, line height 1.08, tracking -0.019em (58px on mobile). Page title (h1).
- **headline-lg:** DSIndigo 40px at weight 400, line height 1.2, tracking -0.013em (30px on mobile). Section headings (h2).
- **headline-md:** DSIndigo 24px at weight 500, line height 1.24, tracking -0.01em (18px on mobile). Sub-section headings.
- **body-md:** DSIndigo 16px at weight 400. Body text.
- **body-lg:** DSIndigo 18px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** DSIndigo 14px at weight 400, line height 1.5, tracking 0.014em. Secondary and small text.
- **caption:** DSIndigo 12px at weight 400, line height 1.5, tracking 0.017em. Captions and fine print.
- **label-lg:** DSIndigo 16px at weight 500, line height 1.5, tracking 0.013em. Large buttons and tabs.
- **label-md:** DSIndigo 14px at weight 500, line height 1.5, tracking 0.014em. Buttons, navigation and labels.
- **label-sm:** DSIndigo 12px at weight 600, line height 1.5, tracking 0.067em, uppercase. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (90% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 16px, lg 24px, xl 40px.
- **Sections:** 96px vertical padding between major sections.
- **Container:** content is capped at 600px.
- **Page margin:** 80px on each side of full-width sections.
- **Breakpoints:** 400px, 425px, 426px, 550px, 600px, 896px, 1219px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F8F3F0 → #EDE9E4) and hairline rings:

- `rgba(19, 0, 50, 0.15) 0px 0px 0px 1px inset`
- `rgb(255, 255, 255) 0px 0px 0px 1px inset`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 288 elements.
- **md (8px):** 88 elements.
- **lg (16px):** 16 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #130032 fill, #FFFFFF text, 16px/500, 0px 8px 8px 0px radius, padding 12px 16px.
- **button-primary-hover:** background #291B45, text #FFFFFF on hover.
- **button-secondary (“TRY FOR FREE”):** #4C00FF fill, #FFFFFF text, 14px/600, 8px radius, padding 12px 16px.
- **button-secondary-hover:** background #4000CC, text #FFFFFF on hover.
- **button-tertiary (“Featured”):** #CBC2FF fill, #130032 text, 14px/500, 8px radius, padding 12px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 1px inset`.
- **button-ghost (“Search”):** transparent fill, #FFFFFF text, 12px/500, 4px radius, padding 0px.
- **input-field:** #FFFFFF fill, #130032 text, 18px/400, 8px 0px 0px 8px radius, padding 24px 16px 8px 16px, border 1px solid #13003226.
- **link:** transparent fill, #130032 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8F3F0, #EDE9E4.
- Do keep text in 3 levels: #130032, #000000, #4E4065.
- Do use #26065D as the brand accent: header, logo and key highlights.
- Do set headlines in DSIndigo with tight tracking (-0.019em).
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 8px and 16px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond DSIndigo.
- Don't use #26065D for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.1s, 0.2s, 0.3s.

- **Easing:** `ease-in-out`, `cubic-bezier(0.33, 0, 0.67, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/docusign.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
