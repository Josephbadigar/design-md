---
version: alpha
name: shadcn/ui
description: "Dark monochrome interface measured from ui.shadcn.com: Geist type, tonal surfaces and 18px corners."
colors:
  background: "#0A0A0A"
  surface: "#0A0A0A"
  on-surface: "#FAFAFA"
  on-background: "#FAFAFA"
  on-surface-variant: "#A1A1A1"
  surface-container-low: "#171717"
  surface-container: "#262626"
  overlay: "#FFFFFF13"
  overlay-strong: "#26262680"
  outline: "#FFFFFF1A"
  primary: "#E5E5E5"
  on-primary: "#171717"
  warning: "#F0B100"
  error: "#FF6467"
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
    rounded: 10px
    padding: 0px 10px
    height: 31px
  button-primary-hover:
    backgroundColor: "#E5E5E5CC"
  button-secondary:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 26px
    padding: 0px 12px
    height: 36px
  button-secondary-hover:
    backgroundColor: "#2F2F2F"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 10px
    padding: 8px 16px 8px 12px
    height: 32px
  button-ghost:
    typography: "{typography.label-md}"
    rounded: 10px
    padding: 8px 16px 8px 12px
  card:
    typography: "{typography.label-md}"
    rounded: 10px
    padding: 8px 16px 8px 12px
  link:
    textColor: "{colors.on-surface-variant}"
---

# shadcn/ui Design System

## Overview

shadcn/ui describes itself as: “Composable, accessible components with thoughtful defaults. Build your own component library with code you can customize, extend, and make your own.” The interface is dark, built on **Near Black (#0A0A0A)** with **Snow (#FAFAFA)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Geist**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 18px.

Measured from [ui.shadcn.com](https://ui.shadcn.com/) on October 21, 2026 at 1440×900 and 390×844 from 330 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Near Black (#0A0A0A):** Page background, seen 1 time. Token `background`.
- **Snow (#FAFAFA):** Primary text and headings, seen 70 times. Token `on-surface`.
- **Gray (#A1A1A1):** Secondary text, seen 34 times. Token `on-surface-variant`.
- **Charcoal (#171717):** Raised areas one step from the page, seen 18 times. Token `surface-container-low`.
- **Graphite (#262626):** Cards and panels, seen 8 times. Token `surface-container`.
- **White 8% (#FFFFFF13):** Translucent fill for cards and controls, seen 8 times. Token `overlay`.
- **Graphite 50% (#26262680):** Stronger translucent fill, seen 4 times. Token `overlay-strong`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 9 times. Token `outline`.
- **Mist (#E5E5E5):** Primary buttons and calls to action, seen 15 times. Token `primary`.
- **Charcoal (#171717):** Text and icons on primary. Token `on-primary`.
- **Vivid Amber (#F0B100):** Warnings and highlights, seen 1 time. Token `warning`.
- **Red (#FF6467):** Errors and destructive states, seen 1 time. Token `error`.

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

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.984998 -0.00000956654 0.0000230074 / 0.1) 0px 0px 0px 1px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, lab(98.26 0 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, lab(98.26 0 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.

## Shapes

Most elements use 18px corners. Measured radii, most used first:

- **sm (18px):** 140 elements.
- **md (19.6px):** 80 elements.
- **xl (24px):** 78 elements.
- **xs (8px):** 40 elements.
- **lg (22px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“New”):** #E5E5E5 fill, #171717 text, 12.8px/500, 10px radius, padding 0px 10px.
- **button-primary-hover:** background #E5E5E5CC, text #171717 on hover.
- **button-secondary (“View Components”):** #262626 fill, #FAFAFA text, 14px/500, 26px radius, padding 0px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-secondary-hover:** background #2F2F2F, text #FAFAFA on hover.
- **button-outline (“Search documentation...”):** #171717 fill, #FAFAFA text, 14px/500, 10px radius, padding 8px 16px 8px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-ghost (“Search documentation...”):** transparent fill, 14px/500, 10px radius, padding 8px 16px 8px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **card:** transparent fill, 14px/500, 10px radius, padding 8px 16px 8px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **link:** transparent fill, #A1A1A1 text, padding 0px.

## Do's and Don'ts

- Do use #0A0A0A for the page and lift surfaces in small steps: #171717, #262626.
- Do keep text in 2 levels: #FAFAFA, #A1A1A1.
- Do let contrast carry emphasis; primary actions use #E5E5E5 on #0A0A0A.
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

Generated by [Sitepeel](https://sitepeel.dev/design-md/ui.shadcn.com/), the free DESIGN.md generator.
