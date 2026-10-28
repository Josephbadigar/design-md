---
version: alpha
name: Nothing
description: "Light monochrome interface measured from nothing.tech: NType82-Regular type with Ndot-Regular, tonal surfaces and 4px corners."
colors:
  background: "#F4F4F4"
  surface: "#F4F4F4"
  on-surface: "#040404"
  on-background: "#040404"
  on-surface-variant: "#595A5A"
  surface-container-low: "#FFFFFF"
  overlay: "#FFFFFF0D"
  overlay-strong: "#3C3C3C99"
  primary: "#040404"
  on-primary: "#FFFFFF"
  warning: "#FFC700"
typography:
  headline-display:
    fontFamily: NType82-Regular
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
  headline-lg:
    fontFamily: Ndot-Regular
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1
  headline-md:
    fontFamily: NType82-Regular
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.1
  body-md:
    fontFamily: NType82-Regular
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: NType82-Regular
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
  code:
    fontFamily: LatteraMonoLL
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.1
  headline-display-mobile:
    fontFamily: NType82-Regular
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1
  headline-md-mobile:
    fontFamily: NType82-Regular
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 8px
  section: 144px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
    padding: 20px 40px
    height: 60px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
  link:
    textColor: "#D8D9D9"
---

# Nothing Design System

## Overview

Nothing describes itself as: “Here at Nothing, we’re building a world where tech is fun again. Remember a time when every new product made you excited? We’re bringing that back.” The interface is light, built on **Snow (#F4F4F4)** with **Near Black (#040404)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **NType82-Regular** and **Ndot-Regular**, with **LatteraMonoLL** for code. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 4px.

Measured from [nothing.tech](https://nothing.tech/) on October 21, 2026 at 1440×900 and 390×844 from 236 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Snow (#F4F4F4):** Page background, seen 2 times. Token `background`.
- **Near Black (#040404):** Primary text and headings, seen 20 times. Token `on-surface`.
- **Slate (#595A5A):** Secondary text, seen 13 times. Token `on-surface-variant`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`, CSS `--tw-ring-offset-color`.
- **White 5% (#FFFFFF0D):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **Graphite 60% (#3C3C3C99):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Near Black (#040404):** Primary buttons and calls to action, seen 54 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Amber (#FFC700):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**NType82-Regular**, **Ndot-Regular** and **LatteraMonoLL** (monospace) share the interface. Fallback stack: `NType82-Regular, sans-serif`. Other loaded fonts: Geist Variable, Geist Mono Variable, Ndot-Bold.

- **headline-display:** NType82-Regular 48px at weight 400, line height 1 (32px on mobile). Page title (h1).
- **headline-lg:** Ndot-Regular 40px at weight 400, line height 1. Section headings (h2).
- **headline-md:** NType82-Regular 24px at weight 400, line height 1.1 (20px on mobile). Sub-section headings.
- **body-md:** NType82-Regular 16px at weight 400, line height 1.4. Body text.
- **body-lg:** NType82-Regular 18px at weight 400, line height 1.4. Lead paragraphs.
- **code:** LatteraMonoLL 11px at weight 400, line height 1.1, uppercase. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (88% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 8px, md 16px, lg 32px, xl 40px.
- **Sections:** 144px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF).

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 24 elements.
- **md (6px):** 24 elements.
- **lg (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“GO TO: INDIA”):** #040404 fill, #FFFFFF text, 14px/400, 8px radius, padding 20px 40px.
- **button-outline (“DISCOVER”):** #FFFFFF fill, #040404 text, 16px/400, 4px radius, padding 12px 16px.
- **button-ghost (“STAY ON UNITED KINGDOM”):** transparent fill, #595A5A text, 14px/400, padding 0px.
- **input-field (“Email address”):** #3C3C3C99 fill, #FFFFFF text, 12px/400, 4px radius, padding 8px 16px.
- **link:** transparent fill, #D8D9D9 text, padding 0px.

## Do's and Don'ts

- Do use #F4F4F4 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 2 levels: #040404, #595A5A.
- Do let contrast carry emphasis; primary actions use #040404 on #F4F4F4.
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 4px corners on most elements; larger surfaces also use 6px and 8px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond NType82-Regular, Ndot-Regular and LatteraMonoLL.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/nothing.tech/), the free DESIGN.md generator.
