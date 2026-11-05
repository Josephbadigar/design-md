---
version: alpha
name: Superlist
description: "Light interface measured from superlist.com: Haffer XH SemiBold type with Inter, purple accents, flat surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#696F81"
  on-background: "#696F81"
  on-surface-variant: "#8E8DA0"
  primary: "#F866DB"
  on-primary: "#000000"
  inverse-surface: "#181824"
  secondary: "#9087FF"
typography:
  headline-display:
    fontFamily: Haffer XH SemiBold
    fontSize: 64px
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Haffer XH SemiBold
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Haffer XH SemiBold
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.005em
  body-lg:
    fontFamily: CUSTOM;Blender Medium
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.3
  body-sm:
    fontFamily: sans-serif
    fontSize: 12px
    fontWeight: 400
  label-md:
    fontFamily: Satoshi
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.2
  headline-display-mobile:
    fontFamily: Haffer XH SemiBold
    fontSize: 48px
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Haffer XH SemiBold
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-md-mobile:
    fontFamily: Haffer XH SemiBold
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
rounded:
  sm: 8px
  md: 10px
spacing:
  xs: 2px
  sm: 6px
  md: 10px
  lg: 25px
  xl: 50px
  gutter: 10px
  margin: 25px
  container: 1500px
components:
  link:
    textColor: "{colors.on-surface-variant}"
---

# Superlist Design System

## Overview

Superlist describes itself as: “From the creators of Wunderlist — the all-in-one task management app for to-do lists, notes, and projects. AI-powered productivity that replaces 5 apps. Free to start, works on Mac, Web, iOS & Android.” The interface is light, built on **White (#FFFFFF)** with **Blue (#696F81)** text, and **Purple (#F866DB)** as the main accent.

Type is set in **Haffer XH SemiBold** and **Inter**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 8px.

Measured from [superlist.com](https://www.superlist.com/) on November 4, 2026 at 1440×900 and 390×844 from 341 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **White (#FFFFFF):** Page background. Token `background`.
- **Blue (#696F81):** Primary text and headings, seen 8 times. Token `on-surface`.
- **Cool Gray (#8E8DA0):** Secondary text, seen 46 times. Token `on-surface-variant`.
- **Purple (#F866DB):** Main accent color, seen 17 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Cool Charcoal (#181824):** High-contrast fills, seen 4 times. Token `inverse-surface`.
- **Light Indigo (#9087FF):** Accent in text, fills and borders, seen 19 times. Token `secondary`.

## Typography

**Haffer XH SemiBold**, **Inter**, **CUSTOM;Blender Medium**, **sans-serif** and **Satoshi** share the interface. Fallback stack: `Haffer XH SemiBold, Haffer XH SemiBold Placeholder, sans-serif`. Other loaded fonts: Jersey 10.

- **headline-display:** Haffer XH SemiBold 64px at weight 600, line height 0.95, tracking -0.02em (48px on mobile). Page title (h1).
- **headline-lg:** Haffer XH SemiBold 48px at weight 600, line height 1.1, tracking -0.02em (36px on mobile). Section headings (h2).
- **headline-md:** Haffer XH SemiBold 24px at weight 400, line height 1.2, tracking -0.02em (18px on mobile). Sub-section headings.
- **body-md:** Inter 14px at weight 400, line height 1.3, tracking -0.005em. Body text.
- **body-lg:** CUSTOM;Blender Medium 16px at weight 400, line height 1.3. Lead paragraphs.
- **body-sm:** sans-serif 12px at weight 400. Secondary and small text.
- **label-md:** Satoshi 16px at weight 500, line height 1.2. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 6% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 10px, lg 25px, xl 50px.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1500px.
- **Page margin:** 25px on each side of full-width sections.
- **Breakpoints:** 809px, 809.98px, 810px, 1199px, 1299.98px, 1399px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 12 elements.
- **md (10px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **link:** transparent fill, #8E8DA0 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #696F81, #8E8DA0.
- Do reserve #F866DB for primary actions and key highlights.
- Do set headlines in Haffer XH SemiBold with tight tracking (-0.02em).
- Do reuse the measured spacing steps (6px, 10px, 25px).
- Do use 8px corners on most elements; larger surfaces also use 10px.
- Don't use #8E8DA0 for body text; it reaches 3.25:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Haffer XH SemiBold, Inter, CUSTOM;Blender Medium, sans-serif and Satoshi.
- Don't use #F866DB for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s.

- **Easing:** `cubic-bezier(0.44, 0, 0.56, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/superlist.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
