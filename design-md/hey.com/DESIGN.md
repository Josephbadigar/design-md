---
version: alpha
name: HEY
description: "Dark interface measured from hey.com: Really Sans Large type with Moniker, light indigo accents, tonal surfaces and 43.68px corners."
colors:
  background: "#202C38"
  surface: "#202C38"
  on-surface: "#ECE9E6"
  on-background: "#ECE9E6"
  on-surface-strong: "#FFFFFF"
  surface-container-low: "#17212B"
  surface-container: "#333C47"
  primary: "#8C85FF"
  on-primary: "#000000"
typography:
  headline-display:
    fontFamily: Really Sans Large
    fontSize: 83px
    fontWeight: 900
    lineHeight: 1.1
  headline-lg:
    fontFamily: Really Sans Large
    fontSize: 48px
    fontWeight: 850
    lineHeight: 1.1
  headline-md:
    fontFamily: Really Sans Large
    fontSize: 40px
    fontWeight: 850
    lineHeight: 1.2
  headline-sm:
    fontFamily: Moniker
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.013em
  body-md:
    fontFamily: Moniker
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.013em
  body-lg:
    fontFamily: Moniker
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.45
    letterSpacing: -0.012em
  body-sm:
    fontFamily: Moniker
    fontSize: 17.5px
    fontWeight: 500
    lineHeight: 1.45
    letterSpacing: -0.012em
  label-md:
    fontFamily: Moniker
    fontSize: 21px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.013em
  label-sm:
    fontFamily: Moniker
    fontSize: 14.5px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.012em
  headline-display-mobile:
    fontFamily: Really Sans Large
    fontSize: 44px
    fontWeight: 900
    lineHeight: 1.1
  headline-md-mobile:
    fontFamily: Really Sans Large
    fontSize: 25px
    fontWeight: 850
    lineHeight: 1.2
  headline-lg-mobile:
    fontFamily: Really Sans Large
    fontSize: 30px
    fontWeight: 850
    lineHeight: 1.1
rounded:
  xs: 20.88px
  sm: 25.6px
  md: 43.68px
  lg: 57.2px
  xl: 74.8px
spacing:
  xs: 3.2px
  md: 10.4px
  lg: 18.72px
  xl: 33.6px
  gutter: 19.2px
  section: 90px
  margin: 32px
components:
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.xs}"
    padding: 4.32px 15.84px 4.32px 4.32px
    height: 42px
  button-secondary:
    textColor: "{colors.on-surface-strong}"
    rounded: "{rounded.xl}"
    padding: 23.8px 29.92px
    height: 62px
  button-tertiary:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 16.64px 21.32px
    height: 46px
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 16.64px 21.32px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 0px 0px 0px 21.6px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-sm}"
    rounded: "{rounded.sm}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# HEY Design System

## Overview

