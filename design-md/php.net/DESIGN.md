---
version: alpha
name: PHP
description: "Dark interface measured from php.net: Fira Sans type, indigo accents, flat surfaces and 30px corners."
colors:
  background: "#333333"
  surface: "#333333"
  on-surface: "#CCCCCC"
  on-background: "#CCCCCC"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#DBE1FF"
  on-surface-muted: "#666666"
  outline: "#336699"
  outline-variant: "#793862"
  primary: "#4F5B93"
  on-primary: "#FFFFFF"
  inverse-surface: "#F2F2F2"
  secondary: "#90A0D0"
typography:
  headline-display:
    fontFamily: Fira Sans
    fontSize: 24px
    fontWeight: 400
    lineHeight: 2
  headline-lg:
    fontFamily: Fira Sans
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
  body-md:
    fontFamily: Fira Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.71
  body-lg:
    fontFamily: Fira Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: Fira Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.7
  label-sm:
    fontFamily: Fira Sans
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.71
rounded:
  sm: 8px
  md: 30px
spacing:
  base: 8px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.headline-lg}"
    rounded: "{rounded.md}"
    padding: 16px 32px
    height: 58px
  button-primary-hover:
    backgroundColor: "{colors.outline-variant}"
  button-secondary:
    backgroundColor: "#404F82"
    textColor: "#B9C3F4"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 8px
    height: 40px
  button-outline:
    textColor: "#B8C0E9"
    typography: "{typography.headline-lg}"
    rounded: "{rounded.md}"
    padding: 16px 32px
    height: 58px
  button-ghost:
    textColor: "#B8C0E9"
    typography: "{typography.headline-lg}"
    rounded: "{rounded.md}"
    padding: 16px 32px
  link:
    textColor: "{colors.outline}"
---

# PHP Design System

## Overview

The interface is dark, built on **Graphite (#333333)** with **Silver (#CCCCCC)** text, and **Indigo (#4F5B93)** as the main accent.

Type is set in **Fira Sans**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 30px.

Measured from [php.net](https://www.php.net/) on November 4, 2026 at 1440×900 and 390×844 from 339 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **Graphite (#333333):** Page background, seen 1 time. Token `background`, CSS `--content-text-color`.
- **Silver (#CCCCCC):** Primary text and headings, seen 13 times. Token `on-surface`, CSS `--background-text-color`.
- **White (#FFFFFF):** Headings and emphasis, seen 13 times. Token `on-surface-strong`.
- **Pale Indigo (#DBE1FF):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Slate (#666666):** Muted text and metadata, seen 16 times. Token `on-surface-muted`.
- **Blue (#336699):** Borders and dividers, seen 63 times. Token `outline`.
- **Dark Pink (#793862):** Secondary dividers, seen 25 times. Token `outline-variant`, CSS `--dark-magenta-color`.
- **Indigo (#4F5B93):** Primary buttons and calls to action, seen 2 times. Token `primary`, CSS `--dark-blue-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Mist (#F2F2F2):** High-contrast fills, seen 1 time. Token `inverse-surface`, CSS `--content-background-color`.
- **Blue (#90A0D0):** Accent, seen 2 times. Token `secondary`.

## Typography

**Fira Sans** carries the whole interface. Fallback stack: `Fira Sans, Source Sans Pro, ui-sans-serif, system-ui`. Other loaded fonts: Fira Mono, fontello.

- **headline-display:** Fira Sans 24px at weight 400, line height 2. Page title (h1).
- **headline-lg:** Fira Sans 20px at weight 400, line height 1.2. Section headings (h2).
- **body-md:** Fira Sans 14px at weight 400, line height 1.71. Body text.
- **body-lg:** Fira Sans 18px at weight 400, line height 1.33. Lead paragraphs.
- **label-md:** Fira Sans 16px at weight 400, line height 1.7. Buttons, navigation and labels.
- **label-sm:** Fira Sans 14px at weight 600, line height 1.71. Small labels and badges.

## Layout

Spacing follows a 8px grid: 97% of measured gaps and paddings are multiples of 8px.

- **Scale:** sm 8px, md 16px, lg 24px, xl 48px.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Breakpoints:** 425px, 465px, 480px, 540px, 760px, 767px, 768px, 784px, 979px, 980px, 992px, 1200px, 1500px, 1548px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.2) 0px 2px 4px 0px`

## Shapes

Most elements use 30px corners. Measured radii, most used first:

- **md (30px):** 8 elements.
- **sm (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“What's new in 8.5”):** #4F5B93 fill, #FFFFFF text, 20px/400, 30px radius, padding 16px 32px.
- **button-primary-hover:** background #793862, text #FFFFFF on hover.
- **button-secondary (“Search docs”):** #404F82 fill, #B9C3F4 text, 16px/400, 8px radius, padding 8px, border 1px solid #6A78BE.
- **button-outline (“Download”):** transparent fill, #B8C0E9 text, 20px/400, 30px radius, padding 16px 32px, border 1px solid #6773AD.
- **button-ghost (“Download”):** transparent fill, #B8C0E9 text, 20px/400, 30px radius, padding 16px 32px, border 1px solid #6773AD.
- **link:** transparent fill, #336699 text, padding 0px.

## Do's and Don'ts

- Do use #333333 for the page.
- Do keep text in 4 levels: #CCCCCC, #FFFFFF, #DBE1FF, #666666.
- Do reserve #4F5B93 for primary actions and key highlights.
- Do keep spacing on the 8px grid.
- Do use 30px corners on most elements; larger surfaces also use 8px.
- Don't use #666666 for body text; it reaches 2.20:1 on #333333. Keep it for large text or metadata.
- Don't introduce new font families beyond Fira Sans.
- Don't use #4F5B93 for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.25s, 0.2s.

- **Easing:** `ease-out`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/php.net/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
