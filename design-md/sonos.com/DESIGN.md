---
version: alpha
name: Sonos
description: "Light monochrome interface measured from sonos.com: aktiv-grotesk type, tonal surfaces and 80px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#2E2E2E"
  on-surface-muted: "#333333"
  on-surface-subtle: "#BFBFBF"
  surface-container-low: "#F4F4F4"
  outline: "#F4F4F4"
  outline-variant: "#BFBFBF"
  primary: "#000000"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: aktiv-grotesk
    fontSize: 96px
    fontWeight: 500
    lineHeight: 1.2
  headline-lg:
    fontFamily: aktiv-grotesk
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1.2
  headline-md:
    fontFamily: aktiv-grotesk
    fontSize: 42px
    fontWeight: 500
    lineHeight: 1
  headline-sm:
    fontFamily: aktiv-grotesk
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
  body-md:
    fontFamily: aktiv-grotesk
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: aktiv-grotesk
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.3
  body-sm:
    fontFamily: aktiv-grotesk
    fontSize: 14px
    fontWeight: 400
  label-md:
    fontFamily: aktiv-grotesk
    fontSize: 16px
    fontWeight: 700
  headline-display-mobile:
    fontFamily: aktiv-grotesk
    fontSize: 54px
    fontWeight: 500
    lineHeight: 1.2
  headline-md-mobile:
    fontFamily: aktiv-grotesk
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.13
  headline-lg-mobile:
    fontFamily: aktiv-grotesk
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.2
rounded:
  sm: 50px
  md: 80px
  full: 9999px
spacing:
  sm: 6px
  md: 16px
  lg: 20px
  xl: 48px
  gutter: 106.67px
  section: 80px
  margin: 106.67px
  container: 1440px
components:
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: 16px 48px
    height: 59px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
  input-field:
    textColor: "#F5F5F5"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px 0px 8px 0px
  link:
    textColor: "{colors.on-surface-subtle}"
---

# Sonos Design System

## Overview

Sonos describes itself as: “Introducing our new soundbar, Beam Ultra, and our latest over ear headphones, Sonos Ace Ultra.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **aktiv-grotesk**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 80px.

Measured from [sonos.com](https://www.sonos.com/en-in/home) on October 21, 2026 at 1440×900 and 390×844 from 369 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 5 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Primary text and headings, seen 34 times. Token `on-surface`.
- **Graphite (#2E2E2E):** Secondary text, seen 7 times. Token `on-surface-variant`.
- **Graphite (#333333):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Silver (#BFBFBF):** Subtle text and placeholders, seen 51 times. Token `on-surface-subtle`.
- **Snow (#F4F4F4):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F4F4F4):** Borders and dividers, seen 1 time. Token `outline`.
- **Silver (#BFBFBF):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Near Black (#000000):** Primary actions (the main text color; the palette is monochrome), seen 56 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**aktiv-grotesk** carries the whole interface. Fallback stack: `aktiv-grotesk, Helvetica, Arial, sans-serif`.

- **headline-display:** aktiv-grotesk 96px at weight 500, line height 1.2 (54px on mobile). Page title (h1).
- **headline-lg:** aktiv-grotesk 64px at weight 500, line height 1.2 (32px on mobile). Section headings (h2).
- **headline-md:** aktiv-grotesk 42px at weight 500, line height 1 (32px on mobile). Sub-section headings.
- **headline-sm:** aktiv-grotesk 40px at weight 400, line height 1.2. Card and feature titles.
- **body-md:** aktiv-grotesk 16px at weight 400. Body text.
- **body-lg:** aktiv-grotesk 21px at weight 400, line height 1.3. Lead paragraphs.
- **body-sm:** aktiv-grotesk 14px at weight 400. Secondary and small text.
- **label-md:** aktiv-grotesk 16px at weight 700. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (78% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 6px, md 16px, lg 20px, xl 48px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 106.67px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 106.67px on each side of full-width sections.
- **Breakpoints:** 400px, 425px, 426px, 500px, 530px, 550px, 600px, 640px, 768px, 769px, 896px, 1023px, 1024px, 1440px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.627) 0px 0px 3px 0px inset, rgb(0, 0, 0) 0px 0px 3px 0px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(224, 224, 224) 0px -1px 0px 0px inset`.

## Shapes

Most elements use 80px corners. Measured radii, most used first:

- **md (80px):** 76 elements.
- **full (9999px):** 12 elements.
- **sm (50px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Shop new arrivals”):** #FFFFFF fill, #000000 text, 18px/500, 80px radius, padding 16px 48px, border 2px solid #000000.
- **button-ghost (“My Account”):** transparent fill, #000000 text, 16px/400, 80px radius, padding 0px.
- **input-field (“Enter email address”):** transparent fill, #F5F5F5 text, 16px/400, padding 0px 0px 8px 0px.
- **link:** transparent fill, #BFBFBF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F4F4F4.
- Do keep text in 4 levels: #000000, #2E2E2E, #333333, #BFBFBF.
- Do let contrast carry emphasis; primary actions use #000000 on #FFFFFF.
- Do reuse the measured spacing steps (6px, 16px, 20px).
- Do use 80px corners on most elements; larger surfaces also use 50px.
- Don't use #BFBFBF for body text; it reaches 1.8:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond aktiv-grotesk.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.1s, 0.3s, 0.5s.

- **Easing:** `cubic-bezier(0.4, 0, 1, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/sonos.com/), the free DESIGN.md generator.
