---
version: alpha
name: Zapier
description: "Light interface measured from zapier.com: Degular Display type with Inter, vivid orange accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFEFB"
  surface: "#FFFEFB"
  on-surface: "#201515"
  on-background: "#201515"
  on-surface-variant: "#36342E"
  on-surface-muted: "#605D52"
  surface-container-low: "#F8F4F0"
  surface-container: "#ECEAE3"
  overlay: "#605D52BF"
  outline: "#DFDCD2"
  outline-variant: "#ECEAE3"
  primary: "#FF4F00"
  on-primary: "#201515"
  secondary: "#4285F4"
  success: "#34A853"
  warning: "#FBBC05"
  error: "#EA4335"
typography:
  headline-display:
    fontFamily: Degular Display
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1
  headline-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.04
  headline-md:
    fontFamily: Serrif
    fontSize: 32px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Serrif
    fontSize: 28px
    fontWeight: 300
    lineHeight: 1.25
    letterSpacing: -0.015em
  title-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 400
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 600
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.71
  headline-display-mobile:
    fontFamily: Degular Display
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1
rounded:
  sm: 4px
  md: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  section: 120px
  margin: 20px
  container: 720px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 6px 10px
    height: 36px
  button-primary-hover:
    backgroundColor: "{colors.surface-container-low}"
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: 18px
    padding: 6px 12px
    height: 36px
  button-tertiary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 12px 24px
    height: 48px
  button-tertiary-hover:
    backgroundColor: "{colors.on-surface-variant}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 6px 10px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 24px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Zapier Design System

## Overview

Zapier describes itself as: “Build and scale AI workflows and agents across 9,000+ apps with Zapier—the most connected AI orchestration platform. Trusted by 3 million+ businesses.” The interface is light, built on **Snow (#FFFEFB)** with **Warm Charcoal (#201515)** text, and **Vivid Orange (#FF4F00)** as the main accent.

Type is set in **Degular Display** and **Inter**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [zapier.com](https://zapier.com/) on October 21, 2026 at 1440×900 and 390×844 from 386 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **Snow (#FFFEFB):** Page background, seen 6 times. Token `background`.
- **Warm Charcoal (#201515):** Primary text and headings, seen 42 times. Token `on-surface`.
- **Warm Graphite (#36342E):** Secondary text, seen 65 times. Token `on-surface-variant`.
- **Warm Slate (#605D52):** Muted text and metadata, seen 16 times. Token `on-surface-muted`.
- **Warm Snow (#F8F4F0):** Raised areas one step from the page, seen 11 times. Token `surface-container-low`.
- **Warm Mist (#ECEAE3):** Cards and panels, seen 6 times. Token `surface-container`.
- **Warm Slate 75% (#605D52BF):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Warm Silver (#DFDCD2):** Borders and dividers, seen 2 times. Token `outline`.
- **Warm Mist (#ECEAE3):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Vivid Orange (#FF4F00):** Primary buttons and calls to action, seen 18 times. Token `primary`.
- **Warm Charcoal (#201515):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#4285F4):** Accent, seen 1 time. Token `secondary`.
- **Green (#34A853):** Success and positive states, seen 1 time. Token `success`.
- **Vivid Amber (#FBBC05):** Warnings and highlights, seen 1 time. Token `warning`.
- **Vivid Red (#EA4335):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Degular Display**, **Inter** and **Serrif** share the interface. Fallback stack: `Degular Display, DegularDisplay, DegularDisplay Fallback, Inter`. Other loaded fonts: DegularDisplay.

- **headline-display:** Degular Display 56px at weight 500, line height 1 (40px on mobile). Page title (h1).
- **headline-lg:** Inter 48px at weight 500, line height 1.04. Section headings (h2).
- **headline-md:** Serrif 32px at weight 300, line height 1.2, tracking -0.02em. Sub-section headings.
- **headline-sm:** Serrif 28px at weight 300, line height 1.25, tracking -0.015em. Card and feature titles.
- **title-lg:** Inter 20px at weight 400, tracking -0.01em. Small titles.
- **body-md:** Inter 14px at weight 400, line height 1.71. Body text.
- **body-lg:** Inter 18px at weight 600. Lead paragraphs.
- **body-sm:** Inter 12px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Inter 16px at weight 400. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1.71. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (81% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 16px, lg 24px, xl 40px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 720px.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 400px, 425px, 426px, 476px, 530px, 550px, 600px, 768px, 896px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F8F4F0 → #ECEAE3) and hairline rings:

- `rgb(32, 21, 21) 0px 0px 0px 1px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (4px):** 88 elements.
- **full (9999px):** 36 elements.
- **md (12px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Products”):** #FF4F00 fill, #201515 text, 14px/400, 4px radius, padding 6px 10px.
- **button-primary-hover:** background #F8F4F0, text #201515 on hover.
- **button-secondary (“Sign up”):** #FF4F00 fill, #FFFEFB text, 14px/600, 18px radius, padding 6px 12px, border 1px solid #FF4F00.
- **button-tertiary (“Explore Zapier for Enterprise”):** #201515 fill, #FFFEFB text, 18px/600, 4px radius, padding 12px 24px, border 1px solid #201515.
- **button-tertiary-hover:** background #36342E, text #FFFEFB on hover.
- **button-ghost (“Products”):** transparent fill, #201515 text, 14px/400, 4px radius, padding 6px 10px.
- **card:** #ECEAE3 fill, #201515 text, 16px/400, 12px radius, padding 24px, border 1px solid #201515, shadow `rgb(32, 21, 21) 0px 0px 0px 1px`.
- **link:** transparent fill, #36342E text, padding 0px.

## Do's and Don'ts

- Do use #FFFEFB for the page and lift surfaces in small steps: #F8F4F0, #ECEAE3.
- Do keep text in 3 levels: #201515, #36342E, #605D52.
- Do reserve #FF4F00 for primary actions and key highlights.
- Do reuse the measured spacing steps (6px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Degular Display, Inter and Serrif.
- Don't use #FF4F00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.25s, 0.3s.

- **Easing:** `ease`, `cubic-bezier(0.16, 1, 0.3, 1)`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/zapier.com/), the free DESIGN.md generator.
