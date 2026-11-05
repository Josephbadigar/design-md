---
version: alpha
name: Laravel
description: "Light interface measured from laravel.com: InstrumentSans type, vivid red accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#737373"
  on-background: "#737373"
  on-surface-strong: "#000000"
  on-surface-variant: "#11181C"
  on-surface-muted: "#171717"
  surface-container-low: "#FAFAFA"
  surface-container: "#F5F5F5"
  outline: "#E5E5E5"
  outline-variant: "#D4D4D4"
  primary: "#F53003"
  on-primary: "#FFFFFF"
  secondary: "#F61500"
  tertiary: "#2563EB"
typography:
  headline-display:
    fontFamily: InstrumentSans
    fontSize: 72px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: InstrumentSans
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.05em
  headline-md:
    fontFamily: InstrumentSans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: InstrumentSans
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.025em
  body-md:
    fontFamily: InstrumentSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: InstrumentSans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
    letterSpacing: -0.025em
  body-sm:
    fontFamily: InstrumentSans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  caption:
    fontFamily: InstrumentSans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-lg:
    fontFamily: InstrumentSans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: InstrumentSans
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.025em
  label-sm:
    fontFamily: InstrumentSans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  code:
    fontFamily: IBM Plex Mono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: InstrumentSans
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.11
    letterSpacing: -0.05em
  headline-lg-mobile:
    fontFamily: InstrumentSans
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.11
    letterSpacing: -0.05em
rounded:
  sm: 6px
  md: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 24px
  xl: 36px
  gutter: 10px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 0px 24px
    height: 48px
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.headline-lg}"
    padding: 4px
    height: 45px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 10px 16px
    height: 43px
  button-ghost:
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 8px 0px 12px
  link:
    textColor: "{colors.on-surface}"
---

# Laravel Design System

## Overview

Laravel describes itself as: “Laravel is a framework for building modern web apps and AI agents. Expressive syntax, built-in tools, and everything you need to ship fast.” The interface is light, built on **White (#FFFFFF)** with **Slate (#737373)** text, and **Vivid Red (#F53003)** as the main accent.

Type is set in **InstrumentSans**, with **IBM Plex Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [laravel.com](https://laravel.com/) on November 4, 2026 at 1440×900 and 390×844 from 398 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 16 times. Token `background`, CSS `--color-white`.
- **Slate (#737373):** Primary text and headings, seen 60 times. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 15 times. Token `on-surface-strong`, CSS `--tw-mask-bottom-from-color`.
- **Cool Charcoal (#11181C):** Secondary text, seen 8 times. Token `on-surface-variant`, CSS `--text-strong-color`.
- **Charcoal (#171717):** Muted text and metadata, seen 48 times. Token `on-surface-muted`.
- **Snow (#FAFAFA):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F5F5F5):** Cards and panels, seen 1 time. Token `surface-container`.
- **Mist (#E5E5E5):** Borders and dividers, seen 14 times. Token `outline`.
- **Silver (#D4D4D4):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Vivid Red (#F53003):** Primary buttons and calls to action, seen 45 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Red (#F61500):** Accent on large areas. Token `secondary`.
- **Vivid Blue (#2563EB):** Accent on large areas, seen 11 times. Token `tertiary`.

## Typography

**InstrumentSans** and **IBM Plex Mono** (monospace) share the interface. Fallback stack: `InstrumentSans, ui-sans-serif, system-ui, sans-serif`.

- **headline-display:** InstrumentSans 72px at weight 400, line height 1, tracking -0.05em (36px on mobile). Page title (h1).
- **headline-lg:** InstrumentSans 60px at weight 400, line height 1, tracking -0.05em (36px on mobile). Section headings (h2).
- **headline-md:** InstrumentSans 24px at weight 500, line height 1.33, tracking -0.025em. Sub-section headings.
- **headline-sm:** InstrumentSans 20px at weight 400, line height 1.4, tracking -0.025em. Card and feature titles.
- **body-md:** InstrumentSans 16px at weight 400, line height 1.5. Body text.
- **body-lg:** InstrumentSans 18px at weight 400, line height 1.56, tracking -0.025em. Lead paragraphs.
- **body-sm:** InstrumentSans 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** InstrumentSans 12px at weight 400, line height 1.33. Captions and fine print.
- **label-lg:** InstrumentSans 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** InstrumentSans 15px at weight 500, line height 1.5, tracking -0.025em. Buttons, navigation and labels.
- **label-sm:** InstrumentSans 14px at weight 500, line height 1.43. Small labels and badges.
- **code:** IBM Plex Mono 14px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (77% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 10px, lg 24px, xl 36px.
- **Gaps:** 10px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.03) 0px 0px 1px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`
- `rgba(0, 0, 0, 0.25) 0px 0px 4px 0px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(245, 48, 3, 0.5) 0px 0px 44px 0px, rgba(245, 48, 3, 0.5) 0px 0px 8px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 68 elements.
- **sm (6px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Deploy on Cloud”):** #F53003 fill, #FFFFFF text, 18px/400, 8px radius, padding 0px 24px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.03) 0px 0px 1px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`.
- **button-secondary (“Toggle AI”):** #F53003 fill, #171717 text, 60px/400, 3.35544e+07px radius, padding 4px, shadow `rgba(0, 0, 0, 0.25) 0px 0px 4px 0px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(245, 48, 3, 0.5) 0px 0px 44px 0px, rgba(245, 48, 3, 0.5) 0px 0px 8px 0px`.
- **button-outline (“UserController.php”):** #FAFAFA fill, #171717 text, 14px/400, padding 10px 16px.
- **button-ghost (“Framework”):** transparent fill, 15px/500, 8px radius, padding 0px 8px 0px 12px.
- **link:** transparent fill, #737373 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFA, #F5F5F5.
- Do keep text in 4 levels: #737373, #000000, #11181C, #171717.
- Do reserve #F53003 for primary actions and key highlights.
- Do set headlines in InstrumentSans with tight tracking (-0.05em).
- Do reuse the measured spacing steps (8px, 10px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 6px.
- Don't introduce new font families beyond InstrumentSans and IBM Plex Mono.
- Don't use #F53003 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.1s, 0.15s, 0.05s, 0.3s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/laravel.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
