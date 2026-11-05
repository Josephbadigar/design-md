---
version: alpha
name: Venmo
description: "Light monochrome interface measured from venmo.com: Venmo Sans type, flat surfaces and pill-shaped controls."
colors:
  background: "#4BB4FF"
  surface: "#4BB4FF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#FFFFFF"
  overlay: "#FFFFFF52"
  outline: "#FFFFFF"
  primary: "#F5F5F7"
  on-primary: "#000000"
  secondary: "#3F34EE"
typography:
  headline-display:
    fontFamily: Venmo Sans
    fontSize: 70.5px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Venmo Sans
    fontSize: 57.5px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Venmo Sans
    fontSize: 47px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.03em
  body-md:
    fontFamily: Venmo Sans
    fontSize: 17px
    fontWeight: 500
    lineHeight: 1.16
  body-lg:
    fontFamily: Venmo Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.35
    letterSpacing: -0.01em
  label-md:
    fontFamily: Venmo Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  label-sm:
    fontFamily: Venmo Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.35
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: Venmo Sans
    fontSize: 44px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: Venmo Sans
    fontSize: 38px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.03em
  headline-md-mobile:
    fontFamily: Venmo Sans
    fontSize: 33px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.03em
rounded:
  sm: 8px
  md: 32px
  full: 9999px
spacing:
  md: 16px
  lg: 20px
  xl: 52.8px
  gutter: 24px
  section: 52.8px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 16px 20px
    height: 52px
  button-primary-hover:
    backgroundColor: "#E1E1E3"
  card:
    backgroundColor: "{colors.outline}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px
---

# Venmo Design System

## Overview

Venmo describes itself as: “Welcome to Venmo! Manage your account balance, send/receive money, split bills, pay friends, and stay connected with your network all in one place.” The interface is light, built on **Blue (#4BB4FF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Venmo Sans**. Headlines run large with tight negative tracking; body text is 17px. The surface language is flat. Controls are pill-shaped.

Measured from [venmo.com](https://venmo.com/) on November 4, 2026 at 1440×900 and 390×844 from 90 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Blue (#4BB4FF):** Page background, seen 2 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 32 times. Token `on-surface`.
- **White (#FFFFFF):** Secondary text, seen 7 times. Token `on-surface-variant`, CSS `--tw-ring-offset-color`.
- **White 32% (#FFFFFF52):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White (#FFFFFF):** Borders and dividers, seen 4 times. Token `outline`, CSS `--tw-ring-offset-color`.
- **Snow (#F5F5F7):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#3F34EE):** Accent, seen 1 time. Token `secondary`.

## Typography

**Venmo Sans** carries the whole interface. Fallback stack: `Venmo Sans`. Other loaded fonts: PayPalOpen-Regular.

- **headline-display:** Venmo Sans 70.5px at weight 700, line height 0.95, tracking -0.03em (44px on mobile). Page title (h1).
- **headline-lg:** Venmo Sans 57.5px at weight 700, line height 0.95, tracking -0.03em (38px on mobile). Section headings (h2).
- **headline-md:** Venmo Sans 47px at weight 700, line height 0.95, tracking -0.03em (33px on mobile). Sub-section headings.
- **body-md:** Venmo Sans 17px at weight 500, line height 1.16. Body text.
- **body-lg:** Venmo Sans 18px at weight 400, line height 1.35, tracking -0.01em. Lead paragraphs.
- **label-md:** Venmo Sans 16px at weight 400, line height 1.15. Buttons, navigation and labels.
- **label-sm:** Venmo Sans 14px at weight 500, line height 1.35, tracking -0.01em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** md 16px, lg 20px, xl 52.8px.
- **Sections:** 52.8px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Breakpoints:** 400px, 575.98px, 600px, 752px, 768px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #FFFFFF borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 52 elements.
- **md (32px):** 12 elements.
- **sm (8px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“See how it works”):** #F5F5F7 fill, #000000 text, 16.9286px/500, 1000px radius, padding 16px 20px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 1px inset`.
- **button-primary-hover:** background #E1E1E3, text #000000 on hover.
- **card:** #FFFFFF fill, #000000 text, 16px/400, 32px radius, padding 0px.

## Do's and Don'ts

- Do use #4BB4FF for the page.
- Do keep text in 2 levels: #000000, #FFFFFF.
- Do let contrast carry emphasis; primary actions use #F5F5F7 on #4BB4FF.
- Do set headlines in Venmo Sans with tight tracking (-0.03em).
- Do reuse the measured spacing steps (16px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 32px corners.
- Don't use #FFFFFF for body text; it reaches 2.26:1 on #4BB4FF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Venmo Sans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.3s, 0.6s.

- **Easing:** `cubic-bezier(0.4, 1.2, 0.2, 1)`, `cubic-bezier(0.22, 1, 0.36, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/venmo.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
