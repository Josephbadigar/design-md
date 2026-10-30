---
version: alpha
name: Notion
description: "Light interface measured from notion.com: NotionInter type, vivid blue accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#0D0D0D"
  on-background: "#0D0D0D"
  on-surface-strong: "#000000"
  on-surface-variant: "#1A1A1A"
  on-surface-muted: "#615D59"
  surface-container-low: "#F9F9F8"
  surface-container: "#E6F3FE"
  overlay: "#0000000D"
  outline: "#0000001A"
  primary: "#0075DE"
  on-primary: "#FFFFFF"
  inverse-surface: "#78736F"
  secondary: "#1AAE39"
  tertiary: "#FFB110"
typography:
  headline-display:
    fontFamily: NotionInter
    fontSize: 96px
    fontWeight: 600
    lineHeight: 1.04
    letterSpacing: -0.048em
  headline-lg:
    fontFamily: NotionInter
    fontSize: 54px
    fontWeight: 700
    lineHeight: 1.04
    letterSpacing: -0.035em
  headline-md:
    fontFamily: NotionInter
    fontSize: 22px
    fontWeight: 700
    lineHeight: 1.27
    letterSpacing: -0.011em
  body-md:
    fontFamily: NotionInter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-lg:
    fontFamily: NotionInter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: NotionInter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  label-sm:
    fontFamily: NotionInter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: 0.01em
  headline-display-mobile:
    fontFamily: NotionInter
    fontSize: 42px
    fontWeight: 600
    lineHeight: 1.14
    letterSpacing: -0.036em
rounded:
  sm: 4px
  md: 8px
  lg: 12px
  full: 9999px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 8px
  container: 500px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 4px 14px
    height: 36px
  button-primary-hover:
    backgroundColor: "#005BAB"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "#005BAB"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 6px 15px
    height: 38px
  button-outline-hover:
    backgroundColor: "#F2F9FF"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 5px 10px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Notion Design System

## Overview

Notion describes itself as: “Build Custom Agents, search across all your apps, and automate busywork. The AI workspace where teams get more done, faster.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#0D0D0D)** text, and **Vivid Blue (#0075DE)** as the main accent.

Type is set in **NotionInter**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 8px.

Measured from [notion.com](https://www.notion.com/) on October 29, 2026 at 1440×900 and 390×844 from 266 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **White (#FFFFFF):** Page background, seen 14 times. Token `background`.
- **Charcoal (#0D0D0D):** Primary text and headings. Token `on-surface`.
- **Near Black (#000000):** Headings and emphasis, seen 13 times. Token `on-surface-strong`.
- **Charcoal (#1A1A1A):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Warm Slate (#615D59):** Muted text and metadata, seen 6 times. Token `on-surface-muted`, CSS `--tatami-color-icon-button-active`.
- **Snow (#F9F9F8):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--tatami-color-menu-button-background`.
- **Pale Blue (#E6F3FE):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--tatami-color-blue-200`.
- **Near Black 5% (#0000000D):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Near Black 10% (#0000001A):** Borders and dividers, seen 14 times. Token `outline`, CSS `--tatami-color-background-base-active`.
- **Vivid Blue (#0075DE):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Warm Slate (#78736F):** High-contrast fills, seen 8 times. Token `inverse-surface`, CSS `--tatami-color-gray-500`.
- **Green (#1AAE39):** Accent in text, fills and borders, seen 2 times. Token `secondary`.
- **Vivid Amber (#FFB110):** Accent in text, fills and borders, seen 2 times. Token `tertiary`.

## Typography

**NotionInter** carries the whole interface. Fallback stack: `NotionInter, Inter, -apple-system, BlinkMacSystemFont`. Other loaded fonts: Lyon Text.

- **headline-display:** NotionInter 96px at weight 600, line height 1.04, tracking -0.048em (42px on mobile). Page title (h1).
- **headline-lg:** NotionInter 54px at weight 700, line height 1.04, tracking -0.035em. Section headings (h2).
- **headline-md:** NotionInter 22px at weight 700, line height 1.27, tracking -0.011em. Sub-section headings.
- **body-md:** NotionInter 14px at weight 400, line height 1.43. Body text.
- **label-lg:** NotionInter 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** NotionInter 14px at weight 500, line height 1.43. Buttons, navigation and labels.
- **label-sm:** NotionInter 12px at weight 500, line height 1.33, tracking 0.01em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 66% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3px, sm 8px, md 16px, lg 24px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 500px.
- **Breakpoints:** 375px, 400px, 440px, 500px, 599px, 600px, 768px, 799px, 839px, 840px, 919px, 960px, 980px, 1080px, 1280px, 1440px, 1600px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F9F9F8 → #E6F3FE) and #0000001A borders.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 180 elements.
- **lg (12px):** 56 elements.
- **sm (4px):** 44 elements.
- **full (9999px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Notion free”):** #0075DE fill, #FFFFFF text, 16px/500, 8px radius, padding 4px 14px.
- **button-primary-hover:** background #005BAB, text #FFFFFF on hover.
- **button-outline (“Request a demo”):** #E6F3FE fill, #005BAB text, 16px/500, 8px radius, padding 6px 15px.
- **button-outline-hover:** background #F2F9FF, text #005BAB on hover.
- **button-ghost (“Product”):** transparent fill, #000000E5 text, 16px/400, 4px radius, padding 5px 10px.
- **card:** #FFFFFF fill, #000000E5 text, 16px/400, 12px radius, padding 0px.
- **link:** transparent fill, #000000E5 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F9F9F8, #E6F3FE.
- Do keep text in 4 levels: #0D0D0D, #000000, #1A1A1A, #615D59.
- Do reserve #0075DE for primary actions and key highlights.
- Do set headlines in NotionInter with tight tracking (-0.048em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 12px and 4px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond NotionInter.
- Don't use #0075DE for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.42, 0, 1, 1)`, `ease`, `cubic-bezier(0.645, 0.045, 0.355, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/notion.com/), the free DESIGN.md generator (engine 2026.10.29+bf9d681d83cf).
