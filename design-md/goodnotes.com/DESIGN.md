---
version: alpha
name: Goodnotes
description: "Light interface measured from goodnotes.com: Roobert type with system-ui, cyan accents, tonal surfaces and 10px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#1E1E1E"
  on-surface-muted: "#565656"
  surface-container-low: "#E8E8E8"
  overlay: "#FFFFFF1A"
  outline: "#BEBEBE"
  outline-variant: "#E0E0E0"
  primary: "#57D2EE"
  on-primary: "#1E1E1E"
  secondary: "#45BFDB"
  tertiary: "#00B3DC"
typography:
  headline-display:
    fontFamily: Roobert
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Roobert
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: Roobert
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Roobert
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.4
  body-sm:
    fontFamily: Roobert
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.2
  label-md:
    fontFamily: Roobert
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.3
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Roobert
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.25
  headline-lg-mobile:
    fontFamily: Roobert
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.02em
rounded:
  sm: 8px
  md: 10px
  lg: 20px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 16px
  margin: 40px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 8.2px 16.4px
    height: 39px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
    height: 45px
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "#00000099"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
    height: 45px
---

# Goodnotes Design System

## Overview

Goodnotes describes itself as: “Bring your thinking to life, collaborate in real time, and turn brainstorming into action with shared notes, whiteboards and text documents.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Cyan (#57D2EE)** as the main accent.

Type is set in **Roobert** and **system-ui**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 10px.

Measured from [goodnotes.com](https://www.goodnotes.com/) on November 4, 2026 at 1440×900 and 390×844 from 249 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 34 times. Token `background`, CSS `--_color---background-white`.
- **Near Black (#000000):** Primary text and headings, seen 32 times. Token `on-surface`.
- **Charcoal (#1E1E1E):** Secondary text, seen 21 times. Token `on-surface-variant`.
- **Slate (#565656):** Muted text and metadata, seen 25 times. Token `on-surface-muted`.
- **Mist (#E8E8E8):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Silver (#BEBEBE):** Borders and dividers, seen 14 times. Token `outline`.
- **Silver (#E0E0E0):** Secondary dividers, seen 4 times. Token `outline-variant`.
- **Cyan (#57D2EE):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **Charcoal (#1E1E1E):** Text and icons on primary. Token `on-primary`.
- **Cyan (#45BFDB):** Accent (CSS variable), seen 1 time. Token `secondary`, CSS `--_02-brand-colors---background--primary--teal<deleted|variable-5801b894-daf4-5e2c-92e9-77e6f2fd3515>`.
- **Vivid Cyan (#00B3DC):** Accent (CSS variable). Token `tertiary`.

## Typography

**Roobert** and **system-ui** share the interface. Fallback stack: `Roobert, Arial, sans-serif`. Other loaded fonts: webflow-icons.

- **headline-display:** Roobert 48px at weight 700, line height 1.2, tracking -0.02em (28px on mobile). Page title (h1).
- **headline-lg:** Roobert 40px at weight 600, line height 1.2, tracking -0.02em (32px on mobile). Section headings (h2).
- **body-md:** Roobert 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Roobert 18px at weight 500, line height 1.4. Lead paragraphs.
- **body-sm:** Roobert 10px at weight 400, line height 1.2. Secondary and small text.
- **label-md:** Roobert 16px at weight 500, line height 1.3. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 700, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (78% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 40px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 376px, 479px, 767px, 768px, 991px, 1200px, 1440px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#E8E8E8) and #BEBEBE borders.

## Shapes

Most elements use 10px corners. Measured radii, most used first:

- **md (10px):** 80 elements.
- **full (9999px):** 20 elements.
- **sm (8px):** 16 elements.
- **lg (20px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start Free”):** #57D2EE fill, #1E1E1E text, 14px/400, 10px radius, padding 8.2px 16.4px.
- **button-primary-hover:** background #45BFDB, text #1E1E1E on hover.
- **button-outline (“PDF Annotation”):** #E8E8E8 fill, #000000 text, 16px/600, 20px 20px 0px 0px radius, padding 0px, border 1px solid #E0E0E0.
- **button-ghost (“Whiteboard”):** #FFFFFF fill, #00000099 text, 16px/600, 20px 20px 0px 0px radius, padding 0px, border 1px solid #E0E0E0.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #E8E8E8.
- Do keep text in 3 levels: #000000, #1E1E1E, #565656.
- Do reserve #57D2EE for primary actions and key highlights.
- Do set headlines in Roobert with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 10px corners on most elements; larger surfaces also use 8px and 20px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Roobert and system-ui.
- Don't use #57D2EE for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s.

- **Easing:** `ease-in-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/goodnotes.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
