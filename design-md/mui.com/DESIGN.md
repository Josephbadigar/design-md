---
version: alpha
name: MUI
description: "Dark interface measured from mui.com: General Sans type with IBM Plex Sans, vivid blue accents, tonal surfaces and 18px corners."
colors:
  background: "#0F1214"
  surface: "#0F1214"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#CCE6FF"
  on-surface-muted: "#B6BEC9"
  on-surface-subtle: "#98A4B3"
  surface-container-low: "#303840"
  surface-container: "#3B3B3B"
  overlay: "#1D212633"
  overlay-strong: "#14171ACC"
  outline: "#1D2126"
  outline-variant: "#303840"
  primary: "#0073E6"
  on-primary: "#FFFFFF"
  secondary: "#3399FF"
  tertiary: "#66B3FF"
  success: "#21CA64"
  warning: "#FFEDA3"
typography:
  headline-display:
    fontFamily: General Sans
    fontSize: 56px
    fontWeight: 600
    lineHeight: 1.11
    letterSpacing: -0.004em
  headline-lg:
    fontFamily: General Sans
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.22
    letterSpacing: -0.006em
  headline-md:
    fontFamily: General Sans
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0.007em
  headline-sm:
    fontFamily: IBM Plex Sans
    fontSize: 24px
    fontWeight: 400
  title-lg:
    fontFamily: IBM Plex Sans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.5
  body-md:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-md:
    fontFamily: IBM Plex Sans
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.25
  label-sm:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: General Sans
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.11
    letterSpacing: -0.005em
  headline-lg-mobile:
    fontFamily: General Sans
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.22
    letterSpacing: -0.008em
rounded:
  sm: 1px
  md: 10px
  lg: 12px
  xl: 18px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 20px
  gutter: 16px
  container: 1200px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 10px 10px 12px
    height: 40px
  button-primary-hover:
    backgroundColor: "#0061C2"
  button-outline:
    backgroundColor: "#1D212666"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 1px 6px 1px 8px
    height: 32px
  button-outline-hover:
    backgroundColor: "{colors.outline}"
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 6px 8px
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-muted}"
---

# MUI Design System

## Overview

