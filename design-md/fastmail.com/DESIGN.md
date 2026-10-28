---
version: alpha
name: Fastmail
description: "Light interface measured from fastmail.com: roca type with Proxima Nova, dark blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1B1E20"
  on-background: "#1B1E20"
  on-surface-variant: "#5B646C"
  on-surface-muted: "#ADB1B5"
  surface-container-low: "#FBF7EF"
  surface-container: "#F4F5F5"
  surface-container-high: "#C1C5C8"
  overlay: "#FFFFFF80"
  overlay-strong: "#F2F7FB1A"
  outline: "#D6D8DA"
  outline-variant: "#FFFFFF1A"
  primary: "#253859"
  on-primary: "#FFFFFF"
  secondary: "#25446A"
  tertiary: "#0067B9"
  warning: "#FFC107"
typography:
  headline-display:
    fontFamily: roca
    fontSize: 58px
    fontWeight: 400
    lineHeight: 1.11
  headline-lg:
    fontFamily: roca
    fontSize: 46px
    fontWeight: 400
    lineHeight: 1.1
  headline-md:
    fontFamily: Proxima Nova
    fontSize: 25.5px
    fontWeight: 600
    lineHeight: 1.4
  body-md:
    fontFamily: Proxima Nova
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Proxima Nova
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Proxima Nova
    fontSize: 12.5px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Proxima Nova
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.4
  headline-display-mobile:
    fontFamily: roca
    fontSize: 46.5px
    fontWeight: 400
    lineHeight: 1.12
  headline-lg-mobile:
    fontFamily: roca
    fontSize: 41.5px
    fontWeight: 400
    lineHeight: 1.1
  headline-md-mobile:
    fontFamily: Proxima Nova
    fontSize: 23px
    fontWeight: 600
    lineHeight: 1.4
rounded:
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 40px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 22.41px
  xl: 35.86px
  gutter: 16px
  section: 125.52px
  margin: 35.45px
  container: 1332px
components:
  button-primary:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.tertiary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 4px 12px 4px 4px
    height: 40px
  button-primary-hover:
    backgroundColor: "#CCE0F1"
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 125.52px 0px 161.38px 0px
  link:
    textColor: "#F4F5F7"
---

# Fastmail Design System

## Overview

Fastmail describes itself as: “Fast, private email hosting for you or your business. More productive, lightning fast, simple and built to save you time.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1B1E20)** text, and **Dark Blue (#253859)** as the main accent.

Type is set in **roca** and **Proxima Nova**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [fastmail.com](https://www.fastmail.com/) on October 21, 2026 at 1440×900 and 390×844 from 355 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #0067B9, #296B9F, #243959.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`, CSS `--brand-color-grey-0`.
- **Charcoal (#1B1E20):** Primary text and headings, seen 71 times. Token `on-surface`.
- **Cool Slate (#5B646C):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Cool Gray (#ADB1B5):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Warm Snow (#FBF7EF):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Snow (#F4F5F5):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--brand-color-grey-5`.
- **Cool Silver (#C1C5C8):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **White 50% (#FFFFFF80):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Snow 10% (#F2F7FB1A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Silver (#D6D8DA):** Borders and dividers, seen 4 times. Token `outline`, CSS `--brand-color-grey-20`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Dark Blue (#253859):** Brand color in logos and imagery, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#25446A):** Brand color in logos and imagery, seen 35 times. Token `secondary`.
- **Dark Blue (#0067B9):** Brand color in the logo, seen 33 times. Token `tertiary`, CSS `--theme-push-select-fg`.
- **Vivid Amber (#FFC107):** Warnings and highlights, seen 2 times. Token `warning`.

## Typography

**roca** and **Proxima Nova** share the interface. Fallback stack: `roca, Georgia Roca Fallback, Iowan Old Style, Palatino Linotype`. Other loaded fonts: Georgia Roca Fallback.

- **headline-display:** roca 58px at weight 400, line height 1.11 (46.5px on mobile). Page title (h1).
- **headline-lg:** roca 46px at weight 400, line height 1.1 (41.5px on mobile). Section headings (h2).
- **headline-md:** Proxima Nova 25.5px at weight 600, line height 1.4 (23px on mobile). Sub-section headings.
- **body-md:** Proxima Nova 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Proxima Nova 16px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** Proxima Nova 12.5px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** Proxima Nova 16px at weight 600, line height 1.4. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 44% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 16px, lg 22.41px, xl 35.86px.
- **Sections:** 125.52px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1332px.
- **Page margin:** 35.45px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 10px 15px -3px, rgba(0, 0, 0, 0.1) 0px 4px 6px -4px`
- `rgba(0, 0, 0, 0.09) 0px 0px 12px 0px, rgba(0, 0, 0, 0.07) 0px 0px 16px 0px, rgba(0, 0, 0, 0.15) 0px 0px 6px 0px`
- `rgba(27, 30, 32, 0.08) 0px 15px 17px -3px, rgba(27, 30, 32, 0.1) 0px 6px 10px -2px, rgba(27, 30, 32, 0.12) 0px 3px 6px -1px, rgba(27, 30, 32, 0.14) 0px 0px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 24 elements.
- **md (16px):** 20 elements.
- **xs (8px):** 12 elements.
- **sm (12px):** 12 elements.
- **xl (40px):** 12 elements.
- **lg (24px):** 10 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Why Fastmail?”):** #C1C5C8 fill, #0067B9 text, 15.9389px/600, 9999px radius, padding 4px 12px 4px 4px, shadow `rgba(0, 0, 0, 0.09) 0px 0px 12px 0px, rgba(0, 0, 0, 0.07) 0px 0px 16px 0px, rgba(0, 0, 0, 0.15) 0px 0px 6px 0px`.
- **button-primary-hover:** background #CCE0F1, text #0067B9 on hover.
- **card:** #FFFFFF fill, #1B1E20 text, 16px/400, 24px 24px 0px 0px radius, padding 125.52px 0px 161.38px 0px.
- **link:** transparent fill, #F4F5F7 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FBF7EF, #F4F5F5, #C1C5C8.
- Do keep text in 3 levels: #1B1E20, #5B646C, #ADB1B5.
- Do use #253859 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 22.41px).
- Do make buttons and chips fully rounded (9999px); most other elements use 16px corners.
- Don't use #ADB1B5 for body text; it reaches 2.2:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond roca and Proxima Nova.
- Don't use #253859 for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.5s, 0.3s.

- **Easing:** `cubic-bezier(0.16, 1, 0.3, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/fastmail.com/), the free DESIGN.md generator.
