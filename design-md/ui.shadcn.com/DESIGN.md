---
version: alpha
name: shadcn/ui
description: "Light monochrome interface measured from ui.shadcn.com: Geist type, tonal surfaces and 18px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0A0A0A"
  on-background: "#0A0A0A"
  on-surface-strong: "#000000"
  on-surface-variant: "#171717"
  on-surface-muted: "#737373"
  surface-container-low: "#FAFAFA"
  surface-container: "#F5F5F5"
  surface-container-high: "#E5E5E5E6"
  overlay: "#E5E5E580"
  overlay-strong: "#F5F5F580"
  outline: "#E5E5E5"
  primary: "#171717"
  on-primary: "#FAFAFA"
  secondary: "#F0B100"
typography:
  headline-display:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.05em
  body-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: 0.05em
  headline-display-mobile:
    fontFamily: Geist
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.025em
rounded:
  xs: 8px
  sm: 18px
  md: 19.6px
  lg: 22px
  xl: 24px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 20px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 10px 0px 12px
    height: 32px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: 26px
    padding: 0px 12px
    height: 36px
  button-ghost:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: 10px
    padding: 8px 16px 8px 12px
    height: 32px
  card:
    typography: "{typography.label-md}"
    rounded: 10px
    padding: 8px 16px 8px 12px
  link:
    textColor: "{colors.on-surface-muted}"
---

# shadcn/ui Design System

## Overview

shadcn/ui describes itself as: “Composable, accessible components with thoughtful defaults. Build your own component library with code you can customize, extend, and make your own.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#0A0A0A)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Geist**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 18px.

Measured from [ui.shadcn.com](https://ui.shadcn.com/) on October 29, 2026 at 1440×900 and 390×844 from 330 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 24 times. Token `background`, CSS `--color-white`.
- **Near Black (#0A0A0A):** Primary text and headings, seen 62 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 12 times. Token `on-surface-strong`.
- **Charcoal (#171717):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Slate (#737373):** Muted text and metadata, seen 34 times. Token `on-surface-muted`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F5F5F5):** Cards and panels, seen 9 times. Token `surface-container`.
- **Mist 90% (#E5E5E5E6):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Mist 50% (#E5E5E580):** Translucent fill for cards and controls, seen 8 times. Token `overlay`.
- **Snow 50% (#F5F5F580):** Stronger translucent fill, seen 4 times. Token `overlay-strong`.
- **Mist (#E5E5E5):** Borders and dividers, seen 9 times. Token `outline`.
- **Charcoal (#171717):** Primary buttons and calls to action, seen 21 times. Token `primary`.
- **Snow (#FAFAFA):** Text and icons on primary. Token `on-primary`.
- **Vivid Amber (#F0B100):** Accent, seen 1 time. Token `secondary`.

## Typography

**Geist** carries the whole interface. Fallback stack: `Geist, Geist Fallback`.

- **headline-display:** Geist 48px at weight 600, line height 1.1, tracking -0.05em (30px on mobile). Page title (h1).
- **body-md:** Geist 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Geist 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-md:** Geist 14px at weight 500, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Geist 12px at weight 500, line height 1.33, tracking 0.05em, uppercase. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 65% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 20px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 560px, 1400px, 1600px, 1800px, 1900px, 2000px, 2200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.145 -0.00000143796 0.00000340492 / 0.05) 0px 0px 0px 1px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, lab(2.75381 0 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, lab(2.75381 0 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.

## Shapes

Most elements use 18px corners. Measured radii, most used first:

- **sm (18px):** 140 elements.
- **md (19.6px):** 80 elements.
- **xl (24px):** 78 elements.
- **xs (8px):** 40 elements.
- **lg (22px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Button”):** #171717 fill, #FAFAFA text, 14px/500, 18px radius, padding 0px 10px 0px 12px.
- **button-outline (“View Components”):** #F5F5F5 fill, #171717 text, 14px/500, 26px radius, padding 0px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-ghost (“Search documentation...”):** #F5F5F5 fill, #000000 text, 14px/500, 10px radius, padding 8px 16px 8px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **card:** transparent fill, 14px/500, 10px radius, padding 8px 16px 8px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **link:** transparent fill, #737373 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA, #F5F5F5, #E5E5E5E6.
- Do keep text in 4 levels: #0A0A0A, #000000, #171717, #737373.
- Do let contrast carry emphasis; primary actions use #171717 on #FFFFFF.
- Do set headlines in Geist with tight tracking (-0.05em).
- Do reuse the measured spacing steps (8px, 10px, 20px).
- Do use 18px corners on most elements; larger surfaces also use 19.6px, 24px and 8px.
- Don't introduce new font families beyond Geist.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ui.shadcn.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
