---
version: alpha
name: Loom
description: "Light interface measured from loom.com: Charlie Display type with Charlie Text, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#101214"
  on-background: "#101214"
  on-surface-strong: "#000000"
  on-surface-variant: "#292A2E"
  surface-container-low: "#F8EEFE"
  surface-container: "#E9F2FE"
  overlay: "#FF613D20"
  outline: "#00000033"
  primary: "#1868DB"
  on-primary: "#FFFFFF"
  secondary: "#82B536"
  tertiary: "#EB9100"
  warning: "#A36700"
  error: "#FF613D"
typography:
  headline-display:
    fontFamily: Charlie Display
    fontSize: 63px
    fontWeight: 700
    lineHeight: 1.03
  headline-lg:
    fontFamily: Charlie Display
    fontSize: 44px
    fontWeight: 700
    lineHeight: 1.14
  headline-md:
    fontFamily: Charlie Display
    fontSize: 32.5px
    fontWeight: 700
    lineHeight: 1.27
  headline-sm:
    fontFamily: Charlie Text
    fontSize: 26.5px
    fontWeight: 400
    lineHeight: 1.52
  title-lg:
    fontFamily: Charlie Display
    fontSize: 25px
    fontWeight: 700
    lineHeight: 1.33
  body-md:
    fontFamily: Charlie Text
    fontSize: 15.5px
    fontWeight: 400
    lineHeight: 1.71
  body-lg:
    fontFamily: Charlie Text
    fontSize: 18.5px
    fontWeight: 400
    lineHeight: 1.65
  body-sm:
    fontFamily: Charlie Text
    fontSize: 12.5px
    fontWeight: 400
    lineHeight: 1.45
  label-md:
    fontFamily: Charlie Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Charlie Text
    fontSize: 12.5px
    fontWeight: 700
    lineHeight: 1.45
  headline-display-mobile:
    fontFamily: Charlie Display
    fontSize: 35px
    fontWeight: 700
    lineHeight: 1.03
  title-lg-mobile:
    fontFamily: Charlie Display
    fontSize: 22px
    fontWeight: 700
    lineHeight: 1.27
rounded:
  sm: 6px
  md: 41.69px
  lg: 68.92px
  full: 9999px
spacing:
  sm: 6px
  md: 16px
  lg: 23.42px
  xl: 36.16px
  gutter: 15.62px
  section: 111.04px
  margin: 36.16px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 7.81px 15.62px
    height: 48px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 7.81px 15.62px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 16px
  link:
    textColor: "{colors.on-surface}"
---

# Loom Design System

## Overview

Loom describes itself as: “Best free online screen recording tool with advanced video editing and video storage trusted by over 22 million people and easy sharing from Loom.com.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#101214)** text, and **Vivid Blue (#1868DB)** as the main accent.

Type is set in **Charlie Display** and **Charlie Text**. Headlines run large; body text is 15.5px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [loom.com](https://www.loom.com/) on October 21, 2026 at 1440×900 and 390×844 from 459 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`.
- **Charcoal (#101214):** Primary text and headings, seen 87 times. Token `on-surface`, CSS `--thd-color-black`.
- **Near Black (#000000):** Headings and emphasis, seen 3 times. Token `on-surface-strong`.
- **Graphite (#292A2E):** Secondary text, seen 20 times. Token `on-surface-variant`, CSS `--lns-themeLight-color-body`.
- **Cool Snow (#F8EEFE):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`, CSS `--lns-themeLight-color-upgrade`.
- **Pale Blue (#E9F2FE):** Cards and panels, seen 5 times. Token `surface-container`, CSS `--lns-color-blurpleLight`.
- **Vivid Red 13% (#FF613D20):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Near Black 20% (#00000033):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Blue (#1868DB):** Brand color in the header, seen 23 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Lime (#82B536):** Most used accent color, seen 8 times. Token `secondary`.
- **Vivid Orange (#EB9100):** Accent, seen 7 times. Token `tertiary`.
- **Dark Orange (#A36700):** Warnings and highlights, seen 7 times. Token `warning`.
- **Vivid Red (#FF613D):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Charlie Display** and **Charlie Text** share the interface. Fallback stack: `Charlie Display, sans-serif`.

- **headline-display:** Charlie Display 63px at weight 700, line height 1.03 (35px on mobile). Page title (h1).
- **headline-lg:** Charlie Display 44px at weight 700, line height 1.14. Section headings (h2).
- **headline-md:** Charlie Display 32.5px at weight 700, line height 1.27. Sub-section headings.
- **headline-sm:** Charlie Text 26.5px at weight 400, line height 1.52. Card and feature titles.
- **title-lg:** Charlie Display 25px at weight 700, line height 1.33 (22px on mobile). Small titles.
- **body-md:** Charlie Text 15.5px at weight 400, line height 1.71. Body text.
- **body-lg:** Charlie Text 18.5px at weight 400, line height 1.65. Lead paragraphs.
- **body-sm:** Charlie Text 12.5px at weight 400, line height 1.45. Secondary and small text.
- **label-md:** Charlie Text 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Charlie Text 12.5px at weight 700, line height 1.45. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 38% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** sm 6px, md 16px, lg 23.42px, xl 36.16px.
- **Sections:** 111.04px vertical padding between major sections.
- **Gaps:** 15.62px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 36.16px on each side of full-width sections.
- **Breakpoints:** 360px, 375px, 640px, 767px, 768px, 820px, 1023px, 1024px, 1025px, 1280px, 1358px, 1600px, 1650px, 1920px, 2384px, 2884px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.03) 0px 4px 6.4px 0px, rgba(0, 0, 0, 0.05) 0px 3px 9.6px 0px, rgba(0, 0, 0, 0.07) 0px 8px 32px 0px, rgba(0, 0, 0, 0.1) 0px 32px 96px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 136 elements.
- **lg (68.92px):** 28 elements.
- **md (41.69px):** 16 elements.
- **sm (6px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Loom for free”):** #1868DB fill, #FFFFFF text, 15.6154px/400, 9999px radius, padding 7.81px 15.62px.
- **button-outline (“Contact Sales”):** #E9F2FE fill, #000000 text, 15.6154px/400, 9999px radius, padding 7.81px 15.62px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 4.45038px`.
- **button-ghost (“Apps”):** transparent fill, #292A2E text, 16px/400, 9999px radius, padding 8px 16px.
- **link:** transparent fill, #101214 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8EEFE, #E9F2FE.
- Do keep text in 3 levels: #101214, #000000, #292A2E.
- Do use #1868DB as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (6px, 16px, 23.42px).
- Do make buttons and chips fully rounded (9999px); most other elements use 68.92px corners.
- Don't introduce new font families beyond Charlie Display and Charlie Text.
- Don't use #1868DB for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.1s, 0.15s, 0.6s, 0.5s. Longer ambient animations run 1s.

- **Easing:** `ease-in-out`, `cubic-bezier(0.4, 0, 1, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/loom.com/), the free DESIGN.md generator.
