---
version: alpha
name: Magic UI
description: "Light interface measured from magicui.design: Geist type, vivid indigo accents, flat surfaces and 14px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0A0A0A"
  on-background: "#0A0A0A"
  on-surface-variant: "#737373"
  on-surface-muted: "#A1A1A1"
  overlay: "#F5F5F580"
  outline: "#E5E5E5"
  primary: "#4F39F6"
  on-primary: "#FFFFFF"
  secondary: "#00C950"
  tertiary: "#2B7FFF"
typography:
  headline-display:
    fontFamily: Geist
    fontSize: 72px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.05em
  body-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Geist
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.63
  label-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.05em
  headline-lg-mobile:
    fontFamily: Geist
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.05em
rounded:
  sm: 10px
  md: 14px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 56px
  gutter: 8px
  section: 56px
  margin: 32px
  container: 1400px
components:
  button-primary:
    textColor: "#FAFAFA"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-secondary:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-outline:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: 8px
    padding: 8px 48px 8px 16px
    height: 32px
  button-ghost:
    typography: "{typography.body-md}"
    rounded: 8px
    padding: 8px 48px 8px 16px
  card:
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 20px
---

# Magic UI Design System

## Overview

Magic UI describes itself as: “Beautiful UI components and templates to make your landing page look stunning.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#0A0A0A)** text, and **Vivid Indigo (#4F39F6)** as the main accent.

Type is set in **Geist**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 14px.

Measured from [magicui.design](https://magicui.design/) on November 4, 2026 at 1440×900 and 390×844 from 359 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #FF4242, #A0FF42, #40A1FF, #43D0FF.

- **White (#FFFFFF):** Page background, seen 44 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Near Black (#0A0A0A):** Primary text and headings, seen 14 times. Token `on-surface`.
- **Slate (#737373):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Gray (#A1A1A1):** Muted text and metadata, seen 84 times. Token `on-surface-muted`.
- **Snow 50% (#F5F5F580):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Mist (#E5E5E5):** Borders and dividers, seen 43 times. Token `outline`.
- **Vivid Indigo (#4F39F6):** Brand color in the header. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Green (#00C950):** Accent in text, fills and borders, seen 2 times. Token `secondary`.
- **Vivid Blue (#2B7FFF):** Accent, seen 11 times. Token `tertiary`.

## Typography

**Geist** carries the whole interface. Fallback stack: `Geist, sans-serif`. Other loaded fonts: Geist Mono.

- **headline-display:** Geist 72px at weight 600, line height 1, tracking -0.05em (48px on mobile). Page title (h1).
- **headline-lg:** Geist 48px at weight 600, line height 1.2, tracking -0.05em (30px on mobile). Section headings (h2).
- **body-md:** Geist 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Geist 15px at weight 400, line height 1.63. Lead paragraphs.
- **label-md:** Geist 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Geist 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing follows a 4px grid: 96% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 56px.
- **Sections:** 56px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1400px.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 600px, 1600px, 2000px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`

## Shapes

Most elements use 14px corners. Measured radii, most used first:

- **md (14px):** 164 elements.
- **sm (10px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Browse Components”):** transparent fill, #FAFAFA text, 14px/500, 10px radius, padding 0px 16px.
- **button-secondary (“Browse Templates”):** transparent fill, #0A0A0A text, 14px/500, 10px radius, padding 0px 16px.
- **button-outline (“Search documentation... ⌘ K”):** #F5F5F580 fill, #737373 text, 14px/400, 8px radius, padding 8px 48px 8px 16px, border 1px solid #E5E5E5, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-ghost (“Search documentation... ⌘ K”):** transparent fill, 14px/400, 8px radius, padding 8px 48px 8px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **card:** transparent fill, 16px/400, 14px radius, padding 20px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #0A0A0A, #737373, #A1A1A1.
- Do use #4F39F6 as the brand accent: header, logo and key highlights.
- Do set headlines in Geist with tight tracking (-0.05em).
- Do keep spacing on the 4px grid.
- Do use 14px corners on most elements; larger surfaces also use 10px.
- Don't use #A1A1A1 for body text; it reaches 2.58:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Geist.
- Don't use #4F39F6 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.3s. Longer ambient animations run 2s, 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/magicui.design/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
