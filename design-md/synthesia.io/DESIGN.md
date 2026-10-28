---
version: alpha
name: Synthesia
description: "Light interface measured from synthesia.io: Basiersquare Webfont type, dark red accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#363636"
  on-background: "#363636"
  on-surface-strong: "#090B22"
  on-surface-variant: "#68686A"
  surface-container-low: "#F7F7F7"
  overlay: "#0D0F2C66"
  overlay-strong: "#0D0F2C33"
  outline: "#FFFFFF33"
  outline-variant: "#DADADD"
  primary: "#771A0D"
  on-primary: "#FFFFFF"
  secondary: "#3E57DA"
  warning: "#FFF4B6"
typography:
  headline-display:
    fontFamily: Basiersquare Webfont
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.065em
  headline-lg:
    fontFamily: Basiersquare Webfont
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.055em
  headline-md:
    fontFamily: Basiersquare Webfont
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.05em
  headline-sm:
    fontFamily: Basiersquare Webfont
    fontSize: 34px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.045em
  title-lg:
    fontFamily: Basiersquare Webfont
    fontSize: 26px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.04em
  body-md:
    fontFamily: Basiersquare Webfont
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Basiersquare Webfont
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.015em
  body-sm:
    fontFamily: Basiersquare Webfont
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: -0.005em
  caption:
    fontFamily: Basiersquare Webfont
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Basiersquare Webfont
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.004em
  label-sm:
    fontFamily: Basiersquare Webfont
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Basiersquare Webfont
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.05em
  headline-md-mobile:
    fontFamily: Basiersquare Webfont
    fontSize: 34px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.045em
rounded:
  sm: 8px
  md: 10px
  lg: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 18px
  xl: 40px
  gutter: 8px
  section: 96px
  margin: 40px
  container: 1216px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 38px
  button-primary-hover:
    backgroundColor: "#0D0F2CCC"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#98989C"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
  link:
    textColor: "{colors.on-surface}"
---

# Synthesia Design System

## Overview

Synthesia describes itself as: “Official Synthesia site. The AI video platform trusted by 90%+ of the Fortune 100 to communicate, train, and upskill teams in 140+ languages.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#363636)** text, and **Dark Red (#771A0D)** as the main accent.

Type is set in **Basiersquare Webfont**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [synthesia.io](https://www.synthesia.io/) on October 21, 2026 at 1440×900 and 390×844 from 343 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 18 times. Token `background`, CSS `--_semantic---text-inverted`.
- **Graphite (#363636):** Primary text and headings, seen 62 times. Token `on-surface`, CSS `--_semantic---text-secondary`.
- **Deep Indigo (#090B22):** Headings and emphasis, seen 25 times. Token `on-surface-strong`, CSS `--_semantic---text-primary`.
- **Slate (#68686A):** Secondary text, seen 7 times. Token `on-surface-variant`, CSS `--_semantic---text-link-tertiary-active`.
- **Snow (#F7F7F7):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Deep Indigo 40% (#0D0F2C66):** Translucent fill for cards and controls, seen 8 times. Token `overlay`, CSS `--base-dark-opacity-40`.
- **Deep Indigo 20% (#0D0F2C33):** Stronger translucent fill, seen 1 time. Token `overlay-strong`, CSS `--base-dark-opacity-20`.
- **White 20% (#FFFFFF33):** Borders and dividers, seen 8 times. Token `outline`.
- **Silver (#DADADD):** Secondary dividers, seen 5 times. Token `outline-variant`, CSS `--_semantic---border-caption`.
- **Dark Red (#771A0D):** Brand accent (CSS variable). Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Indigo (#3E57DA):** Accent, seen 7 times. Token `secondary`.
- **Light Amber (#FFF4B6):** Warnings and highlights, seen 2 times. Token `warning`, CSS `--yellow-300`.

## Typography

**Basiersquare Webfont** carries the whole interface. Fallback stack: `Basiersquare Webfont, sans-serif`.

- **headline-display:** Basiersquare Webfont 72px at weight 500, line height 1, tracking -0.065em (44px on mobile). Page title (h1).
- **headline-lg:** Basiersquare Webfont 56px at weight 500, line height 1, tracking -0.055em. Section headings (h2).
- **headline-md:** Basiersquare Webfont 44px at weight 500, line height 1.05, tracking -0.05em (34px on mobile). Sub-section headings.
- **headline-sm:** Basiersquare Webfont 34px at weight 500, line height 1.12, tracking -0.045em. Card and feature titles.
- **title-lg:** Basiersquare Webfont 26px at weight 500, line height 1.15, tracking -0.04em. Small titles.
- **body-md:** Basiersquare Webfont 16px at weight 400, line height 1.38, tracking -0.01em. Body text.
- **body-lg:** Basiersquare Webfont 18px at weight 500, line height 1.33, tracking -0.015em. Lead paragraphs.
- **body-sm:** Basiersquare Webfont 14px at weight 400, line height 1.43, tracking -0.005em. Secondary and small text.
- **caption:** Basiersquare Webfont 12px at weight 400, line height 1.5. Captions and fine print.
- **label-md:** Basiersquare Webfont 16px at weight 500, line height 1.5, tracking -0.004em. Buttons, navigation and labels.
- **label-sm:** Basiersquare Webfont 12px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (81% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 18px, xl 40px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1216px.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 479px, 764px, 767px, 768px, 991px, 992px, 1030px, 1035px, 1096px, 1180px, 1440px, 1920px, 2560px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F7F7F7):

- `rgb(218, 218, 221) 0px 0px 0px 1px inset`
- `rgb(227, 235, 255) 0px 0px 0px 3px`
- `rgba(255, 255, 255, 0.4) 0px 0px 0px 1px inset`

A few raised panels add a soft drop shadow: `rgba(16, 24, 40, 0.08) 0px 2px 10px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 84 elements.
- **md (10px):** 76 elements.
- **sm (8px):** 24 elements.
- **lg (12px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #090B22 fill, #FFFFFF text, 14px/500, 8px radius, padding 8px 16px, shadow `rgba(16, 24, 40, 0.08) 0px 2px 10px 0px`.
- **button-primary-hover:** background #0D0F2CCC, text #FFFFFF on hover.
- **button-ghost (“Video”):** transparent fill, #68686A text, 16px/400, padding 0px.
- **input-field (“Hey, Luke here! Ready to create ”):** #F7F7F7 fill, #98989C text, 16px/400, 8px radius, padding 12px 16px, border 1px solid #DADADD.
- **link:** transparent fill, #363636 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F7F7.
- Do keep text in 3 levels: #363636, #090B22, #68686A.
- Do use #771A0D as the brand accent: header, logo and key highlights.
- Do set headlines in Basiersquare Webfont with tight tracking (-0.065em).
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do make buttons and chips fully rounded (9999px); most other elements use 10px corners.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Basiersquare Webfont.
- Don't use #771A0D for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s.

- **Easing:** `ease`, `ease-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/synthesia.io/), the free DESIGN.md generator.
