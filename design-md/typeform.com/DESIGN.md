---
version: alpha
name: Typeform
description: "Dark monochrome interface measured from typeform.com: Tobias type with Twklausanne 350, flat surfaces and pill-shaped controls."
colors:
  background: "#2A222B"
  surface: "#2A222B"
  on-surface: "#FAF9FB"
  on-background: "#FAF9FB"
  on-surface-variant: "#ECCFFA"
  primary: "#FAF9FB"
  on-primary: "#2A222B"
  secondary: "#A057BB"
typography:
  headline-display:
    fontFamily: Tobias
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.013em
  headline-lg:
    fontFamily: Twklausanne 350
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.1
  headline-md:
    fontFamily: Tobias
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1
  headline-sm:
    fontFamily: Twklausanne 500
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: -0.01em
  title-lg:
    fontFamily: Twklausanne 400
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: Twklausanne 500
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-sm:
    fontFamily: Twklausanne 600
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.2
  label-md:
    fontFamily: Twklausanne 400
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
  label-sm:
    fontFamily: Twklausanne 400
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1
rounded:
  sm: 12px
  md: 12.5px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 12px 20px
    height: 40px
  button-primary-hover:
    backgroundColor: "#EEECEE"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 8px 20px
    height: 40px
  button-outline-hover:
    backgroundColor: "#3E3040"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 24px
  link:
    textColor: "{colors.primary}"
---

# Typeform Design System

## Overview

Typeform describes itself as: “Build AI-powered forms that get 3.5x more data — then trigger automated workflows to enrich leads, follow up, and grow revenue. No code. Start free.” The interface is dark, built on **Cool Graphite (#2A222B)** with **Snow (#FAF9FB)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Tobias** and **Twklausanne 350**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [typeform.com](https://www.typeform.com/) on November 4, 2026 at 1440×900 and 390×844 from 280 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 6 roles, plus gradient stops #A057BB.

- **Cool Graphite (#2A222B):** Page background, seen 12 times. Token `background`, CSS `--tokens--tag--tag-bg-active`.
- **Snow (#FAF9FB):** Primary text and headings, seen 37 times. Token `on-surface`, CSS `--tokens--button--primary-text`.
- **Pale Violet (#ECCFFA):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Snow (#FAF9FB):** Primary buttons and calls to action, seen 78 times. Token `primary`, CSS `--tokens--button--primary-text`.
- **Cool Graphite (#2A222B):** Text and icons on primary. Token `on-primary`.
- **Purple (#A057BB):** Accent in text, fills and borders, seen 4 times. Token `secondary`.

## Typography

**Tobias**, **Twklausanne 350**, **Twklausanne 500**, **Twklausanne 400** and **Twklausanne 600** share the interface. Fallback stack: `Tobias, Times New Roman, sans-serif`. Other loaded fonts: Inter.

- **headline-display:** Tobias 80px at weight 400, line height 1, tracking -0.013em. Page title (h1).
- **headline-lg:** Twklausanne 350 48px at weight 400, line height 1.1. Section headings (h2).
- **headline-md:** Tobias 28px at weight 400, line height 1. Sub-section headings.
- **headline-sm:** Twklausanne 500 24px at weight 400, line height 1.15, tracking -0.01em. Card and feature titles.
- **title-lg:** Twklausanne 400 20px at weight 400, line height 1.3. Small titles.
- **body-md:** Twklausanne 500 16px at weight 400, line height 1. Body text.
- **body-sm:** Twklausanne 600 14px at weight 400, line height 1.2. Secondary and small text.
- **label-md:** Twklausanne 400 16px at weight 400, line height 1.3. Buttons, navigation and labels.
- **label-sm:** Twklausanne 400 13px at weight 400, line height 1, uppercase. Small labels and badges.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 425px, 426px, 479px, 500px, 550px, 600px, 767px, 768px, 769px, 890px, 896px, 897px, 991px, 1023px, 1024px, 1280px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(173, 158, 177, 0.07) -10px -10px 20px -10px inset, rgb(37, 28, 39) 10px 10px 20px -9px inset`
- `rgb(42, 34, 43) 0px 0px 0px 1px inset`

A few raised panels add a soft drop shadow: `rgb(182, 109, 213) 0px 0px 15px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 68 elements.
- **sm (12px):** 48 elements.
- **md (12.5px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #FAF9FB fill, #2A222B text, 16px/400, 12px radius, padding 12px 20px.
- **button-primary-hover:** background #EEECEE, text #2A222B on hover.
- **button-outline (“Contact sales”):** #2A222B fill, #FAF9FB text, 16px/400, 12px radius, padding 8px 20px, border 1px solid #FAF9FB.
- **button-outline-hover:** background #3E3040, text #FAF9FB on hover.
- **button-ghost (“Save your spot”):** transparent fill, #FAF9FB text, 16px/400, padding 0px.
- **card:** #2A222B fill, #FAF9FB text, 16px/400, 12px radius, padding 24px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(173, 158, 177, 0.07) -10px -10px 20px -10px inset, rgb(37, 28, 39) 10px 10px 20px -9px inset`.
- **link:** transparent fill, #FAF9FB text, padding 0px.

## Do's and Don'ts

- Do use #2A222B for the page.
- Do keep text in 2 levels: #FAF9FB, #ECCFFA.
- Do let contrast carry emphasis; primary actions use #FAF9FB on #2A222B.
- Do set headlines in Tobias with tight tracking (-0.013em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 12px corners.
- Don't use heavy drop shadows; keep depth to hairline rings.
- Don't introduce new font families beyond Tobias, Twklausanne 350, Twklausanne 500, Twklausanne 400 and Twklausanne 600.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.25s, 0.35s.

- **Easing:** `ease`, `ease-out`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/typeform.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
