---
version: alpha
name: IBM
description: "Light interface measured from ibm.com: IBM Plex Sans type, vivid blue accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#161616"
  on-background: "#161616"
  on-surface-variant: "#525252"
  surface-container-low: "#F4F4F4"
  outline: "#C6C6C6"
  outline-variant: "#E0E0E0"
  primary: "#0F62FE"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: IBM Plex Sans
    fontSize: 53.5px
    fontWeight: 300
    lineHeight: 1.17
  headline-lg:
    fontFamily: IBM Plex Sans
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.25
  headline-md:
    fontFamily: IBM Plex Sans
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.29
  headline-sm:
    fontFamily: IBM Plex Sans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
  body-md:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  body-sm:
    fontFamily: IBM Plex Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: 0.027em
  label-md:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.29
    letterSpacing: 0.011em
  headline-display-mobile:
    fontFamily: IBM Plex Sans
    fontSize: 33px
    fontWeight: 400
    lineHeight: 1.25
rounded:
  sm: 4px
  md: 16px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 64px
  gutter: 8px
  margin: 32px
  container: 1584px
components:
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 1px 4px
---

# IBM Design System

## Overview

IBM describes itself as: “For more than a century, IBM has been a global technology innovator, leading advances in AI, automation and hybrid cloud solutions that help businesses grow.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#161616)** text, and **Vivid Blue (#0F62FE)** as the main accent.

Type is set in **IBM Plex Sans**. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 4px.

Measured from [ibm.com/us-en](https://www.ibm.com/us-en) (the site sent our reader to its /us-en version; ibm.com was asked for) on November 4, 2026 at 1440×900 and 390×844 from 201 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles, plus gradient stops #0F62FE, #8A3FFC.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`, CSS `--tc-bg-color`.
- **Charcoal (#161616):** Primary text and headings, seen 33 times. Token `on-surface`, CSS `--tc-text-color`.
- **Slate (#525252):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **Snow (#F4F4F4):** Raised areas one step from the page, seen 9 times. Token `surface-container-low`, CSS `--cds-field`.
- **Silver (#C6C6C6):** Borders and dividers, seen 7 times. Token `outline`, CSS `--cds-border-subtle-selected`.
- **Silver (#E0E0E0):** Secondary dividers, seen 6 times. Token `outline-variant`, CSS `--cds-border-subtle`.
- **Vivid Blue (#0F62FE):** Most used accent color, seen 17 times. Token `primary`, CSS `--tc-gradient-hover-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**IBM Plex Sans** carries the whole interface. Fallback stack: `IBM Plex Sans, Helvetica Neue, Arial, sans-serif`. Other loaded fonts: ibm_icons, Lato.

- **headline-display:** IBM Plex Sans 53.5px at weight 300, line height 1.17 (33px on mobile). Page title (h1).
- **headline-lg:** IBM Plex Sans 32px at weight 400, line height 1.25. Section headings (h2).
- **headline-md:** IBM Plex Sans 28px at weight 400, line height 1.29. Sub-section headings.
- **headline-sm:** IBM Plex Sans 20px at weight 600, line height 1.4. Card and feature titles.
- **body-md:** IBM Plex Sans 16px at weight 400, line height 1. Body text.
- **body-sm:** IBM Plex Sans 12px at weight 400, line height 1.33, tracking 0.027em. Secondary and small text.
- **label-md:** IBM Plex Sans 14px at weight 400, line height 1.29, tracking 0.011em. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 93% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1584px.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 1056px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F4F4F4) and hairline rings:

- `rgb(255, 255, 255) 0px 0px 0px 1440px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 28 elements.
- **md (16px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-ghost (“1”):** transparent fill, #161616 text, 14px/600, padding 1px 4px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F4F4F4.
- Do keep text in 2 levels: #161616, #525252.
- Do reserve #0F62FE for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 16px.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond IBM Plex Sans.
- Don't use #0F62FE for large backgrounds or body text.
- Don't make interface transitions slower than 0.24s.

## Motion

Interface transitions are quick: 0.15s, 0.24s, 0.07s.

- **Easing:** `cubic-bezier(0.2, 0, 0.38, 0.9)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/ibm.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
