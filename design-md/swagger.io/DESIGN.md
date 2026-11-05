---
version: alpha
name: Swagger
description: "Light interface measured from swagger.io: DM Sans type, vivid blue accents, flat surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#212529"
  on-background: "#212529"
  on-surface-variant: "#173647"
  overlay: "#E6E6E633"
  primary: "#1874FE"
  on-primary: "#FFFFFF"
  secondary: "#F56A00"
  tertiary: "#061C5A"
typography:
  headline-display:
    fontFamily: DM Sans
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.2
  headline-lg:
    fontFamily: DM Sans
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.25
  headline-md:
    fontFamily: DM Sans
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
  body-md:
    fontFamily: DM Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: DM Sans
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.45
  label-lg:
    fontFamily: DM Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  label-md:
    fontFamily: DM Sans
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.43
  label-sm:
    fontFamily: DM Sans
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1.33
rounded:
  sm: 4px
  md: 8px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 8px
  section: 128px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10.5px 21px
    height: 43px
  button-primary-hover:
    backgroundColor: "#0D408C"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 12px 24px
    height: 50px
  button-secondary-hover:
    backgroundColor: "#AE4B00"
  button-outline:
    textColor: "{colors.primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10.5px 21px
    height: 43px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 8px 16px
  link:
    textColor: "{colors.on-primary}"
---

# Swagger Design System

## Overview

Swagger describes itself as: “Simplify API development for users, teams, and enterprises with our open source and professional toolset. Findogut how Swagger can help you and get started today.” The interface is light, built on **White (#FFFFFF)** with **Cool Graphite (#212529)** text, and **Vivid Blue (#1874FE)** as the main accent.

Type is set in **DM Sans**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 4px.

Measured from [swagger.io](https://swagger.io/) on November 4, 2026 at 1440×900 and 390×844 from 259 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **White (#FFFFFF):** Page background, seen 3 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Cool Graphite (#212529):** Primary text and headings, seen 31 times. Token `on-surface`.
- **Deep Blue (#173647):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Mist 20% (#E6E6E633):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Vivid Blue (#1874FE):** Brand color on large areas, seen 27 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#F56A00):** Secondary buttons, seen 2 times. Token `secondary`.
- **Deep Blue (#061C5A):** Accent in text, fills and borders, seen 10 times. Token `tertiary`.

## Typography

**DM Sans** carries the whole interface. Fallback stack: `DM Sans, sans-serif`. Other loaded fonts: Font Awesome 5 Pro.

- **headline-display:** DM Sans 40px at weight 700, line height 1.2. Page title (h1).
- **headline-lg:** DM Sans 32px at weight 700, line height 1.25. Section headings (h2).
- **headline-md:** DM Sans 24px at weight 600, line height 1.33. Sub-section headings.
- **body-md:** DM Sans 14px at weight 400, line height 1.43. Body text.
- **body-lg:** DM Sans 18px at weight 600, line height 1.45. Lead paragraphs.
- **label-lg:** DM Sans 16px at weight 400, line height 1.6. Large buttons and tabs.
- **label-md:** DM Sans 14px at weight 700, line height 1.43. Buttons, navigation and labels.
- **label-sm:** DM Sans 12px at weight 700, line height 1.33, uppercase. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (81% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 12px, lg 20px, xl 40px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 450px, 576px, 640px, 649.98px, 650px, 768px, 980px, 992px, 1030px, 1200px, 1229.98px, 1230px, 1232px, 1280px, 1328px, 1440px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 20 elements.
- **md (8px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #1874FE fill, #FFFFFF text, 14px/600, 4px radius, padding 10.5px 21px.
- **button-primary-hover:** background #0D408C, text #FFFFFF on hover.
- **button-secondary (“See how we do it”):** #F56A00 fill, #FFFFFF text, 16px/600, 4px radius, padding 12px 24px.
- **button-secondary-hover:** background #AE4B00, text #FFFFFF on hover.
- **button-outline (“Sign In”):** transparent fill, #1874FE text, 14px/600, 4px radius, padding 10.5px 21px, border 1px solid #1874FE.
- **button-ghost (“Products”):** transparent fill, #173647 text, 16px/400, padding 8px 16px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #212529, #173647.
- Do use #1874FE as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 4px corners on most elements; larger surfaces also use 8px.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond DM Sans.
- Don't use #1874FE for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.2s, 0.15s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/swagger.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
