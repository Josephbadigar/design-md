---
version: alpha
name: Primer
description: "Light interface measured from primer.style: Mona Sans type with Mona Sans VF, vivid blue accents, tonal surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#58635B"
  on-surface-muted: "#59636E"
  surface-container-low: "#F6F8FA"
  outline: "#D1D9E0"
  primary: "#0377FF"
  on-primary: "#000000"
  secondary: "#08872B"
  tertiary: "#0055D5"
typography:
  headline-display:
    fontFamily: Mona Sans
    fontSize: 56px
    fontWeight: 440
    lineHeight: 1.1
  headline-lg:
    fontFamily: Mona Sans
    fontSize: 34px
    fontWeight: 500
    lineHeight: 1.3
  headline-md:
    fontFamily: Mona Sans
    fontSize: 28px
    fontWeight: 480
    lineHeight: 1.35
  headline-sm:
    fontFamily: Mona Sans
    fontSize: 22px
    fontWeight: 480
    lineHeight: 1.4
  body-md:
    fontFamily: Mona Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Mona Sans VF
    fontSize: 14px
    fontWeight: 500
  headline-display-mobile:
    fontFamily: Mona Sans
    fontSize: 36px
    fontWeight: 440
    lineHeight: 1.2
  headline-lg-mobile:
    fontFamily: Mona Sans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.3
  headline-sm-mobile:
    fontFamily: Mona Sans
    fontSize: 20px
    fontWeight: 480
    lineHeight: 1.4
rounded:
  md: 6px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  gutter: 8px
  margin: 24px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#25292E"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 12px
    height: 32px
  button-outline-hover:
    backgroundColor: "#EFF2F5"
  link:
    textColor: "{colors.on-surface-muted}"
---

# Primer Design System

## Overview

Primer describes itself as: “The Design System for GitHub” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Blue (#0377FF)** as the main accent.

Type is set in **Mona Sans** and **Mona Sans VF**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 6px.

Measured from [primer.style](https://primer.style/) on November 4, 2026 at 1440×900 and 390×844 from 97 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 3 times. Token `background`, CSS `--bgColor-white`.
- **Near Black (#000000):** Primary text and headings, seen 9 times. Token `on-surface`, CSS `--brand-Testimonial-quote-color-default`.
- **Slate (#58635B):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Blue (#59636E):** Muted text and metadata, seen 5 times. Token `on-surface-muted`, CSS `--progressBar-bgColor-neutral`.
- **Snow (#F6F8FA):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Cool Silver (#D1D9E0):** Borders and dividers, seen 3 times. Token `outline`, CSS `--button-danger-borderColor-rest`.
- **Vivid Blue (#0377FF):** Brand accent (CSS variable), seen 1 time. Token `primary`, CSS `--brand-Eyebrowbanner-fgColor-green-blue-end`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Dark Green (#08872B):** Accent (CSS variable). Token `secondary`.
- **Blue (#0055D5):** Accent in text, fills and borders, seen 19 times. Token `tertiary`.

## Typography

**Mona Sans** and **Mona Sans VF** share the interface. Fallback stack: `Mona Sans, MonaSansFallback, -apple-system, BlinkMacSystemFont`.

- **headline-display:** Mona Sans 56px at weight 440, line height 1.1 (36px on mobile). Page title (h1).
- **headline-lg:** Mona Sans 34px at weight 500, line height 1.3 (24px on mobile). Section headings (h2).
- **headline-md:** Mona Sans 28px at weight 480, line height 1.35. Sub-section headings.
- **headline-sm:** Mona Sans 22px at weight 480, line height 1.4 (20px on mobile). Card and feature titles.
- **body-md:** Mona Sans 16px at weight 400, line height 1.5. Body text.
- **label-md:** Mona Sans VF 14px at weight 500. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 618px, 768px, 1012px, 1280px, 1300px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(31, 35, 40, 0.04) 0px 1px 0px 0px`

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Give feedback”):** #F6F8FA fill, #25292E text, 14px/500, 6px radius, padding 0px 12px, border 1px solid #D1D9E0, shadow `rgba(31, 35, 40, 0.04) 0px 1px 0px 0px`.
- **button-outline-hover:** background #EFF2F5, text #25292E on hover.
- **link:** transparent fill, #59636E text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F6F8FA.
- Do keep text in 3 levels: #000000, #58635B, #59636E.
- Do use #0377FF as the brand accent: header, logo and key highlights.
- Do keep spacing on the 4px grid.
- Do use 6px corners on most elements.
- Don't introduce new font families beyond Mona Sans and Mona Sans VF.
- Don't use #0377FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.08s, 0.2s.

- **Easing:** `cubic-bezier(0.65, 0, 0.35, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/primer.style/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
