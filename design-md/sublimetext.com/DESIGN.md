---
version: alpha
name: Sublime Text
description: "Light interface measured from sublimetext.com: Lato type, blue accents, tonal surfaces and 3px corners."
colors:
  background: "#EEEEEE"
  surface: "#EEEEEE"
  on-surface: "#555555"
  on-background: "#555555"
  on-surface-variant: "#666666"
  on-surface-muted: "#777777"
  surface-container-low: "#FFFFFF"
  surface-container: "#CCCCCC"
  overlay: "#EEEEEECC"
  overlay-strong: "#CCCCCCCC"
  outline: "#CCCCCC"
  primary: "#3C78B4"
  on-primary: "#FFFFFF"
  inverse-surface: "#888888"
  secondary: "#157BBC"
  link: "#4075BF"
typography:
  headline-display:
    fontFamily: Lato
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.6
  headline-lg:
    fontFamily: Lato
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.6
  headline-md:
    fontFamily: Lato
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0.021em
  body-md:
    fontFamily: Lato
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: Lato
    fontSize: 14.5px
    fontWeight: 400
    lineHeight: 1.6
  caption:
    fontFamily: Lato
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.6
  headline-display-mobile:
    fontFamily: Lato
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.53
rounded:
  md: 3px
spacing:
  xs: 2px
  sm: 8px
  md: 9.6px
  lg: 20px
  xl: 40px
  container: 1200px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 8px 15px
    height: 42px
  button-primary-hover:
    backgroundColor: "#336699"
  button-ghost:
    textColor: "#999999"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 2px 4px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: 4px
    padding: 16px
  link:
    textColor: "{colors.link}"
---

# Sublime Text Design System

## Overview

Sublime Text describes itself as: “Sublime Text is a sophisticated text editor for code, markup and prose. You'll love the slick user interface, extraordinary features and amazing performance.” The interface is light, built on **Mist (#EEEEEE)** with **Slate (#555555)** text, and **Blue (#3C78B4)** as the main accent.

Type is set in **Lato**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 3px.

Measured from [sublimetext.com](https://www.sublimetext.com/) on November 4, 2026 at 1440×900 and 390×844 from 87 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Mist (#EEEEEE):** Page background, seen 1 time. Token `background`.
- **Slate (#555555):** Primary text and headings, seen 13 times. Token `on-surface`.
- **Slate (#666666):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Slate (#777777):** Muted text and metadata, seen 10 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Silver (#CCCCCC):** Cards and panels, seen 3 times. Token `surface-container`.
- **Mist 80% (#EEEEEECC):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Silver 80% (#CCCCCCCC):** Stronger translucent fill, seen 2 times. Token `overlay-strong`.
- **Silver (#CCCCCC):** Borders and dividers, seen 5 times. Token `outline`.
- **Blue (#3C78B4):** Primary buttons and calls to action, seen 4 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Gray (#888888):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Blue (#157BBC):** Accent, seen 1 time. Token `secondary`.
- **Blue (#4075BF):** Inline links, seen 2 times. Token `link`.

## Typography

**Lato** carries the whole interface. Fallback stack: `Lato, Arial, sans-serif`.

- **headline-display:** Lato 48px at weight 400, line height 1.6 (30px on mobile). Page title (h1).
- **headline-lg:** Lato 32px at weight 700, line height 1.6. Section headings (h2).
- **headline-md:** Lato 24px at weight 400, line height 1.6, tracking 0.021em, uppercase. Sub-section headings.
- **body-md:** Lato 16px at weight 400, line height 1.6. Body text.
- **body-sm:** Lato 14.5px at weight 400, line height 1.6. Secondary and small text.
- **caption:** Lato 13px at weight 400, line height 1.6. Captions and fine print.

## Layout

Spacing does not follow a strict grid: 50% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 9.6px, lg 20px, xl 40px.
- **Container:** content is capped at 1200px.
- **Breakpoints:** 550px, 640px, 700px, 820px, 1000px, 1024px, 1100px, 1140px, 1160px, 1200px, 1240px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.08) 0px 0px 20px 0px`
- `rgba(58, 58, 58, 0.3) 1px 1px 5px 0px`

## Shapes

Most elements use 3px corners. Measured radii, most used first:

- **md (3px):** 72 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“INSTALL FOR LINUX”):** #3C78B4 fill, #FFFFFF text, 16px/400, 3px radius, padding 8px 15px.
- **button-primary-hover:** background #336699, text #FFFFFF on hover.
- **button-ghost (“Pause”):** transparent fill, #999999 text, 14.4px/400, padding 2px 4px.
- **card:** #FFFFFF fill, #555555 text, 16px/400, 4px radius, padding 16px, shadow `rgba(58, 58, 58, 0.3) 1px 1px 5px 0px`.
- **link:** transparent fill, #4075BF text, padding 0px.

## Do's and Don'ts

- Do use #EEEEEE for the page and lift surfaces in small steps: #FFFFFF, #CCCCCC.
- Do keep text in 3 levels: #555555, #666666, #777777.
- Do reserve #3C78B4 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 9.6px, 20px).
- Do use 3px corners on most elements.
- Don't use #777777 for body text; it reaches 3.86:1 on #EEEEEE. Keep it for large text or metadata.
- Don't introduce new font families beyond Lato.
- Don't use #3C78B4 for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s.

- **Easing:** `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/sublimetext.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
