---
version: alpha
name: Next.js
description: "Dark monochrome interface measured from nextjs.org: GeistSans type, tonal surfaces and 4px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#EDEDED"
  on-background: "#EDEDED"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#A1A1A1"
  on-surface-muted: "#8F8F8F"
  surface-container-low: "#0A0A0A"
  surface-container: "#292929"
  outline: "#454545"
  outline-variant: "#292929"
  primary: "#EDEDED"
  on-primary: "#000000"
  secondary: "#0057FF"
typography:
  headline-display:
    fontFamily: GeistSans
    fontSize: 64px
    fontWeight: 450
    lineHeight: 1
    letterSpacing: -0.06em
  headline-lg:
    fontFamily: GeistSans
    fontSize: 56px
    fontWeight: 450
    lineHeight: 1
    letterSpacing: -0.06em
  body-md:
    fontFamily: GeistSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.65
  body-lg:
    fontFamily: GeistSans
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: GeistSans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: GeistSans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: GeistSans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.65
  headline-display-mobile:
    fontFamily: GeistSans
    fontSize: 40px
    fontWeight: 450
    lineHeight: 1.2
    letterSpacing: -0.05em
  headline-lg-mobile:
    fontFamily: GeistSans
    fontSize: 32px
    fontWeight: 450
    lineHeight: 1.25
    letterSpacing: -0.04em
rounded:
  sm: 2px
  md: 4px
  lg: 6px
  xl: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 32px
  section: 144px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 0px 6px 0px 14px
    height: 32px
  button-outline-hover:
    backgroundColor: "#1A1A1A"
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 0px 12px
  link:
    textColor: "{colors.primary}"
---

# Next.js Design System

## Overview

Next.js describes itself as: “Next.js by Vercel is the full-stack React framework for the web.” The interface is dark, built on **Near Black (#000000)** with **Mist (#EDEDED)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **GeistSans**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [nextjs.org](https://nextjs.org/) on October 21, 2026 at 1440×900 and 390×844 from 312 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **Near Black (#000000):** Page background, seen 9 times. Token `background`, CSS `--ds-background-200`.
- **Mist (#EDEDED):** Primary text and headings, seen 49 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 6 times. Token `on-surface-strong`.
- **Gray (#A1A1A1):** Secondary text, seen 54 times. Token `on-surface-variant`.
- **Gray (#8F8F8F):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Near Black (#0A0A0A):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Graphite (#292929):** Cards and panels, seen 5 times. Token `surface-container`, CSS `--color-gray-300`.
- **Graphite (#454545):** Borders and dividers, seen 5 times. Token `outline`, CSS `--color-gray-500`.
- **Graphite (#292929):** Secondary dividers, seen 3 times. Token `outline-variant`, CSS `--color-gray-300`.
- **Mist (#EDEDED):** Primary actions (the main text color; the palette is monochrome), seen 57 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0057FF):** Most used accent color, seen 8 times. Token `secondary`, CSS `--color-next-blue`.

## Typography

**GeistSans** carries the whole interface. Fallback stack: `GeistSans, GeistSans Fallback`. Other loaded fonts: Geist Mono, GeistSans Fallback.

- **headline-display:** GeistSans 64px at weight 450, line height 1, tracking -0.06em (40px on mobile). Page title (h1).
- **headline-lg:** GeistSans 56px at weight 450, line height 1, tracking -0.06em (32px on mobile). Section headings (h2).
- **body-md:** GeistSans 16px at weight 400, line height 1.65. Body text.
- **body-lg:** GeistSans 24px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** GeistSans 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** GeistSans 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** GeistSans 14px at weight 500, line height 1.65. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (90% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 40px.
- **Sections:** 144px vertical padding between major sections.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Breakpoints:** 401px, 600px, 601px, 640px, 960px, 961px, 1020px, 1024px, 1150px, 1200px, 1280px, 1400px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#0A0A0A → #292929) and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(46, 46, 46) 0px 0px 0px 1px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 104 elements.
- **sm (2px):** 32 elements.
- **xl (8px):** 20 elements.
- **lg (6px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Search… ⌘K”):** #0A0A0A fill, #EDEDED text, 14px/400, 6px radius, padding 0px 6px 0px 14px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(46, 46, 46) 0px 0px 0px 1px`.
- **button-outline-hover:** background #1A1A1A, text #EDEDED on hover.
- **input-field (“your@email.com”):** #0A0A0A fill, #FFFFFF text, 14px/400, padding 0px 12px.
- **link:** transparent fill, #EDEDED text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #0A0A0A, #292929.
- Do keep text in 4 levels: #EDEDED, #FFFFFF, #A1A1A1, #8F8F8F.
- Do let contrast carry emphasis; primary actions use #EDEDED on #000000.
- Do set headlines in GeistSans with tight tracking (-0.06em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 2px, 8px and 6px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond GeistSans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.15s, 0.1s, 0.2s, 0.4s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.32, 0.72, 0, 1)`, `cubic-bezier(0.23, 1, 0.32, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/nextjs.org/), the free DESIGN.md generator.