HEY describes itself as: “Gmail, Outlook, and Apple got complacent and took their eye off the ball. Then along came HEY.” The interface is dark, built on **Deep Blue (#202C38)** with **Warm Mist (#ECE9E6)** text, and **Light Indigo (#8C85FF)** as the main accent.

Type is set in **Really Sans Large** and **Moniker**. Headlines run large; body text is 21px. Depth comes from soft drop shadows. Corners are mostly 43.68px.

Measured from [hey.com](https://www.hey.com/) on October 21, 2026 at 1440×900 and 390×844 from 195 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles, plus gradient stops #867EFF, #DE8983, #5522FA, #EC8580.

- **Deep Blue (#202C38):** Page background, seen 12 times. Token `background`, CSS `--color-surface`.
- **Warm Mist (#ECE9E6):** Primary text and headings, seen 88 times. Token `on-surface`, CSS `--color-ink`.
- **White (#FFFFFF):** Headings and emphasis, seen 7 times. Token `on-surface-strong`, CSS `--color-white`.
- **Deep Blue (#17212B):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Dark Blue (#333C47):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--color-stone`.
- **Light Indigo (#8C85FF):** Most used accent color, seen 10 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.

## Typography

**Really Sans Large** and **Moniker** share the interface. Fallback stack: `Really Sans Large, sans-serif`. Other loaded fonts: Shantell Sans.

- **headline-display:** Really Sans Large 83px at weight 900, line height 1.1 (44px on mobile). Page title (h1).
- **headline-lg:** Really Sans Large 48px at weight 850, line height 1.1 (30px on mobile). Section headings (h2).
- **headline-md:** Really Sans Large 40px at weight 850, line height 1.2 (25px on mobile). Sub-section headings.
- **headline-sm:** Moniker 32px at weight 400, line height 1.4, tracking -0.013em. Card and feature titles.
- **body-md:** Moniker 21px at weight 400, line height 1, tracking -0.013em. Body text.
- **body-lg:** Moniker 24px at weight 400, line height 1.45, tracking -0.012em. Lead paragraphs.
- **body-sm:** Moniker 17.5px at weight 500, line height 1.45, tracking -0.012em. Secondary and small text.
- **label-md:** Moniker 21px at weight 500, line height 1, tracking -0.013em. Buttons, navigation and labels.
- **label-sm:** Moniker 14.5px at weight 500, line height 1, tracking -0.012em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 4% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.2px, md 10.4px, lg 18.72px, xl 33.6px.
- **Sections:** 90px vertical padding between major sections.
- **Gaps:** 19.2px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 11.52px 11.52px -11.52px, rgba(0, 0, 0, 0.2) 0px 17.28px 17.28px -17.28px, rgba(0, 0, 0, 0.3) 0px 23.04px 23.04px -23.04px`
- `rgba(0, 0, 0, 0.02) 0px 0px 0px 1px, rgba(0, 0, 0, 0.2) 0px 6.4px 51.2px -25.6px, rgba(0, 0, 0, 0.3) 0px 12.8px 76.8px -32px, rgba(0, 0, 0, 0.4) 0px 12.8px 25.6px -38.4px, rgba(0, 0, 0, 0.5) 0px 25.6px 38.4px -51.2px, rgba(0, 0, 0, 0.6) 0px 38.4px 51.2px -64px`
- `rgba(23, 33, 43, 0.1) 0px 2.72px 32.64px 0px, rgba(23, 33, 43, 0.1) 0px 5.44px 43.52px 0px, rgba(23, 33, 43, 0.1) 0px 8.16px 54.4px 0px`

## Shapes

Most elements use 43.68px corners. Measured radii, most used first:

- **md (43.68px):** 124 elements.
- **xs (20.88px):** 36 elements.
- **lg (57.2px):** 12 elements.
- **xl (74.8px):** 12 elements.
- **sm (25.6px):** 6 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“Ryan Hoover”):** #202C38 fill, #ECE9E6 text, 14.4px/500, 20.88px radius, padding 4.32px 15.84px 4.32px 4.32px, shadow `rgba(0, 0, 0, 0.1) 0px 11.52px 11.52px -11.52px, rgba(0, 0, 0, 0.2) 0px 17.28px 17.28px -17.28px, rgba(0, 0, 0, 0.3) 0px 23.04px 23.04px -23.04px`.
- **button-secondary (“Try HEY free for 30-days”):** transparent fill, #FFFFFF text, 27.2px/500, 74.8px radius, padding 23.8px 29.92px.
- **button-tertiary (“Try HEY free”):** transparent fill, #FFFFFF text, 20.8px/500, 57.2px radius, padding 16.64px 21.32px.
- **button-ghost (“Try HEY free”):** transparent fill, #FFFFFF text, 20.8px/500, 57.2px radius, padding 16.64px 21.32px.
- **input-field (“julie.young@hey.com”):** transparent fill, #ECE9E6 text, 24px/400, padding 0px 0px 0px 21.6px.
- **card:** #202C38 fill, #ECE9E6 text, 32px/400, 25.6px radius, padding 0px, shadow `rgba(0, 0, 0, 0.02) 0px 0px 0px 1px, rgba(0, 0, 0, 0.2) 0px 6.4px 51.2px -25.6px, rgba(0, 0, 0, 0.3) 0px 12.8px 76.8px -32px, rgba(0, 0, 0, 0.4) 0px 12.8px 25.6px -38.4px, rgba(0, 0, 0, 0.5) 0px 25.6px 38.4px -51.2px, rgba(0, 0, 0, 0.6) 0px 38.4px 51.2px -64px`.
- **link:** transparent fill, #ECE9E6 text, padding 0px.

## Do's and Don'ts

- Do use #202C38 for the page and lift surfaces in small steps: #17212B, #333C47.
- Do keep text in 2 levels: #ECE9E6, #FFFFFF.
- Do reserve #8C85FF for primary actions and key highlights.
- Do reuse the measured spacing steps (10.4px, 18.72px).
- Do use 43.68px corners on most elements; larger surfaces also use 20.88px, 57.2px and 74.8px.
- Don't introduce new font families beyond Really Sans Large and Moniker.
- Don't use #8C85FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s.

- **Easing:** `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/hey.com/), the free DESIGN.md generator.
