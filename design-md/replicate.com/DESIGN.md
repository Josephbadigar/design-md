---
version: alpha
name: Replicate
description: "Dark monochrome interface measured from replicate.com: rb-freigeist-neue type with basier-square, tonal surfaces and pill-shaped controls."
colors:
  background: "#111111"
  surface: "#111111"
  on-surface: "#EEEEEE"
  on-background: "#EEEEEE"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#B4B4B4"
  on-surface-muted: "#606060"
  surface-container-low: "#181111"
  surface-container: "#1B180F"
  surface-container-high: "#000000"
  overlay: "#0000001A"
  outline: "#FFFFFF33"
  outline-variant: "#000000"
  primary: "#FFFFFF"
  on-primary: "#000000"
  secondary: "#FF7B72"
  tertiary: "#EC6142"
  error: "#EA2804"
  warning: "#F5E147"
typography:
  headline-display:
    fontFamily: rb-freigeist-neue
    fontSize: 128px
    fontWeight: 700
    lineHeight: 1
  headline-lg:
    fontFamily: rb-freigeist-neue
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
  headline-md:
    fontFamily: rb-freigeist-neue
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.2
  headline-sm:
    fontFamily: basier-square
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.33
  title-lg:
    fontFamily: basier-square
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
  body-md:
    fontFamily: basier-square
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: basier-square
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: basier-square
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: rb-freigeist-neue
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: basier-square
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  code:
    fontFamily: jetbrains-mono
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.5
  headline-sm-mobile:
    fontFamily: basier-square
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
  headline-md-mobile:
    fontFamily: rb-freigeist-neue
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
rounded:
  md: 2px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 64px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: 0px
    padding: 12px 16px
    height: 54px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 8px 12px
    height: 42px
  button-outline-hover:
    backgroundColor: "#FFFFFF1B"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 10px 8px
  input-field:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 6px 56px 6px 28px
  card:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Replicate Design System

## Overview

Replicate describes itself as: “Run open-source machine learning models with a cloud API” The interface is dark, built on **Charcoal (#111111)** with **Mist (#EEEEEE)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **rb-freigeist-neue** and **basier-square**, with **jetbrains-mono** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [replicate.com](https://replicate.com/) on October 21, 2026 at 1440×900 and 390×844 from 379 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles, plus gradient stops #FF6BFC, #EA2804, #F6F47F.

- **Charcoal (#111111):** Page background, seen 4 times. Token `background`.
- **Mist (#EEEEEE):** Primary text and headings, seen 29 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 5 times. Token `on-surface-strong`, CSS `--tw-ring-offset-color`.
- **Gray (#B4B4B4):** Secondary text, seen 25 times. Token `on-surface-variant`.
- **Slate (#606060):** Muted text and metadata, seen 8 times. Token `on-surface-muted`.
- **Warm Charcoal (#181111):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Warm Charcoal (#1B180F):** Cards and panels, seen 2 times. Token `surface-container`.
- **Near Black (#000000):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Near Black 10% (#0000001A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 20% (#FFFFFF33):** Borders and dividers, seen 6 times. Token `outline`.
- **Near Black (#000000):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 27 times. Token `primary`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Light Red (#FF7B72):** Most used accent color, seen 14 times. Token `secondary`.
- **Vivid Red (#EC6142):** Most used accent color, seen 12 times. Token `tertiary`.
- **Vivid Red (#EA2804):** Errors and destructive states, seen 15 times. Token `error`.
- **Vivid Yellow (#F5E147):** Warnings and highlights, seen 2 times. Token `warning`, CSS `--yellow-11`.

## Typography

**rb-freigeist-neue**, **basier-square** and **jetbrains-mono** (monospace) share the interface. Fallback stack: `rb-freigeist-neue, ui-sans-serif, system-ui, sans-serif`.

- **headline-display:** rb-freigeist-neue 128px at weight 700, line height 1. Page title (h1).
- **headline-lg:** rb-freigeist-neue 48px at weight 400, line height 1. Section headings (h2).
- **headline-md:** rb-freigeist-neue 30px at weight 600, line height 1.2 (24px on mobile). Sub-section headings.
- **headline-sm:** basier-square 24px at weight 400, line height 1.33 (20px on mobile). Card and feature titles.
- **title-lg:** basier-square 20px at weight 400, line height 1.4. Small titles.
- **body-md:** basier-square 16px at weight 400, line height 1.5. Body text.
- **body-lg:** basier-square 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** basier-square 12px at weight 400, line height 1.33, lowercase. Secondary and small text.
- **label-md:** rb-freigeist-neue 16px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** basier-square 14px at weight 400, line height 1.43. Small labels and badges.
- **code:** jetbrains-mono 11px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 16px, lg 24px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(102, 84, 23) 0px 1px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 108 elements.
- **md (2px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started for free”):** #FFFFFF fill, #000000 text, 18px/400, padding 12px 16px, border 1px solid #FFFFFF.
- **button-primary-hover:** background #FFFFFFED, text #000000 on hover.
- **button-outline (“Push a model”):** #000000 fill, #EEEEEE text, 16px/400, padding 8px 12px, border 1px solid #EEEEEE.
- **button-outline-hover:** background #FFFFFF1B, text #EEEEEE on hover.
- **button-ghost (“Node”):** transparent fill, #EEEEEE text, 14px/400, padding 10px 8px.
- **input-field (“Search 'best image models' or 't”):** #0000001A fill, #EEEEEE text, 14px/400, padding 6px 56px 6px 28px.
- **card:** transparent fill, #EEEEEE text, 16px/400, padding 0px.
- **link:** transparent fill, #EEEEEE text, padding 0px.

## Do's and Don'ts

- Do use #111111 for the page and lift surfaces in small steps: #181111, #1B180F, #000000.
- Do keep text in 4 levels: #EEEEEE, #FFFFFF, #B4B4B4, #606060.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #111111.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 2px corners.
- Don't use #606060 for body text; it reaches 3.0:1 on #111111. Keep it for large text or metadata.
- Don't introduce new font families beyond rb-freigeist-neue, basier-square and jetbrains-mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.5s, 0.2s. Longer ambient animations run 10s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `linear`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/replicate.com/), the free DESIGN.md generator.
