---
version: alpha
name: MongoDB
description: "Dark interface measured from mongodb.com: Sohne Condensed type with Sohne, vivid green accents, tonal surfaces and 16px corners."
colors:
  background: "#061621"
  surface: "#061621"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#FDFEEC"
  on-surface-muted: "#E5E8DC"
  on-surface-subtle: "#3D4F58"
  surface-container-low: "#081B28"
  outline: "#3D4F58"
  outline-variant: "#FFFFFF1A"
  primary: "#00ED64"
  on-primary: "#001E2B"
  inverse-surface: "#F3F5E6"
  secondary: "#016BF8"
  tertiary: "#765CF8"
  success: "#00684A"
typography:
  headline-display:
    fontFamily: Sohne Condensed
    fontSize: 64px
    fontWeight: 700
    lineHeight: 1.13
  headline-lg:
    fontFamily: Sohne Condensed
    fontSize: 58px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Sohne
    fontSize: 36px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: 0.01em
  headline-sm:
    fontFamily: Sohne Condensed
    fontSize: 32px
    fontWeight: 700
    lineHeight: 0.95
  title-lg:
    fontFamily: Sohne Condensed
    fontSize: 24px
    fontWeight: 700
    lineHeight: 0.95
  body-md:
    fontFamily: Sohne
    fontSize: 14px
    fontWeight: 400
  body-lg:
    fontFamily: Sohne
    fontSize: 16px
    fontWeight: 300
  label-lg:
    fontFamily: Sohne
    fontSize: 16px
    fontWeight: 400
  label-md:
    fontFamily: Sohne
    fontSize: 15px
    fontWeight: 600
  label-sm:
    fontFamily: Sohne
    fontSize: 14px
    fontWeight: 500
  code:
    fontFamily: Sohne Mono
    fontSize: 12px
    fontWeight: 600
    letterSpacing: 0.1em
  title-lg-mobile:
    fontFamily: Sohne Condensed
    fontSize: 18px
    fontWeight: 700
    lineHeight: 0.95
rounded:
  xs: 2px
  sm: 4px
  md: 12px
  lg: 16px
  xl: 48px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 128px
  margin: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 16px 32px
    height: 50px
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.background}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 15px 24px
    height: 48px
  button-tertiary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 8px
    padding: 8px 16px
    height: 38px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.background}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# MongoDB Design System

## Overview

