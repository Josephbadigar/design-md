---
version: alpha
name: CodePen
description: "Dark interface measured from codepen.io: Telefon Black type with Lato, green accents, tonal surfaces and 4px corners."
colors:
  background: "#131417"
  surface: "#131417"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#B7BBC8"
  on-surface-muted: "#9B9DAD"
  on-surface-subtle: "#868CA0"
  surface-container-low: "#1E1F26"
  surface-container: "#010101"
  surface-container-high: "#252830"
  surface-container-highest: "#2C303AE6"
  outline: "#444857"
  primary: "#47CF73"
  on-primary: "#000000"
  inverse-surface: "#FFFFFFE6"
  secondary: "#1F798F"
  tertiary: "#76DAFF"
typography:
  headline-display:
    fontFamily: Telefon Black
    fontSize: 90px
    fontWeight: 400
    lineHeight: 1.1
  headline-lg:
    fontFamily: Telefon Black
    fontSize: 49px
    fontWeight: 800
    lineHeight: 1.15
  body-md:
    fontFamily: Lato
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Lato
    fontSize: 22.5px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Lato
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: Lato
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: Lato
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.2
  code:
    fontFamily: SFMono-Regular
    fontSize: 11px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.027em
  headline-display-mobile:
    fontFamily: Telefon Black
    fontSize: 39px
    fontWeight: 400
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: Telefon Black
    fontSize: 39px
    fontWeight: 800
    lineHeight: 1.15
rounded:
  xs: 1px
  sm: 4px
  md: 15px
  lg: 19.5px
  xl: 26.25px
spacing:
  xs: 3.26px
  sm: 8px
  md: 15px
  lg: 22.5px
  gutter: 11.25px
  section: 150px
  margin: 30px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10px 16px
    height: 42px
  button-primary-hover:
    backgroundColor: "#248C46"
    textColor: "{colors.on-surface}"
  button-secondary:
    backgroundColor: "{colors.outline}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10px 16px
    height: 38px
  button-secondary-hover:
    backgroundColor: "#5A5F73"
  button-outline:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10px 16px
    height: 44px
  input-field:
    textColor: "{colors.on-surface}"
    rounded: 3px
    padding: 6.6px 0px 6.6px 6.6px
  link:
    textColor: "{colors.secondary}"
---

# CodePen Design System

## Overview

CodePen describes itself as: “Build, share & learn with CodePen 2.0, the best community for developers with an all new online code editor featuring a file system, compiler, realtime & async collaboration, deployment, and more.” The interface is dark, built on **Charcoal (#131417)** with **White (#FFFFFF)** text, and **Green (#47CF73)** as the main accent.

Type is set in **Telefon Black** and **Lato**, with **SFMono-Regular** for code. Headlines run large; body text is 15px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [codepen.io](https://codepen.io/) on November 4, 2026 at 1440×900 and 390×844 from 266 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #FFDD40, #47CF73, #0EBEFF, #AE63E4.

- **Charcoal (#131417):** Page background, seen 2 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 31 times. Token `on-surface`, CSS `--cp-input-focus-bg`.
- **Cool Silver (#B7BBC8):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Cool Gray (#9B9DAD):** Muted text and metadata, seen 29 times. Token `on-surface-muted`, CSS `--cp-color-9`.
- **Blue (#868CA0):** Subtle text and placeholders, seen 4 times. Token `on-surface-subtle`, CSS `--cp-control-bar-color`.
- **Cool Charcoal (#1E1F26):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`, CSS `--cp-color-16`.
- **Near Black (#010101):** Cards and panels, seen 2 times. Token `surface-container`.
- **Cool Graphite (#252830):** Hover and pressed fills, seen 1 time. Token `surface-container-high`, CSS `--cp-modal-content-border`.
- **Cool Graphite 90% (#2C303AE6):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Dark Blue (#444857):** Borders and dividers, seen 1 time. Token `outline`, CSS `--cp-pen-header-button-hover-bg`.
- **Green (#47CF73):** Primary buttons and calls to action, seen 21 times. Token `primary`, CSS `--cp-color-posts`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **White 90% (#FFFFFFE6):** High-contrast fills, seen 9 times. Token `inverse-surface`.
- **Dark Cyan (#1F798F):** Accent in text, fills and borders, seen 28 times. Token `secondary`.
- **Light Cyan (#76DAFF):** Accent in text, fills and borders, seen 6 times. Token `tertiary`.

## Typography

**Telefon Black**, **Lato** and **SFMono-Regular** (monospace) share the interface. Fallback stack: `Telefon Black, sans-serif`. Other loaded fonts: Telefon.

- **headline-display:** Telefon Black 90px at weight 400, line height 1.1 (39px on mobile). Page title (h1).
- **headline-lg:** Telefon Black 49px at weight 800, line height 1.15 (39px on mobile). Section headings (h2).
- **body-md:** Lato 15px at weight 400, line height 1.5. Body text.
- **body-lg:** Lato 22.5px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** Lato 12px at weight 400, line height 1.5. Secondary and small text.
- **caption:** Lato 11px at weight 400, line height 1.4. Captions and fine print.
- **label-md:** Lato 15px at weight 700, line height 1.2. Buttons, navigation and labels.
- **code:** SFMono-Regular 11px at weight 600, line height 1.2, tracking -0.027em. Code and technical values.

## Layout

Spacing does not follow a strict grid: 23% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.26px, sm 8px, md 15px, lg 22.5px.
- **Sections:** 150px vertical padding between major sections.
- **Gaps:** 11.25px is the most common gap in flex and grid layouts.
- **Page margin:** 30px on each side of full-width sections.
- **Breakpoints:** 400px, 550px, 551px, 650px, 728px, 750px, 767px, 768px, 830px, 831px, 900px, 1100px, 1101px, 1408px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(10, 10, 12, 0.6) 0px 1px 3px 0px`
- `rgba(255, 255, 255, 0.2) 0px 1px 5px 0px`
- `rgba(0, 0, 0, 0.38) 0px 24px 80px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 72 elements.
- **xs (1px):** 16 elements.
- **lg (19.5px):** 8 elements.
- **xl (26.25px):** 8 elements.
- **md (15px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up”):** #47CF73 fill, #000000 text, 15px/400, 4px radius, padding 10px 16px.
- **button-primary-hover:** background #248C46, text #FFFFFF on hover.
- **button-secondary (“Try The Editor”):** #444857 fill, #FFFFFF text, 15px/400, 4px radius, padding 10px 16px.
- **button-secondary-hover:** background #5A5F73, text #FFFFFF on hover.
- **button-outline (“Log In”):** #252830 fill, #FFFFFF text, 15px/400, 4px radius, padding 10px 16px.
- **input-field (“Search CodePen...”):** transparent fill, #FFFFFF text, 16.5px/700, 3px radius, padding 6.6px 0px 6.6px 6.6px.
- **link:** transparent fill, #1F798F text, padding 0px.

## Do's and Don'ts

- Do use #131417 for the page and lift surfaces in small steps: #1E1F26, #010101, #252830, #2C303AE6.
- Do keep text in 4 levels: #FFFFFF, #B7BBC8, #9B9DAD, #868CA0.
- Do reserve #47CF73 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 15px, 22.5px).
- Do use 4px corners on most elements; larger surfaces also use 1px, 19.5px and 26.25px.
- Don't introduce new font families beyond Telefon Black, Lato and SFMono-Regular.
- Don't use #47CF73 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.2s, 0.125s, 0.3s, 0.4s. Longer ambient animations run 2s, 1.75s.

- **Easing:** `ease`, `ease-in-out`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/codepen.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
