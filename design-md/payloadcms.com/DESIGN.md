---
version: alpha
name: Payload
description: "Light monochrome interface measured from payloadcms.com: untitledSans type, flat surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#808080"
  outline: "#FFFFFF20"
  primary: "#000000"
  on-primary: "#FFFFFF"
  inverse-surface: "#070707"
typography:
  headline-display:
    fontFamily: untitledSans
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: untitledSans
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.05em
  headline-md:
    fontFamily: untitledSans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.05em
  headline-sm:
    fontFamily: untitledSans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.05em
  title-lg:
    fontFamily: untitledSans
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.04em
  body-md:
    fontFamily: untitledSans
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.2
  label-md:
    fontFamily: untitledSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  label-sm:
    fontFamily: untitledSans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0.25em
  code:
    fontFamily: GeistMono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  headline-display-mobile:
    fontFamily: untitledSans
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.05em
  headline-lg-mobile:
    fontFamily: untitledSans
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.05em
  headline-sm-mobile:
    fontFamily: untitledSans
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.05em
rounded:
  sm: 4px
  md: 40px
spacing:
  xs: 2.4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 64px
  gutter: 16px
  section: 128px
  container: 1440px
components:
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 4px 8px
    height: 28px
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  input-field:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "#D0D0D0"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 16px 24px
  link:
    textColor: "{colors.on-primary}"
---

# Payload Design System

## Overview

Payload describes itself as: “Built with TypeScript and React, Payload is an open-source headless CMS and application framework. Build anything.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **untitledSans**, with **GeistMono** for code. Headlines run large with tight negative tracking; body text is 15px. The surface language is flat. Corners are mostly 4px.

Measured from [payloadcms.com](https://payloadcms.com/) on November 4, 2026 at 1440×900 and 390×844 from 251 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`, CSS `--docsearch-footer-background`.
- **Near Black (#000000):** Primary text and headings, seen 1 time. Token `on-surface`, CSS `--theme-elevation-1000`.
- **Gray (#808080):** Secondary text, seen 2 times. Token `on-surface-variant`, CSS `--color-base-500`.
- **White 13% (#FFFFFF20):** Borders and dividers, seen 12 times. Token `outline`.
- **Near Black (#000000):** Primary actions (the main text color; the palette is monochrome), seen 12 times. Token `primary`, CSS `--theme-elevation-1000`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Near Black (#070707):** High-contrast fills, seen 1 time. Token `inverse-surface`.

## Typography

**untitledSans** and **GeistMono** (monospace) share the interface. Fallback stack: `untitledSans, untitledSans Fallback`. Other loaded fonts: Roboto Mono.

- **headline-display:** untitledSans 64px at weight 500, line height 1, tracking -0.05em (40px on mobile). Page title (h1).
- **headline-lg:** untitledSans 48px at weight 500, line height 1, tracking -0.05em (28px on mobile). Section headings (h2).
- **headline-md:** untitledSans 32px at weight 500, line height 1, tracking -0.05em. Sub-section headings.
- **headline-sm:** untitledSans 24px at weight 500, line height 1.2, tracking -0.05em (18px on mobile). Card and feature titles.
- **title-lg:** untitledSans 22px at weight 400, line height 1.2, tracking -0.04em. Small titles.
- **body-md:** untitledSans 15px at weight 400, line height 1.2. Body text.
- **label-md:** untitledSans 16px at weight 400, line height 1.4. Buttons, navigation and labels.
- **label-sm:** untitledSans 12px at weight 400, line height 1, tracking 0.25em, uppercase. Small labels and badges.
- **code:** GeistMono 14px at weight 400, line height 1.4. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (70% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2.4px, sm 8px, md 16px, lg 24px, xl 64px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Breakpoints:** 400px, 600px, 768px, 1024px, 1170px, 1200px, 1400px, 1600px, 1920px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #FFFFFF20 borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 4 elements.
- **md (40px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Get Started”):** #FFFFFF fill, #000000 text, 15px/400, 4px radius, padding 4px 8px, border 1px solid #FFFFFF.
- **button-ghost (“Product”):** transparent fill, #FFFFFF text, 16px/400, padding 0px.
- **input-field (“Enter your email”):** #070707 fill, #D0D0D0 text, 16px/400, padding 16px 24px, border 1px solid #FFFFFF20.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #000000, #808080.
- Do let contrast carry emphasis; primary actions use #000000 on #FFFFFF.
- Do set headlines in untitledSans with tight tracking (-0.05em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 40px.
- Don't use #808080 for body text; it reaches 3.95:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond untitledSans and GeistMono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.55s.

## Motion

Interface transitions are quick: 0.55s, 0.35s, 0.3s, 0.45s. Longer ambient animations run 0.9s.

- **Easing:** `cubic-bezier(0.165, 0.84, 0.44, 1)`, `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/payloadcms.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
