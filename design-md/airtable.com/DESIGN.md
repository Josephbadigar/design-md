---
version: alpha
name: Airtable
description: "Light interface measured from airtable.com: ATSeasonSans type with SF Pro Text, red accents, tonal surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#2E2F32"
  on-background: "#2E2F32"
  on-surface-strong: "#181D26"
  on-surface-variant: "#1D1F25"
  on-surface-muted: "#979AA0"
  surface-container-low: "#EEF0F4"
  surface-container: "#E0DAFD"
  overlay: "#FFFFFF1F"
  overlay-strong: "#FFFFFF38"
  outline: "#1D1F251A"
  outline-variant: "#0000000D"
  primary: "#944D37"
  on-primary: "#FFFFFF"
  inverse-surface: "#161616"
  secondary: "#5AA2FF"
  tertiary: "#CADCFF"
  warning: "#A26811"
  success: "#048A0E"
typography:
  headline-display:
    fontFamily: ATSeasonSans
    fontSize: 58.5px
    fontWeight: 550
    lineHeight: 1.1
  headline-lg:
    fontFamily: ATSeasonSans
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.15
  headline-md:
    fontFamily: ATSeasonSans
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.5
  headline-sm:
    fontFamily: ATSeasonSans
    fontSize: 20px
    fontWeight: 550
    lineHeight: 1.5
    letterSpacing: 0.005em
  body-md:
    fontFamily: ATSeasonSans
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.35
  body-sm:
    fontFamily: SF Pro Text
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.54
  label-lg:
    fontFamily: ATSeasonSans
    fontSize: 16px
    fontWeight: 550
    lineHeight: 1.35
    letterSpacing: 0.01em
  label-md:
    fontFamily: SF Pro Text
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1
  label-sm:
    fontFamily: ATSeasonSans
    fontSize: 14.5px
    fontWeight: 550
    lineHeight: 1.3
  headline-display-mobile:
    fontFamily: ATSeasonSans
    fontSize: 48px
    fontWeight: 550
    lineHeight: 1.15
  headline-lg-mobile:
    fontFamily: ATSeasonSans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.15
rounded:
  sm: 4px
  md: 6px
  lg: 100px
  full: 9999px
spacing:
  xs: 2px
  sm: 6px
  md: 10px
  lg: 18px
  xl: 48px
  gutter: 8px
  section: 48px
components:
  button-primary:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 12px 24px
    height: 46px
  button-secondary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
    height: 37px
  button-secondary-hover:
    backgroundColor: "#040E20B0"
  button-outline:
    textColor: "{colors.inverse-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 12px 24px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "#333840"
---

# Airtable Design System

## Overview

Airtable describes itself as: “500,000+ brands use Airtable to enable real-time collaboration, automate repetitive tasks & manual work, and streamline business processes in minutes. Join them.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#2E2F32)** text, and **Red (#944D37)** as the main accent.

Type is set in **ATSeasonSans** and **SF Pro Text**. Headlines run large; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 6px.

Measured from [airtable.com](https://www.airtable.com/) on October 21, 2026 at 1440×900 and 390×844 from 354 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 18 roles.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`, CSS `--color-text-inverse-primary`.
- **Graphite (#2E2F32):** Primary text and headings, seen 37 times. Token `on-surface`.
- **Cool Charcoal (#181D26):** Headings and emphasis, seen 8 times. Token `on-surface-strong`, CSS `--color-icon-primary`.
- **Cool Charcoal (#1D1F25):** Secondary text, seen 7 times. Token `on-surface-variant`.
- **Cool Gray (#979AA0):** Muted text and metadata, seen 8 times. Token `on-surface-muted`.
- **Cool Mist (#EEF0F4):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Pale Indigo (#E0DAFD):** Cards and panels, seen 3 times. Token `surface-container`.
- **White 12% (#FFFFFF1F):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **White 22% (#FFFFFF38):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Cool Charcoal 10% (#1D1F251A):** Borders and dividers, seen 1 time. Token `outline`.
- **Near Black 5% (#0000000D):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Red (#944D37):** Brand color on large areas, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#161616):** High-contrast fills, seen 2 times. Token `inverse-surface`.
- **Blue (#5AA2FF):** Brand accent (CSS variable), seen 12 times. Token `secondary`.
- **Pale Blue (#CADCFF):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.
- **Dark Orange (#A26811):** Warnings and highlights, seen 2 times. Token `warning`.
- **Dark Green (#048A0E):** Success and positive states, seen 2 times. Token `success`.

## Typography

**ATSeasonSans** and **SF Pro Text** share the interface. Fallback stack: `ATSeasonSans, -apple-system, BlinkMacSystemFont, sans-serif`. Other loaded fonts: Haas, Haas Groot Disp, Source Sans 3.

- **headline-display:** ATSeasonSans 58.5px at weight 550, line height 1.1 (48px on mobile). Page title (h1).
- **headline-lg:** ATSeasonSans 48px at weight 500, line height 1.15 (32px on mobile). Section headings (h2).
- **headline-md:** ATSeasonSans 32px at weight 600, line height 1.5. Sub-section headings.
- **headline-sm:** ATSeasonSans 20px at weight 550, line height 1.5, tracking 0.005em. Card and feature titles.
- **body-md:** ATSeasonSans 18px at weight 500, line height 1.35. Body text.
- **body-sm:** SF Pro Text 13px at weight 400, line height 1.54. Secondary and small text.
- **label-lg:** ATSeasonSans 16px at weight 550, line height 1.35, tracking 0.01em. Large buttons and tabs.
- **label-md:** SF Pro Text 15px at weight 500, line height 1. Buttons, navigation and labels.
- **label-sm:** ATSeasonSans 14.5px at weight 550, line height 1.3. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 38% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 6px, md 10px, lg 18px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 768px, 1024px, 1080px, 1319px, 1536px, 1600px, 1664px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.32) 0px 0px 0.5px 0px, rgba(0, 0, 0, 0.08) 0px 0px 1px 0px, rgba(0, 0, 0, 0.08) 0px 1px 1.5px 0px, rgba(0, 0, 0, 0.06) 0px 0px 0px 0.5px`
- `rgba(15, 48, 106, 0.05) 0px 0px 20px 0px`

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 60 elements.
- **lg (100px):** 60 elements.
- **full (9999px):** 28 elements.
- **sm (4px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start building for free”):** #161616 fill, #FFFFFF text, 16px/650, 4px radius, padding 12px 24px.
- **button-secondary (“Sign up for free”):** #181D26 fill, #FFFFFF text, 14px/550, 4px radius, padding 8px 16px, border 1px solid #181D26.
- **button-secondary-hover:** background #040E20B0, text #FFFFFF on hover.
- **button-outline (“Book a demo”):** transparent fill, #161616 text, 16px/650, 4px radius, padding 12px 24px, border 1px solid #161616.
- **button-ghost (“Platform”):** transparent fill, #181D26 text, 14px/550, padding 0px.
- **link:** transparent fill, #333840 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EEF0F4, #E0DAFD.
- Do keep text in 4 levels: #2E2F32, #181D26, #1D1F25, #979AA0.
- Do use #944D37 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (6px, 10px, 18px).
- Do use 6px corners on most elements; larger surfaces also use 100px and 4px.
- Don't use #979AA0 for body text; it reaches 2.8:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond ATSeasonSans and SF Pro Text.
- Don't use #944D37 for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.001s, 0.25s.

- **Easing:** `ease`, `cubic-bezier(0.2, 0.9, 0.3, 1.2)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/airtable.com/), the free DESIGN.md generator.
