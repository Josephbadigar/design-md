---
version: alpha
name: Calendly.com
description: "Light interface measured from calendly.com: Calendly Sans type with Wulkan Text, pale blue accents, tonal surfaces and 4px corners."
colors:
  background: "#FCFBF8"
  surface: "#FCFBF8"
  on-surface: "#071A31"
  on-background: "#071A31"
  on-surface-variant: "#3D464E"
  on-surface-muted: "#5F6D77"
  surface-container-low: "#FFFFFF"
  overlay: "#FCFBF80D"
  overlay-strong: "#071A310D"
  outline: "#FCFBF81A"
  outline-variant: "#071A310D"
  primary: "#C3DFFE"
  on-primary: "#000000"
  secondary: "#467DCA"
  tertiary: "#6BB1FF"
typography:
  headline-display:
    fontFamily: Calendly Sans
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.028em
  headline-lg:
    fontFamily: Calendly Sans
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.033em
  headline-md:
    fontFamily: Wulkan Text
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.042em
  headline-sm:
    fontFamily: Geist
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.028em
  title-lg:
    fontFamily: Calendly Sans
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.2
  body-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.4
  label-lg:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.4
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.4
  headline-display-mobile:
    fontFamily: Calendly Sans
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
  headline-md-mobile:
    fontFamily: Wulkan Text
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.1
rounded:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 48px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 120px
  margin: 24px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 12px 16px
    height: 48px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 20px
    padding: 12px 20px
    height: 50px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 12px 16px
    height: 48px
  link:
    textColor: "{colors.background}"
---

# Calendly.com Design System

## Overview

Calendly.com describes itself as: “Calendly connects and simplifies all of the work around meetings, from scheduling, payments, and meeting prep to notetaking, contact management, and follow-up.” The interface is light, built on **Snow (#FCFBF8)** with **Deep Blue (#071A31)** text, and **Pale Blue (#C3DFFE)** as the main accent.

Type is set in **Calendly Sans** and **Wulkan Text**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [calendly.com](https://calendly.com/) on November 9, 2026 at 1440×900 and 390×844 from 401 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Snow (#FCFBF8):** Page background, seen 15 times. Token `background`, CSS `--color-ramp-orange-025`.
- **Deep Blue (#071A31):** Primary text and headings, seen 38 times. Token `on-surface`.
- **Cool Graphite (#3D464E):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Blue (#5F6D77):** Muted text and metadata, seen 13 times. Token `on-surface-muted`, CSS `--color-text-secondary`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Snow 5% (#FCFBF80D):** Translucent fill for cards and controls, seen 12 times. Token `overlay`.
- **Deep Blue 5% (#071A310D):** Stronger translucent fill, seen 7 times. Token `overlay-strong`.
- **Snow 10% (#FCFBF81A):** Borders and dividers, seen 12 times. Token `outline`.
- **Deep Blue 5% (#071A310D):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Pale Blue (#C3DFFE):** Brand color on large areas. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Blue (#467DCA):** Accent in logos and imagery. Token `secondary`.
- **Light Blue (#6BB1FF):** Accent, seen 6 times. Token `tertiary`.

## Typography

**Calendly Sans**, **Wulkan Text** and **Geist** share the interface. Fallback stack: `Calendly Sans, system-ui, -apple-system, Segoe UI`.

- **headline-display:** Calendly Sans 72px at weight 500, line height 1.1, tracking -0.028em (40px on mobile). Page title (h1).
- **headline-lg:** Calendly Sans 60px at weight 500, line height 1.1, tracking -0.033em. Section headings (h2).
- **headline-md:** Wulkan Text 48px at weight 500, line height 1.1, tracking -0.042em (28px on mobile). Sub-section headings.
- **headline-sm:** Geist 36px at weight 500, line height 1.1, tracking -0.028em. Card and feature titles.
- **title-lg:** Calendly Sans 28px at weight 500, line height 1.2. Small titles.
- **body-md:** Geist 14px at weight 400, line height 1.4. Body text.
- **body-lg:** Geist 18px at weight 500, line height 1.4. Lead paragraphs.
- **label-lg:** Geist 16px at weight 400, line height 1. Large buttons and tabs.
- **label-md:** Geist 14px at weight 500, line height 1.4. Buttons, navigation and labels.
- **label-sm:** Geist 12px at weight 500, line height 1.4. Small labels and badges.

## Layout

Spacing follows a 4px grid: 98% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 24px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(11, 53, 88, 0.16) 0px 20px 48px -12px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **xs (4px):** 172 elements.
- **sm (8px):** 48 elements.
- **md (12px):** 48 elements.
- **lg (16px):** 32 elements.
- **xl (48px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started for free”):** #071A31 fill, #FCFBF8 text, 14px/400, 16px radius, padding 12px 16px.
- **button-outline (“Sign up with Google”):** #FCFBF8 fill, #071A31 text, 16px/500, 20px radius, padding 12px 20px, border 1px solid #FCFBF8.
- **button-ghost (“Log In”):** transparent fill, #071A31 text, 14px/400, 16px radius, padding 12px 16px, border 1px solid #071A31.
- **link:** transparent fill, #FCFBF8B2 text, padding 0px.

## Do's and Don'ts

- Do use #FCFBF8 for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 3 levels: #071A31, #3D464E, #5F6D77.
- Do use #C3DFFE as the brand accent: header, logo and key highlights.
- Do set headlines in Calendly Sans with tight tracking (-0.028em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 8px, 12px and 16px.
- Don't introduce new font families beyond Calendly Sans, Wulkan Text and Geist.
- Don't use #C3DFFE for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.5s, 0.18s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/calendly.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
