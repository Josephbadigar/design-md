---
version: alpha
name: Descript
description: "Dark interface measured from descript.com: brett type with gamuthDisplay, vivid red accents, tonal surfaces and 5px corners."
colors:
  background: "#390A1A"
  surface: "#390A1A"
  on-surface: "#D1C7CB"
  on-background: "#D1C7CB"
  on-surface-strong: "#FFF8F4"
  on-surface-variant: "#FFF7FD"
  on-surface-muted: "#FFF7FA"
  surface-container-low: "#110A0D"
  surface-container: "#190308"
  surface-container-high: "#180101"
  surface-container-highest: "#4C343E"
  primary: "#F73B3B"
  on-primary: "#FFF7FD"
  inverse-surface: "#FFFFFF"
  secondary: "#772A4D"
  tertiary: "#5B142E"
typography:
  headline-display:
    fontFamily: brett
    fontSize: 72px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: gamuthDisplay
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.1
  headline-md:
    fontFamily: gamuthDisplay
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.1
  headline-sm:
    fontFamily: booton
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.3
  title-lg:
    fontFamily: brett
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0.04em
  body-md:
    fontFamily: booton
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Arial
    fontSize: 14px
    fontWeight: 400
  label-md:
    fontFamily: booton
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-lg-mobile:
    fontFamily: gamuthDisplay
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.1
rounded:
  sm: 5px
  md: 8px
  lg: 12px
  xl: 16px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 48px
  gutter: 8px
  section: 104px
  margin: 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 16px 32px
    height: 56px
  button-primary-hover:
    backgroundColor: "#B81B1E"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.inverse-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 16px 24px
    height: 54px
  button-secondary-hover:
    backgroundColor: "{colors.tertiary}"
  button-tertiary:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 14px 24px 14px 16px
    height: 44px
  button-ghost:
    textColor: "#C4B5BB"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 14px 24px 14px 16px
  card:
    backgroundColor: "{colors.background}"
    textColor: "#1A1A1A"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 48px
  link:
    textColor: "{colors.on-surface}"
---

# Descript Design System

## Overview

Descript describes itself as: “Descript is the AI video and audio editor that makes editing as easy as editing text. Record, transcribe, edit, and publish in one tool. Try it free.” The interface is dark, built on **Deep Pink (#390A1A)** with **Warm Silver (#D1C7CB)** text, and **Vivid Red (#F73B3B)** as the main accent.

Type is set in **brett** and **gamuthDisplay**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 5px.

Measured from [descript.com](https://www.descript.com/) on October 21, 2026 at 1440×900 and 390×844 from 356 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Deep Pink (#390A1A):** Page background, seen 21 times. Token `background`, CSS `--Maroon-900`.
- **Warm Silver (#D1C7CB):** Primary text and headings, seen 41 times. Token `on-surface`.
- **Warm Snow (#FFF8F4):** Headings and emphasis, seen 14 times. Token `on-surface-strong`, CSS `--Red-0`.
- **Snow (#FFF7FD):** Secondary text, seen 9 times. Token `on-surface-variant`, CSS `--Maroon-0`.
- **Warm Snow (#FFF7FA):** Muted text and metadata, seen 36 times. Token `on-surface-muted`.
- **Warm Charcoal (#110A0D):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Deep Red (#190308):** Cards and panels, seen 2 times. Token `surface-container`.
- **Deep Red (#180101):** Hover and pressed fills, seen 1 time. Token `surface-container-high`, CSS `--Red-950`.
- **Dark Pink (#4C343E):** Highest raised elements, seen 2 times. Token `surface-container-highest`, CSS `--Neutral-750`.
- **Vivid Red (#F73B3B):** Primary buttons and calls to action, seen 16 times. Token `primary`.
- **Snow (#FFF7FD):** Text and icons on primary. Token `on-primary`.
- **White (#FFFFFF):** High-contrast fills, seen 7 times. Token `inverse-surface`, CSS `--tw-ring-offset-color`.
- **Dark Pink (#772A4D):** Secondary buttons, seen 35 times. Token `secondary`, CSS `--Maroon-700`.
- **Deep Pink (#5B142E):** Secondary buttons, seen 17 times. Token `tertiary`.

## Typography

**brett**, **gamuthDisplay**, **booton** and **Arial** share the interface. Fallback stack: `brett, brett Fallback, system-ui, Roboto`. Other loaded fonts: booton Fallback, brett Fallback.

- **headline-display:** brett 72px at weight 400, line height 1, tracking -0.02em. Page title (h1).
- **headline-lg:** gamuthDisplay 56px at weight 700, line height 1.1 (40px on mobile). Section headings (h2).
- **headline-md:** gamuthDisplay 40px at weight 700, line height 1.1. Sub-section headings.
- **headline-sm:** booton 24px at weight 600, line height 1.3. Card and feature titles.
- **title-lg:** brett 18px at weight 400, line height 1, tracking 0.04em, uppercase. Small titles.
- **body-md:** booton 18px at weight 400, line height 1.4. Body text.
- **body-sm:** Arial 14px at weight 400. Secondary and small text.
- **label-md:** booton 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 48px.
- **Sections:** 104px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 64px on each side of full-width sections.
- **Breakpoints:** 475px, 640px, 767px, 768px, 1024px, 1120px, 1199px, 1280px, 1536px, 1800px, 2000px, 2200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.16) 0px 3px 3px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.16) 0px 2px 4px 0px`
- `rgba(0, 0, 0, 0.16) 0px 2px 4px 0px`

## Shapes

Most elements use 5px corners. Measured radii, most used first:

- **sm (5px):** 76 elements.
- **lg (12px):** 48 elements.
- **md (8px):** 24 elements.
- **xl (16px):** 20 elements.
- **full (9999px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started for free”):** #F73B3B fill, #FFF7FD text, 16px/400, 12px radius, padding 16px 32px.
- **button-primary-hover:** background #B81B1E, text #FFF7FD on hover.
- **button-secondary (“Sign up”):** #772A4D fill, #FFFFFF text, 16px/600, 12px radius, padding 16px 24px, shadow `rgba(0, 0, 0, 0.16) 0px 2px 4px 0px`.
- **button-secondary-hover:** background #5B142E, text #FFFFFF on hover.
- **button-tertiary (“Record”):** #5B142E fill, #FFF7FD text, 16px/600, 8px radius, padding 14px 24px 14px 16px.
- **button-ghost (“Edit”):** transparent fill, #C4B5BB text, 16px/400, 8px radius, padding 14px 24px 14px 16px.
- **card:** #390A1A fill, #1A1A1A text, 16px/400, 16px radius, padding 48px.
- **link:** transparent fill, #D1C7CB text, padding 0px.

## Do's and Don'ts

- Do use #390A1A for the page and lift surfaces in small steps: #110A0D, #190308, #180101, #4C343E.
- Do keep text in 4 levels: #D1C7CB, #FFF8F4, #FFF7FD, #FFF7FA.
- Do reserve #F73B3B for primary actions and key highlights.
- Do set headlines in brett with tight tracking (-0.02em).
- Do keep spacing on the 4px grid.
- Do use 5px corners on most elements; larger surfaces also use 12px, 8px and 16px.
- Don't introduce new font families beyond brett, gamuthDisplay, booton and Arial.
- Don't use #F73B3B for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.5s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/descript.com/), the free DESIGN.md generator.
