---
version: alpha
name: Liveblocks
description: "Dark interface measured from liveblocks.io: suisse type, purple accents, flat surfaces and 4px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#B7B4B4"
  on-surface-muted: "#918D8D"
  on-surface-subtle: "#635F5F"
  overlay: "#FDFCFC29"
  overlay-strong: "#FFFFFF73"
  outline: "#FDFCFC29"
  primary: "#D165EC"
  on-primary: "#000000"
  secondary: "#88BEF2"
  tertiary: "#EFD26C"
typography:
  headline-display:
    fontFamily: suisse
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: suisse
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: 0.004em
  body-md:
    fontFamily: suisse
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.25
  body-lg:
    fontFamily: suisse
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: suisse
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: suisse
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  label-sm:
    fontFamily: suisse
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
  code:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: suisse
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.015em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 28px
  xl: 48px
  gutter: 8px
  section: 196px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 14px
    height: 36px
  button-outline:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    padding: 4px 4px 4px 12px
    height: 38px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 12px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Liveblocks Design System

## Overview

Liveblocks describes itself as: “Liveblocks provides the infrastructure to handle concurrent edits on shared data, so people and AI agents can collaborate without breaking your app.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Purple (#D165EC)** as the main accent.

Type is set in **suisse**, with **JetBrains Mono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [liveblocks.io](https://liveblocks.io/) on November 4, 2026 at 1440×900 and 390×844 from 442 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #F2EFC8, #4778B4.

- **Near Black (#000000):** Page background, seen 2 times. Token `background`, CSS `--tw-mask-bottom-from-color`.
- **White (#FFFFFF):** Primary text and headings, seen 32 times. Token `on-surface`.
- **Gray (#B7B4B4):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Gray (#918D8D):** Muted text and metadata, seen 91 times. Token `on-surface-muted`, CSS `--lb-marketing-color-neutral-300`.
- **Slate (#635F5F):** Subtle text and placeholders, seen 2 times. Token `on-surface-subtle`, CSS `--color-marketing-subtlest`.
- **Snow 16% (#FDFCFC29):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **White 45% (#FFFFFF73):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Snow 16% (#FDFCFC29):** Borders and dividers, seen 1 time. Token `outline`.
- **Purple (#D165EC):** Brand accent (CSS variable). Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#88BEF2):** Accent (CSS variable). Token `secondary`.
- **Amber (#EFD26C):** Accent (CSS variable). Token `tertiary`.

## Typography

**suisse** and **JetBrains Mono** (monospace) share the interface. Fallback stack: `suisse, suisse Fallback, -apple-system, BlinkMacSystemFont`.

- **headline-display:** suisse 60px at weight 500, line height 1.1, tracking -0.02em (36px on mobile). Page title (h1).
- **headline-lg:** suisse 20px at weight 400, line height 1.38, tracking 0.004em. Section headings (h2).
- **body-md:** suisse 14px at weight 400, line height 1.25. Body text.
- **body-lg:** suisse 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-lg:** suisse 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** suisse 14px at weight 500, line height 1.43. Buttons, navigation and labels.
- **label-sm:** suisse 12px at weight 500, line height 1.33. Small labels and badges.
- **code:** JetBrains Mono 14px at weight 400, line height 1.43. Code and technical values.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 28px, xl 48px.
- **Sections:** 196px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(39, 38, 38) 0px 0px 0px 1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(255, 255, 255) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 280 elements.
- **md (6px):** 72 elements.
- **lg (8px):** 32 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #FFFFFF fill, #000000 text, 14px/500, 6px radius, padding 0px 14px.
- **button-outline (“New Introducing Liveblocks Sync”):** transparent fill, #B7B4B4 text, 16px/500, 3.35544e+07px radius, padding 4px 4px 4px 12px, border 1px solid #FDFCFC29.
- **button-ghost (“Product”):** transparent fill, #FFFFFF text, 14px/500, 6px radius, padding 8px 12px.
- **input-field:** transparent fill, #FFFFFF text, 16px/400, padding 0px.
- **link:** transparent fill, #918D8D text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page.
- Do keep text in 4 levels: #FFFFFF, #B7B4B4, #918D8D, #635F5F.
- Do use #D165EC as the brand accent: header, logo and key highlights.
- Do set headlines in suisse with tight tracking (-0.02em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 6px and 8px.
- Don't use #635F5F for body text; it reaches 3.33:1 on #000000. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond suisse and JetBrains Mono.
- Don't use #D165EC for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.2s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0, 0, 0.2, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/liveblocks.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
