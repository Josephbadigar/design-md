---
version: alpha
name: Plain
description: "Light interface measured from plain.com: ABC Favorit Regular type with ABC Favorit Medium, teal accents, flat surfaces and 6px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#0A2414"
  on-surface-muted: "#607066"
  outline: "#1AD379"
  primary: "#1AD379"
  on-primary: "#F3FBE9"
  success: "#17B267"
  error: "#FFBAC3"
typography:
  headline-display:
    fontFamily: ABC Favorit Regular
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: ABC Favorit Regular
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: -0.02em
  headline-md:
    fontFamily: ABC Favorit Regular
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.17
    letterSpacing: -0.02em
  body-md:
    fontFamily: ABC Favorit Regular
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.01em
  body-lg:
    fontFamily: ABC Favorit Medium
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.01em
  body-sm:
    fontFamily: sans-serif
    fontSize: 12px
    fontWeight: 400
  label-md:
    fontFamily: ABC Favorit Medium
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.01em
  code:
    fontFamily: Geist Mono
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.46
    letterSpacing: 0.015em
  headline-display-mobile:
    fontFamily: ABC Favorit Regular
    fontSize: 46px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: ABC Favorit Regular
    fontSize: 31px
    fontWeight: 400
    lineHeight: 1.16
    letterSpacing: -0.02em
rounded:
  md: 6px
spacing:
  sm: 8px
  md: 10px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 8px 10px 7px 10px
    height: 34px
  button-primary-hover:
    backgroundColor: "{colors.success}"
  link:
    textColor: "{colors.success}"
---

# Plain Design System

## Overview

Plain describes itself as: “Plain is the AI support stack built for B2B teams. Composable infrastructure that gives you complete flexibility to build a support motion that grows with your business — no-code or all-code.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Teal (#1AD379)** as the main accent.

Type is set in **ABC Favorit Regular** and **ABC Favorit Medium**, with **Geist Mono** for code. Headlines run large with tight negative tracking; body text is 15px. The surface language is flat. Corners are mostly 6px.

Measured from [plain.com](https://www.plain.com/) on October 29, 2026 at 1440×900 and 390×844 from 299 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 24 times. Token `on-surface`.
- **Deep Green (#0A2414):** Secondary text, seen 51 times. Token `on-surface-variant`.
- **Slate (#607066):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Teal (#1AD379):** Borders and dividers, seen 3 times. Token `outline`.
- **Teal (#1AD379):** Primary buttons and calls to action, seen 24 times. Token `primary`.
- **Pale Lime (#F3FBE9):** Text and icons on primary. Token `on-primary`.
- **Teal (#17B267):** Success and positive states, seen 34 times. Token `success`.
- **Pale Red (#FFBAC3):** Errors and destructive states, seen 4 times. Token `error`.

## Typography

**ABC Favorit Regular**, **ABC Favorit Medium**, **sans-serif** and **Geist Mono** (monospace) share the interface. Fallback stack: `ABC Favorit Regular, ABC Favorit Regular Placeholder, sans-serif`.

- **headline-display:** ABC Favorit Regular 80px at weight 400, line height 1, tracking -0.02em (46px on mobile). Page title (h1).
- **headline-lg:** ABC Favorit Regular 48px at weight 400, line height 1.04, tracking -0.02em (31px on mobile). Section headings (h2).
- **headline-md:** ABC Favorit Regular 24px at weight 400, line height 1.17, tracking -0.02em. Sub-section headings.
- **body-md:** ABC Favorit Regular 15px at weight 400, line height 1.33, tracking -0.01em. Body text.
- **body-lg:** ABC Favorit Medium 18px at weight 500, line height 1.33, tracking -0.01em. Lead paragraphs.
- **body-sm:** sans-serif 12px at weight 400. Secondary and small text.
- **label-md:** ABC Favorit Medium 15px at weight 500, line height 1.33, tracking -0.01em. Buttons, navigation and labels.
- **code:** Geist Mono 13px at weight 500, line height 1.46, tracking 0.015em. Code and technical values.

## Layout

Spacing does not follow a strict grid: 57% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 8px, md 10px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 576px, 798.98px, 799px, 959px, 959.98px, 960px, 1069px, 1069.98px, 1199px, 1249px, 1272px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #1AD379 borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 44 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“BOOK A DEMO”):** #1AD379 fill, #F3FBE9 text, 12px/400, 6px radius, padding 8px 10px 7px 10px.
- **button-primary-hover:** background #17B267, text #F3FBE9 on hover.
- **link:** transparent fill, #17B267 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #000000, #0A2414, #607066.
- Do reserve #1AD379 for primary actions and key highlights.
- Do set headlines in ABC Favorit Regular with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 10px).
- Do use 6px corners on most elements.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond ABC Favorit Regular, ABC Favorit Medium, sans-serif and Geist Mono.
- Don't use #1AD379 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.4s.

- **Easing:** `cubic-bezier(0.44, 0, 0.56, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/plain.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
