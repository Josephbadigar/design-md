---
version: alpha
name: n8n
description: "Light interface measured from n8n.io: n8n Baumer Uniwidth type with Inter, pale red accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FAFAFA"
  surface: "#FAFAFA"
  on-surface: "#161616"
  on-background: "#161616"
  on-surface-variant: "#212121"
  on-surface-muted: "#303030"
  on-surface-subtle: "#616161"
  surface-container-low: "#F0F0F0"
  surface-container: "#E6E6E6"
  surface-container-high: "#D9D9D9"
  outline: "#FFBCCA"
  outline-variant: "#D9D9D9"
  primary: "#FFBCCA"
  on-primary: "#161616"
  error: "#FF91AC"
typography:
  headline-display:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 64px
    fontWeight: 500
    lineHeight: 0.85
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.01em
  headline-md:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.13
  title-lg:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1
  body-md:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.29
  label-lg:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.25
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.2
  code:
    fontFamily: n8n Baumer Mono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.29
    letterSpacing: 0.02em
  headline-display-mobile:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 48px
    fontWeight: 500
    lineHeight: 0.92
    letterSpacing: -0.01em
  headline-md-mobile:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.06
    letterSpacing: -0.01em
  title-lg-mobile:
    fontFamily: n8n Baumer Uniwidth
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
rounded:
  sm: 8px
  md: 24px
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
  margin: 24px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 47px
  button-secondary:
    backgroundColor: "{colors.outline}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 12px 16px
    height: 42px
  button-tertiary:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 12px 16px
    height: 42px
  button-tertiary-hover:
    backgroundColor: "#C2C2C2"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 12px 16px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 16px 32px 16px 16px
  link:
    textColor: "{colors.background}"
---

# n8n Design System

## Overview

n8n describes itself as: “n8n is a workflow automation platform that uniquely combines AI capabilities with business process automation, giving technical teams the flexibility of code with the speed of no-code.” The interface is light, built on **Snow (#FAFAFA)** with **Charcoal (#161616)** text, and **Pale Red (#FFBCCA)** as the main accent.

Type is set in **n8n Baumer Uniwidth** and **Inter**, with **n8n Baumer Mono** for code. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Controls are pill-shaped.

Measured from [n8n.io](https://n8n.io/) on October 21, 2026 at 1440×900 and 390×844 from 331 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Snow (#FAFAFA):** Page background, seen 2 times. Token `background`, CSS `--color-surface-card-transparent`.
- **Charcoal (#161616):** Primary text and headings, seen 51 times. Token `on-surface`.
- **Charcoal (#212121):** Secondary text, seen 4 times. Token `on-surface-variant`, CSS `--color-stroke-invert-secondary`.
- **Graphite (#303030):** Muted text and metadata, seen 32 times. Token `on-surface-muted`, CSS `--color-stroke-default-secondary`.
- **Slate (#616161):** Subtle text and placeholders, seen 4 times. Token `on-surface-subtle`.
- **Mist (#F0F0F0):** Raised areas one step from the page, seen 11 times. Token `surface-container-low`, CSS `--color-grey-100`.
- **Mist (#E6E6E6):** Cards and panels, seen 3 times. Token `surface-container`, CSS `--color-surface-backgrounds-widget`.
- **Silver (#D9D9D9):** Hover and pressed fills, seen 8 times. Token `surface-container-high`.
- **Pale Red (#FFBCCA):** Borders and dividers, seen 2 times. Token `outline`, CSS `--color-surface-button-primary-default`.
- **Silver (#D9D9D9):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Pale Red (#FFBCCA):** Primary buttons and calls to action, seen 10 times. Token `primary`, CSS `--color-surface-button-primary-default`.
- **Charcoal (#161616):** Text and icons on primary. Token `on-primary`.
- **Light Red (#FF91AC):** Errors and destructive states, seen 1 time. Token `error`, CSS `--color-stroke-highlight-default`.

## Typography

**n8n Baumer Uniwidth**, **Inter** and **n8n Baumer Mono** (monospace) share the interface. Fallback stack: `n8n Baumer Uniwidth, Helvetica, system-ui, -apple-system`.

- **headline-display:** n8n Baumer Uniwidth 64px at weight 500, line height 0.85, tracking -0.01em (48px on mobile). Page title (h1).
- **headline-lg:** n8n Baumer Uniwidth 48px at weight 500, line height 1, tracking -0.01em. Section headings (h2).
- **headline-md:** n8n Baumer Uniwidth 40px at weight 500, line height 1.05, tracking -0.01em (32px on mobile). Sub-section headings.
- **headline-sm:** n8n Baumer Uniwidth 32px at weight 500, line height 1.13. Card and feature titles.
- **title-lg:** n8n Baumer Uniwidth 24px at weight 500, line height 1 (20px on mobile). Small titles.
- **body-md:** n8n Baumer Uniwidth 16px at weight 400, line height 1.5. Body text.
- **body-sm:** n8n Baumer Uniwidth 14px at weight 400, line height 1.29. Secondary and small text.
- **label-lg:** n8n Baumer Uniwidth 16px at weight 500, line height 1.25. Large buttons and tabs.
- **label-md:** Inter 15px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** n8n Baumer Uniwidth 14px at weight 500, line height 1.2. Small labels and badges.
- **code:** n8n Baumer Mono 14px at weight 400, line height 1.29, tracking 0.02em, uppercase. Code and technical values.

## Layout

Spacing follows a 4px grid: 95% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 440px, 624px, 767px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F0F0F0 → #E6E6E6 → #D9D9D9) and #FFBCCA borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 184 elements.
- **md (24px):** 80 elements.
- **sm (8px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Accept all”):** #FFBCCA fill, #161616 text, 14px/400, 9999px radius, padding 8px 16px.
- **button-secondary (“GET STARTED”):** #FFBCCA fill, #212121 text, 14px/400, 9999px radius, padding 12px 16px.
- **button-tertiary (“TALK TO SALES”):** #D9D9D9 fill, #161616 text, 14px/400, 9999px radius, padding 12px 16px.
- **button-tertiary-hover:** background #C2C2C2, text #161616 on hover.
- **button-ghost (“PRODUCT”):** transparent fill, #161616 text, 14px/400, 9999px radius, padding 12px 16px.
- **card:** #F0F0F0 fill, #161616 text, 16px/400, 24px radius, padding 16px 32px 16px 16px.
- **link:** transparent fill, #FAFAFA text, padding 0px.

## Do's and Don'ts

- Do use #FAFAFA for the page and lift surfaces in small steps: #F0F0F0, #E6E6E6, #D9D9D9.
- Do keep text in 4 levels: #161616, #212121, #303030, #616161.
- Do reserve #FFBCCA for primary actions and key highlights.
- Do set headlines in n8n Baumer Uniwidth with tight tracking (-0.01em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 24px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond n8n Baumer Uniwidth, Inter and n8n Baumer Mono.
- Don't use #FFBCCA for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.5s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/n8n.io/), the free DESIGN.md generator.
