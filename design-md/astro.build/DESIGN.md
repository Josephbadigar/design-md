---
version: alpha
name: Astro
description: "Dark interface measured from astro.build: Obviously type with system-ui, dark indigo accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#060913"
  surface: "#060913"
  on-surface: "#F2F6FA"
  on-background: "#F2F6FA"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#BFC1C9"
  on-surface-muted: "#858B98"
  surface-container-low: "#0D0F14"
  surface-container: "#0C0F19"
  overlay: "#2C2C2C4D"
  overlay-strong: "#0609138C"
  outline: "#858B9833"
  outline-variant: "#858B984D"
  primary: "#1A1367"
  on-primary: "#FFFFFF"
  secondary: "#5919A7"
  tertiary: "#54B9FF"
  success: "#4BF3C8"
  warning: "#FFD493"
typography:
  headline-display:
    fontFamily: Obviously
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.1
  headline-lg:
    fontFamily: Obviously
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.2
  headline-md:
    fontFamily: Obviously
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.4
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
  body-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.81
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Obviously
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: Obviously
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
rounded:
  sm: 8px
  md: 12px
  lg: 16px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 48px
  gutter: 8px
  margin: 32px
  container: 1280px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 42px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 4px 12px
  card:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Astro Design System

## Overview

Astro describes itself as: “Astro builds fast content sites, powerful web applications, dynamic server APIs, and everything in-between.” The interface is dark, built on **Cool Charcoal (#060913)** with **Cool Snow (#F2F6FA)** text, and **Dark Indigo (#1A1367)** as the main accent.

Type is set in **Obviously** and **system-ui**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [astro.build](https://astro.build/) on October 21, 2026 at 1440×900 and 390×844 from 409 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles, plus gradient stops #D83333, #F041FF, #3245FF, #B845ED.

- **Cool Charcoal (#060913):** Page background, seen 3 times. Token `background`.
- **Cool Snow (#F2F6FA):** Primary text and headings, seen 21 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 25 times. Token `on-surface-strong`, CSS `--tw-ring-offset-color`.
- **Cool Silver (#BFC1C9):** Secondary text, seen 35 times. Token `on-surface-variant`.
- **Cool Gray (#858B98):** Muted text and metadata, seen 11 times. Token `on-surface-muted`.
- **Cool Charcoal (#0D0F14):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Cool Charcoal (#0C0F19):** Cards and panels, seen 15 times. Token `surface-container`.
- **Graphite 30% (#2C2C2C4D):** Translucent fill for cards and controls, seen 7 times. Token `overlay`.
- **Cool Charcoal 55% (#0609138C):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Cool Gray 20% (#858B9833):** Borders and dividers, seen 34 times. Token `outline`.
- **Cool Gray 30% (#858B984D):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Dark Indigo (#1A1367):** Brand color in logos and imagery. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Violet (#5919A7):** Brand color in logos and imagery, seen 18 times. Token `secondary`.
- **Blue (#54B9FF):** Most used accent color, seen 15 times. Token `tertiary`.
- **Teal (#4BF3C8):** Success and positive states, seen 12 times. Token `success`.
- **Light Orange (#FFD493):** Warnings and highlights, seen 3 times. Token `warning`.

## Typography

**Obviously** and **system-ui** share the interface. Fallback stack: `Obviously, obviously-fallback, system-ui, sans-serif`. Other loaded fonts: Inter, MDIO, md-io-fallback, obviously-fallback.

- **headline-display:** Obviously 48px at weight 700, line height 1.1 (30px on mobile). Page title (h1).
- **headline-lg:** Obviously 30px at weight 400, line height 1.2 (24px on mobile). Section headings (h2).
- **headline-md:** Obviously 20px at weight 700, line height 1.4. Sub-section headings.
- **body-md:** system-ui 16px at weight 300, line height 1.5. Body text.
- **body-sm:** system-ui 14px at weight 400, line height 1.81. Secondary and small text.
- **label-md:** system-ui 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 100% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 32px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 68 elements.
- **lg (16px):** 60 elements.
- **sm (8px):** 44 elements.
- **md (12px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #FFFFFF fill, #F2F6FA text, 16px/400, 9999px radius, padding 8px 16px.
- **button-primary-hover:** background #F2F6FA, text #F2F6FA on hover.
- **button-outline (“Astro 7.4 Available now!”):** #0609138C fill, #F2F6FA text, 16px/400, 9999px radius, padding 0px.
- **button-ghost (“React”):** transparent fill, #F2F6FA text, 16px/400, 8px radius, padding 0px.
- **input-field (“your@email.com”):** #060913 fill, #F2F6FA text, 16px/400, 8px radius, padding 4px 12px, border 1px solid #23262D.
- **card:** #0C0F19 fill, #F2F6FA text, 16px/400, 16px radius, padding 0px, border 1px solid #858B9833.
- **link:** transparent fill, #BFC1C9 text, padding 0px.

## Do's and Don'ts

- Do use #060913 for the page and lift surfaces in small steps: #0D0F14, #0C0F19.
- Do keep text in 4 levels: #F2F6FA, #FFFFFF, #BFC1C9, #858B98.
- Do use #1A1367 as the brand accent: header, logo and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 16px corners.
- Don't introduce new font families beyond Obviously and system-ui.
- Don't use #1A1367 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.5s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/astro.build/), the free DESIGN.md generator.
