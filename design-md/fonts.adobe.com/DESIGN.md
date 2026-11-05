---
version: alpha
name: Adobe Fonts
description: "Light monochrome interface measured from fonts.adobe.com: adobe-clean type, flat surfaces and 16px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#4B4B4B"
  on-background: "#4B4B4B"
  on-surface-strong: "#2C2C2C"
  on-surface-variant: "#B1B1B1"
  outline: "#DADADA"
  primary: "#4B4B4B"
  on-primary: "#FFFFFF"
  inverse-surface: "#222222"
  secondary: "#0000EE"
typography:
  headline-display:
    fontFamily: adobe-clean
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.3
  body-md:
    fontFamily: adobe-clean
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: adobe-clean
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: adobe-clean
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: adobe-clean
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.06em
  label-md:
    fontFamily: adobe-clean
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.5
  label-sm:
    fontFamily: adobe-clean
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.5
rounded:
  md: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  margin: 30px
components:
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 14px
    height: 32px
  button-outline-hover:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
  button-ghost:
    textColor: "#292929"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 5px 16px 6px 16px
    height: 32px
  button-ghost-hover:
    backgroundColor: "#E9E9E9"
  link:
    textColor: "#D5D5D5"
---

# Adobe Fonts Design System

## Overview

Adobe Fonts describes itself as: “Adobe Fonts partners with the world’s leading type foundries to bring thousands of beautiful fonts to designers every day. No need to worry about licensing, and you can use fonts from Adobe Fonts on the web or in desktop” The interface is light, built on **White (#FFFFFF)** with **Graphite (#4B4B4B)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **adobe-clean**. Headlines run large; body text is 14px. The surface language is flat. Corners are mostly 16px.

Measured from [fonts.adobe.com](https://fonts.adobe.com/) on November 4, 2026 at 1440×900 and 390×844 from 129 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background, seen 7 times. Token `background`, CSS `--vs-background-color`.
- **Graphite (#4B4B4B):** Primary text and headings, seen 14 times. Token `on-surface`.
- **Graphite (#2C2C2C):** Headings and emphasis, seen 10 times. Token `on-surface-strong`.
- **Gray (#B1B1B1):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Silver (#DADADA):** Borders and dividers, seen 1 time. Token `outline`.
- **Graphite (#4B4B4B):** Primary actions (the main text color; the palette is monochrome), seen 18 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#222222):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Vivid Indigo (#0000EE):** Accent, seen 1 time. Token `secondary`.

## Typography

**adobe-clean** carries the whole interface. Fallback stack: `adobe-clean, adobe-clean-han-japanese, source-sans-pro, Helvetica Neue`. Other loaded fonts: adobe-notdef, mjwq-normal-400.

- **headline-display:** adobe-clean 28px at weight 700, line height 1.3. Page title (h1).
- **body-md:** adobe-clean 14px at weight 400, line height 1.5. Body text.
- **body-lg:** adobe-clean 18px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** adobe-clean 12px at weight 400, line height 1.5. Secondary and small text.
- **caption:** adobe-clean 11px at weight 400, line height 1.5, tracking 0.06em. Captions and fine print.
- **label-md:** adobe-clean 15px at weight 700, line height 1.5. Buttons, navigation and labels.
- **label-sm:** adobe-clean 14px at weight 700, line height 1.5. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (78% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 40px.
- **Page margin:** 30px on each side of full-width sections.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #DADADA borders.

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **md (16px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“View more”):** transparent fill, #4B4B4B text, 15px/700, 16px radius, padding 0px 14px, border 2px solid #4B4B4B.
- **button-outline-hover:** background #4B4B4B, text #FFFFFF on hover.
- **button-ghost (“Sign in”):** transparent fill, #292929 text, 14px/700, 16px radius, padding 5px 16px 6px 16px, border 2px solid #DADADA.
- **button-ghost-hover:** background #E9E9E9, text #292929 on hover.
- **link:** transparent fill, #D5D5D5 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #4B4B4B, #2C2C2C, #B1B1B1.
- Do let contrast carry emphasis; primary actions use #4B4B4B on #FFFFFF.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 16px corners on most elements.
- Don't use #B1B1B1 for body text; it reaches 2.14:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond adobe-clean.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.125s, 0.2s.

- **Easing:** `ease-out`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/fonts.adobe.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
