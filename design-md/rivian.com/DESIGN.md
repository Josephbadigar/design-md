---
version: alpha
name: Rivian
description: "Light interface measured from rivian.com: Liga type with Adventure, vivid amber accents, tonal surfaces and 40px corners."
colors:
  background: "#ECECEC"
  surface: "#ECECEC"
  on-surface: "#151515"
  on-background: "#151515"
  on-surface-strong: "#000000"
  surface-container-low: "#F2F2F2"
  surface-container: "#FFFFFF"
  outline: "#FFFFFF"
  outline-variant: "#D1D1D180"
  primary: "#FFAA00"
  on-primary: "#000000"
  secondary: "#A15842"
  error: "#E84826"
typography:
  headline-display:
    fontFamily: Liga
    fontSize: 360px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.022em
  headline-lg:
    fontFamily: Adventure
    fontSize: 72px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Adventure
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.07
    letterSpacing: -0.045em
  headline-sm:
    fontFamily: Adventure
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.02em
  title-lg:
    fontFamily: Adventure
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.25
  body-md:
    fontFamily: Adventure
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Adventure
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: Adventure
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: Adventure
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.031em
  label-sm:
    fontFamily: Adventure
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.14
    letterSpacing: -0.036em
  headline-lg-mobile:
    fontFamily: Adventure
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.09
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 12px
  lg: 36px
  xl: 40px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 40px
  gutter: 12px
  container: 1920px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 32px
  button-secondary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.surface-container}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px 16px
    height: 40px
  button-secondary-hover:
    backgroundColor: "#333333"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.xl}"
    padding: 8px 16px
    height: 56px
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  input-field:
    backgroundColor: "#212121"
    textColor: "{colors.surface-container}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 20px 16px 0px 16px
  link:
    textColor: "{colors.surface-container}"
---

# Rivian Design System

## Overview

Rivian describes itself as: “Discover Rivian's long-range electric vehicles, innovative EV trucks, SUVs and vans built for adventure. Join the movement towards a sustainable future.” The interface is light, built on **Mist (#ECECEC)** with **Charcoal (#151515)** text, and **Vivid Amber (#FFAA00)** as the main accent.

Type is set in **Liga** and **Adventure**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 40px.

Measured from [rivian.com](https://rivian.com/) on October 21, 2026 at 1440×900 and 390×844 from 269 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles, plus gradient stops #8BA8BD, #5D767D.

- **Mist (#ECECEC):** Page background. Token `background`.
- **Charcoal (#151515):** Primary text and headings, seen 18 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 46 times. Token `on-surface-strong`, CSS `--k-preference-tabs-purposes-header-link-color`.
- **Mist (#F2F2F2):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`, CSS `--k-banner-header-returnButton-background-color`.
- **White (#FFFFFF):** Cards and panels, seen 15 times. Token `surface-container`, CSS `--k-consentGate-header-background`.
- **White (#FFFFFF):** Borders and dividers, seen 5 times. Token `outline`, CSS `--k-consentGate-header-background`.
- **Silver 50% (#D1D1D180):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Amber (#FFAA00):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Red (#A15842):** Most used accent color, seen 3 times. Token `secondary`.
- **Vivid Red (#E84826):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Liga** and **Adventure** share the interface. Fallback stack: `Liga`.

- **headline-display:** Liga 360px at weight 500, line height 1, tracking -0.022em. Page title (h1).
- **headline-lg:** Adventure 72px at weight 600, line height 1, tracking -0.025em (44px on mobile). Section headings (h2).
- **headline-md:** Adventure 56px at weight 600, line height 1.07, tracking -0.045em. Sub-section headings.
- **headline-sm:** Adventure 36px at weight 600, line height 1.2, tracking -0.02em. Card and feature titles.
- **title-lg:** Adventure 32px at weight 400, line height 1.25. Small titles.
- **body-md:** Adventure 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Adventure 16px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** Adventure 10px at weight 400, line height 1.4. Secondary and small text.
- **label-md:** Adventure 16px at weight 500, line height 1.25, tracking -0.031em. Buttons, navigation and labels.
- **label-sm:** Adventure 14px at weight 500, line height 1.14, tracking -0.036em. Small labels and badges.

## Layout

Spacing follows a 4px grid: 96% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 40px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1920px.
- **Breakpoints:** 640px, 768px, 1024px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.15) 0px 2px 8px 0px`

## Shapes

Most elements use 40px corners. Measured radii, most used first:

- **xl (40px):** 132 elements.
- **full (9999px):** 32 elements.
- **md (12px):** 24 elements.
- **lg (36px):** 16 elements.
- **sm (4px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Demo drive”):** #FFAA00 fill, #000000 text, 14px/600, 9999px radius, padding 8px 16px.
- **button-secondary (“Accept All”):** #000000 fill, #FFFFFF text, 14px/600, 36px radius, padding 0px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-secondary-hover:** background #333333, text #FFFFFF on hover.
- **button-outline (“Explore more”):** #FFFFFF fill, #000000 text, 14px/500, 40px radius, padding 8px 16px.
- **button-ghost (“Manage Preferences”):** transparent fill, #000000 text, 14px/600, 36px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **input-field (“Email”):** #212121 fill, #FFFFFF text, 16px/400, 4px radius, padding 20px 16px 0px 16px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #ECECEC for the page and lift surfaces in small steps: #F2F2F2, #FFFFFF.
- Do keep text in 2 levels: #151515, #000000.
- Do reserve #FFAA00 for primary actions and key highlights.
- Do set headlines in Liga with tight tracking (-0.022em).
- Do keep spacing on the 4px grid.
- Do use 40px corners on most elements; larger surfaces also use 12px, 36px and 4px.
- Don't introduce new font families beyond Liga and Adventure.
- Don't use #FFAA00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.2s, 0.1s.

- **Easing:** `cubic-bezier(0.83, 0, 0.17, 1)`, `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/rivian.com/), the free DESIGN.md generator.
