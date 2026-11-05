---
version: alpha
name: Aceternity UI
description: "Light interface measured from ui.aceternity.com: Local x2wexs type, vivid blue accents, tonal surfaces and 5.6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#09090B"
  on-background: "#09090B"
  on-surface-variant: "#404040"
  on-surface-muted: "#525252"
  on-surface-subtle: "#737373"
  surface-container-low: "#F5F5F5"
  surface-container: "#E5E5E5"
  overlay: "#2B7FFF40"
  outline: "#D4D4D4"
  primary: "#3074FE"
  on-primary: "#000000"
  inverse-surface: "#171717"
  secondary: "#1DA1F2"
  tertiary: "#F0B100"
typography:
  headline-display:
    fontFamily: Local x2wexs
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Local x2wexs
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Local x2wexs
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: Local x2wexs
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.4
  body-md:
    fontFamily: Local x2wexs
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Local x2wexs
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Local x2wexs
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Local x2wexs
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Local x2wexs
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.025em
rounded:
  xs: 5.6px
  sm: 7.6px
  md: 10px
  lg: 20px
  xl: 24px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 8px
  section: 80px
  margin: 32px
  container: 1280px
components:
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-subtle}"
    rounded: 7px
    padding: 0px 4px 0px 8px
    height: 28px
  button-ghost:
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
  link:
    textColor: "{colors.on-surface-subtle}"
---

# Aceternity UI Design System

## Overview

Aceternity UI describes itself as: “Aceternity UI is a React component library with 200+ copy-paste components, blocks, and landing page templates built with Tailwind CSS and Motion.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#09090B)** text, and **Vivid Blue (#3074FE)** as the main accent.

Type is set in **Local x2wexs**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 5.6px.

Measured from [ui.aceternity.com](https://ui.aceternity.com/) on November 4, 2026 at 1440×900 and 390×844 from 438 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #3F80FF, #2867F2, #77A5FF, #497CEB.

- **White (#FFFFFF):** Page background, seen 46 times. Token `background`, CSS `--card`.
- **Near Black (#09090B):** Primary text and headings, seen 35 times. Token `on-surface`, CSS `--popover-foreground`.
- **Graphite (#404040):** Secondary text, seen 41 times. Token `on-surface-variant`.
- **Slate (#525252):** Muted text and metadata, seen 42 times. Token `on-surface-muted`.
- **Slate (#737373):** Subtle text and placeholders, seen 27 times. Token `on-surface-subtle`.
- **Snow (#F5F5F5):** Raised areas one step from the page, seen 13 times. Token `surface-container-low`.
- **Mist (#E5E5E5):** Cards and panels, seen 6 times. Token `surface-container`.
- **Vivid Blue 25% (#2B7FFF40):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Silver (#D4D4D4):** Borders and dividers, seen 2 times. Token `outline`.
- **Vivid Blue (#3074FE):** Main accent color, seen 6 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#171717):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Vivid Blue (#1DA1F2):** Accent, seen 17 times. Token `secondary`.
- **Vivid Amber (#F0B100):** Accent, seen 5 times. Token `tertiary`.

## Typography

**Local x2wexs** carries the whole interface. Fallback stack: `__Local_x2wexs, system-ui, -apple-system, BlinkMacSystemFont`. Other loaded fonts: __Local_x2wexs.

- **headline-display:** Local x2wexs 48px at weight 600, line height 1, tracking -0.025em (30px on mobile). Page title (h1).
- **headline-lg:** Local x2wexs 30px at weight 500, line height 1.2, tracking -0.025em. Section headings (h2).
- **headline-md:** Local x2wexs 24px at weight 600, line height 1.33, tracking -0.025em. Sub-section headings.
- **headline-sm:** Local x2wexs 20px at weight 700, line height 1.4. Card and feature titles.
- **body-md:** Local x2wexs 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Local x2wexs 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-md:** Local x2wexs 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Local x2wexs 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (74% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 16px, lg 32px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 32px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0 0 0 / 0.05) 0px 0px 0px 1px, oklab(0 0 0 / 0.1) 0px 1px 3px 0px, oklab(0 0 0 / 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0 0 0 / 0.1) 0px 0px 0px 1px, oklab(0 0 0 / 0.1) 0px 1px 3px 0px, oklab(0 0 0 / 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0 0 0 / 0.05) 0px 0px 0px 1px, oklab(0 0 0 / 0.05) 0px 1px 3px 0px, oklab(0 0 0 / 0.05) 0px 1px 2px -1px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklch(0.623 0.214 259.815) 0px 0px 0px 1px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.

## Shapes

Most elements use 5.6px corners. Measured radii, most used first:

- **xs (5.6px):** 128 elements.
- **md (10px):** 80 elements.
- **lg (20px):** 48 elements.
- **sm (7.6px):** 44 elements.
- **xl (24px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Search ⌘ K”):** #FFFFFF fill, #737373 text, 12px/400, 7px radius, padding 0px 4px 0px 8px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0 0 0 / 0.05) 0px 0px 0px 1px, oklab(0 0 0 / 0.05) 0px 1px 3px 0px, oklab(0 0 0 / 0.05) 0px 1px 2px -1px`.
- **button-ghost (“Resources”):** transparent fill, 14px/500, 7.6px radius, padding 0px 12px.
- **link:** transparent fill, #737373 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F5F5, #E5E5E5.
- Do keep text in 4 levels: #09090B, #404040, #525252, #737373.
- Do reserve #3074FE for primary actions and key highlights.
- Do set headlines in Local x2wexs with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 5.6px corners on most elements; larger surfaces also use 10px, 20px and 7.6px.
- Don't introduce new font families beyond Local x2wexs.
- Don't use #3074FE for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ui.aceternity.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