MUI describes itself as: “MUI provides a simple, customizable, and accessible library of React components. Follow your own design system, or start with Material Design.” The interface is dark, built on **Charcoal (#0F1214)** with **White (#FFFFFF)** text, and **Vivid Blue (#0073E6)** as the main accent.

Type is set in **General Sans** and **IBM Plex Sans**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 18px.

Measured from [mui.com](https://mui.com/) on October 21, 2026 at 1440×900 and 390×844 from 355 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles, plus gradient stops #3399FF, #004D99, #F5C400, #AD6800.

- **Charcoal (#0F1214):** Page background, seen 1 time. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 32 times. Token `on-surface`, CSS `--font-color-onDark`.
- **Pale Blue (#CCE6FF):** Secondary text, seen 36 times. Token `on-surface-variant`.
- **Light Blue (#B6BEC9):** Muted text and metadata, seen 38 times. Token `on-surface-muted`.
- **Blue (#98A4B3):** Subtle text and placeholders, seen 9 times. Token `on-surface-subtle`, CSS `--muidocs-palette-text-tertiary`.
- **Cool Graphite (#303840):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Graphite (#3B3B3B):** Cards and panels, seen 2 times. Token `surface-container`.
- **Cool Charcoal 20% (#1D212633):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Cool Charcoal 80% (#14171ACC):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Cool Charcoal (#1D2126):** Borders and dividers, seen 8 times. Token `outline`.
- **Cool Graphite (#303840):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **Vivid Blue (#0073E6):** Primary buttons and calls to action, seen 5 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#3399FF):** Most used accent color, seen 16 times. Token `secondary`.
- **Blue (#66B3FF):** Most used accent color, seen 15 times. Token `tertiary`.
- **Green (#21CA64):** Success and positive states, seen 6 times. Token `success`.
- **Light Amber (#FFEDA3):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**General Sans** and **IBM Plex Sans** share the interface. Fallback stack: `General Sans, -apple-system, BlinkMacSystemFont, Segoe UI`. Other loaded fonts: Roboto.

- **headline-display:** General Sans 56px at weight 600, line height 1.11, tracking -0.004em (40px on mobile). Page title (h1).
- **headline-lg:** General Sans 36px at weight 600, line height 1.22, tracking -0.006em (24px on mobile). Section headings (h2).
- **headline-md:** General Sans 30px at weight 600, line height 1.5, tracking 0.007em. Sub-section headings.
- **headline-sm:** IBM Plex Sans 24px at weight 400. Card and feature titles.
- **title-lg:** IBM Plex Sans 20px at weight 600, line height 1.5. Small titles.
- **body-md:** IBM Plex Sans 14px at weight 400, line height 1.5. Body text.
- **body-lg:** IBM Plex Sans 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-lg:** IBM Plex Sans 16px at weight 600, line height 1.5. Large buttons and tabs.
- **label-md:** IBM Plex Sans 15px at weight 500, line height 1.25. Buttons, navigation and labels.
- **label-sm:** IBM Plex Sans 14px at weight 600, line height 1.5. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 54% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 16px, lg 20px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1200px.
- **Breakpoints:** 0px, 599.95px, 600px, 768px, 900px, 1200px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(48, 56, 64, 0.3) 0px 1px 0px 0px inset, rgb(9, 11, 11) 0px -1px 0px 0px inset, rgb(9, 11, 11) 0px 1px 2px 0px`
- `rgba(29, 33, 38, 0.4) 0px 2px 0px 0px inset, rgb(9, 11, 11) 0px -2px 0px 0px inset, rgb(9, 11, 11) 0px 1px 2px 0px`
- `rgba(9, 11, 11, 0.2) 0px -3px 1px 0px inset, rgb(15, 18, 20) 0px 2px 3px 0px`

## Shapes

Most elements use 18px corners. Measured radii, most used first:

- **xl (18px):** 124 elements.
- **lg (12px):** 116 elements.
- **sm (1px):** 44 elements.
- **full (9999px):** 20 elements.
- **md (10px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Discover the Core libraries”):** #0073E6 fill, #FFFFFF text, 15px/500, 10px radius, padding 8px 10px 10px 12px, border 1px solid #006BD6, shadow `rgba(51, 153, 255, 0.5) 0px 1px 0px 0px inset, rgba(0, 77, 153, 0.4) 0px -1px 0px 1px inset, rgba(9, 11, 11, 0.1) 0px 2px 4px 0px`.
- **button-primary-hover:** background #0061C2, text #FFFFFF on hover.
- **button-outline (“Search… Ctrl+K”):** #1D212666 fill, #B6BEC9 text, 14px/400, 12px radius, padding 1px 6px 1px 8px, border 1px solid #30384066, shadow `rgba(48, 56, 64, 0.1) 0px 1px 0px 0px inset, rgb(9, 11, 11) 0px -1px 0px 0px inset, rgb(9, 11, 11) 0px 1px 2px 0px`.
- **button-outline-hover:** background #1D2126, text #B6BEC9 on hover.
- **button-ghost (“Products”):** transparent fill, #B6BEC9 text, 14px/600, 12px radius, padding 6px 8px.
- **input-field (“Temperature”):** #3B3B3B fill, #FFFFFF text, 13.3333px/400, padding 0px.
- **link:** transparent fill, #B6BEC9 text, padding 0px.

## Do's and Don'ts

- Do use #0F1214 for the page and lift surfaces in small steps: #303840, #3B3B3B.
- Do keep text in 4 levels: #FFFFFF, #CCE6FF, #B6BEC9, #98A4B3.
- Do reserve #0073E6 for primary actions and key highlights.
- Do set headlines in General Sans with tight tracking (-0.004em).
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 18px corners on most elements; larger surfaces also use 12px, 1px and 10px.
- Don't introduce new font families beyond General Sans and IBM Plex Sans.
- Don't use #0073E6 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.25s, 0.1s, 0.2s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mui.com/), the free DESIGN.md generator.