MongoDB describes itself as: “MongoDB is the intelligent data platform for the AI era. Get your ideas to market faster with flexible, real-time data that scales across any cloud.” The interface is dark, built on **Deep Blue (#061621)** with **White (#FFFFFF)** text, and **Vivid Green (#00ED64)** as the main accent.

Type is set in **Sohne Condensed** and **Sohne**, with **Sohne Mono** for code. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 16px.

Measured from [mongodb.com](https://www.mongodb.com/) on October 21, 2026 at 1440×900 and 390×844 from 336 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #B1FF05, #00ED64, #001E2B, #21313C.

- **Deep Blue (#061621):** Page background, seen 3 times. Token `background`, CSS `--color-link-inline-hover`.
- **White (#FFFFFF):** Primary text and headings, seen 32 times. Token `on-surface`, CSS `--color-background-panel`.
- **Pale Yellow (#FDFEEC):** Secondary text, seen 18 times. Token `on-surface-variant`, CSS `--color-card-background-primary`.
- **Mist (#E5E8DC):** Muted text and metadata, seen 7 times. Token `on-surface-muted`, CSS `--color-background-surface-tertiary`.
- **Dark Blue (#3D4F58):** Subtle text and placeholders, seen 4 times. Token `on-surface-subtle`.
- **Deep Blue (#081B28):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Dark Blue (#3D4F58):** Borders and dividers, seen 11 times. Token `outline`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Green (#00ED64):** Primary buttons and calls to action, seen 17 times. Token `primary`, CSS `--mdb-br-spring`.
- **Deep Cyan (#001E2B):** Text and icons on primary. Token `on-primary`.
- **Warm Mist (#F3F5E6):** High-contrast fills, seen 28 times. Token `inverse-surface`, CSS `--color-background-surface-secondary`.
- **Vivid Blue (#016BF8):** Secondary buttons, seen 19 times. Token `secondary`.
- **Indigo (#765CF8):** Brand color on large areas, seen 15 times. Token `tertiary`.
- **Deep Teal (#00684A):** Success and positive states, seen 16 times. Token `success`, CSS `--color-state-link-cta-hover`.

## Typography

**Sohne Condensed**, **Sohne** and **Sohne Mono** (monospace) share the interface. Fallback stack: `Sohne Condensed, Helvetica Neue, Helvetica, Arial`. Other loaded fonts: MongoDB Value Serif, Noto Sans KR.

- **headline-display:** Sohne Condensed 64px at weight 700, line height 1.13. Page title (h1).
- **headline-lg:** Sohne Condensed 58px at weight 700, line height 0.95, tracking -0.01em. Section headings (h2).
- **headline-md:** Sohne 36px at weight 700, line height 0.95, tracking 0.01em. Sub-section headings.
- **headline-sm:** Sohne Condensed 32px at weight 700, line height 0.95. Card and feature titles.
- **title-lg:** Sohne Condensed 24px at weight 700, line height 0.95 (18px on mobile). Small titles.
- **body-md:** Sohne 14px at weight 400. Body text.
- **body-lg:** Sohne 16px at weight 300. Lead paragraphs.
- **label-lg:** Sohne 16px at weight 400. Large buttons and tabs.
- **label-md:** Sohne 15px at weight 600. Buttons, navigation and labels.
- **label-sm:** Sohne 14px at weight 500. Small labels and badges.
- **code:** Sohne Mono 12px at weight 600, tracking 0.1em, uppercase. Code and technical values.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 48px on each side of full-width sections.
- **Breakpoints:** 460px, 767px, 768px, 948px, 1023px, 1024px, 1200px, 1280px, 1281px, 1374px, 1440px, 1680px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.15) 0px 3px 9px 0px`
- `rgba(0, 30, 43, 0.12) 0px 26px 44px 0px, rgba(0, 0, 0, 0.13) 0px 7px 13px 0px`
- `rgba(0, 0, 0, 0.13) 0px 7px 12px 0px`

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **lg (16px):** 120 elements.
- **full (9999px):** 40 elements.
- **xs (2px):** 36 elements.
- **sm (4px):** 20 elements.
- **xl (48px):** 16 elements.
- **md (12px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #00ED64 fill, #001E2B text, 16px/500, 4px radius, padding 16px 32px, border 1px solid #00684A.
- **button-secondary (“Get Started”):** #00ED64 fill, #061621 text, 16px/500, 4px radius, padding 15px 24px, border 1px solid #00ED64.
- **button-tertiary (“Builder”):** #016BF8 fill, #FFFFFF text, 14px/500, 8px radius, padding 8px 16px.
- **button-ghost (“Products”):** transparent fill, #FFFFFF text, 16px/400, padding 0px.
- **card:** #081B28 fill, #061621 text, 16px/400, 12px radius, padding 0px, border 1px solid #FFFFFF1A.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #061621 for the page and lift surfaces in small steps: #081B28.
- Do keep text in 4 levels: #FFFFFF, #FDFEEC, #E5E8DC, #3D4F58.
- Do reserve #00ED64 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 16px corners on most elements; larger surfaces also use 2px, 4px and 48px.
- Don't use #3D4F58 for body text; it reaches 2.1:1 on #061621. Keep it for large text or metadata.
- Don't introduce new font families beyond Sohne Condensed, Sohne and Sohne Mono.
- Don't use #00ED64 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.25s, 0.15s. Longer ambient animations run 3s.

- **Easing:** `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mongodb.com/), the free DESIGN.md generator.
