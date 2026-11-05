---
version: alpha
name: CleanShot X
description: "Light interface measured from cleanshot.com: Google Sans Flex type, vivid blue accents, flat surfaces and 20px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#161618"
  on-surface-muted: "#6A6A6B"
  overlay: "#1616180D"
  overlay-strong: "#FFFFFF3D"
  outline: "#FFFFFF3D"
  primary: "#0D44E8"
  on-primary: "#FFFFFF"
typography:
  headline-display:
    fontFamily: Google Sans Flex
    fontSize: 60px
    fontWeight: 600
    lineHeight: 1.1
  headline-lg:
    fontFamily: Google Sans Flex
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.2
  headline-md:
    fontFamily: Google Sans Flex
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
  body-md:
    fontFamily: Google Sans Flex
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.15
  body-lg:
    fontFamily: Google Sans Flex
    fontSize: 18px
    fontWeight: 450
    lineHeight: 1.67
  body-sm:
    fontFamily: Google Sans Flex
    fontSize: 14px
    fontWeight: 450
    lineHeight: 1.43
  caption:
    fontFamily: Google Sans Flex
    fontSize: 13px
    fontWeight: 450
    lineHeight: 1.23
  label-md:
    fontFamily: Google Sans Flex
    fontSize: 15px
    fontWeight: 550
    lineHeight: 1.6
  label-sm:
    fontFamily: Google Sans Flex
    fontSize: 14px
    fontWeight: 550
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Google Sans Flex
    fontSize: 42px
    fontWeight: 600
    lineHeight: 1.14
  headline-lg-mobile:
    fontFamily: Google Sans Flex
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.25
  headline-md-mobile:
    fontFamily: Google Sans Flex
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.4
rounded:
  sm: 14px
  md: 20px
  lg: 40px
spacing:
  base: 4px
  xs: 3px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 34px
  gutter: 12px
  section: 124px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px
    height: 40px
  button-primary-hover:
    backgroundColor: "#0A31A6"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 20px
    height: 48px
  button-outline-hover:
    textColor: "{colors.primary}"
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px 13px 0px 16px
  input-field:
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 16px
    padding: 0px 18px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# CleanShot X Design System

## Overview

CleanShot X describes itself as: “CleanShot X is the best screenshot and screen recording app for Mac with a built-in annotation tool, Cloud uploading, scrolling capture, and a lot more.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Blue (#0D44E8)** as the main accent.

Type is set in **Google Sans Flex**. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 20px.

Measured from [cleanshot.com](https://cleanshot.com/) on November 4, 2026 at 1440×900 and 390×844 from 301 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles, plus gradient stops #174EF2.

- **White (#FFFFFF):** Page background, seen 20 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 26 times. Token `on-surface`.
- **Charcoal (#161618):** Secondary text, seen 21 times. Token `on-surface-variant`.
- **Slate (#6A6A6B):** Muted text and metadata, seen 17 times. Token `on-surface-muted`.
- **Charcoal 5% (#1616180D):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **White 24% (#FFFFFF3D):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 24% (#FFFFFF3D):** Borders and dividers, seen 2 times. Token `outline`.
- **Vivid Blue (#0D44E8):** Primary buttons and calls to action, seen 20 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**Google Sans Flex** carries the whole interface. Fallback stack: `Google Sans Flex, SF Pro Display, SF UI Text, Helvetica Neue`.

- **headline-display:** Google Sans Flex 60px at weight 600, line height 1.1 (42px on mobile). Page title (h1).
- **headline-lg:** Google Sans Flex 40px at weight 600, line height 1.2 (32px on mobile). Section headings (h2).
- **headline-md:** Google Sans Flex 20px at weight 600, line height 1.4 (18px on mobile). Sub-section headings.
- **body-md:** Google Sans Flex 16px at weight 400, line height 1.15. Body text.
- **body-lg:** Google Sans Flex 18px at weight 450, line height 1.67. Lead paragraphs.
- **body-sm:** Google Sans Flex 14px at weight 450, line height 1.43. Secondary and small text.
- **caption:** Google Sans Flex 13px at weight 450, line height 1.23. Captions and fine print.
- **label-md:** Google Sans Flex 15px at weight 550, line height 1.6. Buttons, navigation and labels.
- **label-sm:** Google Sans Flex 14px at weight 550, line height 1.43. Small labels and badges.

## Layout

Spacing follows a 4px grid: 95% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 3px, sm 8px, md 12px, lg 32px, xl 34px.
- **Sections:** 124px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(22, 22, 24, 0.02) 0px 7px 20px -8px, rgba(22, 22, 24, 0.02) 0px 29px 33px -4px, rgba(22, 22, 24, 0.05) 0px 22px 30px -8px, rgba(22, 22, 24, 0.06) 0px 0px 0px 1px`
- `rgba(4, 24, 85, 0.28) 0px 2px 6px -1px, rgba(66, 174, 247, 0.48) 0px 6px 14px 0px inset`
- `rgba(22, 22, 24, 0.2) 0px 2px 6px -1px, rgba(22, 22, 24, 0.16) 0px 0px 0px 1px`

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **md (20px):** 120 elements.
- **sm (14px):** 64 elements.
- **lg (40px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Buy now”):** #0D44E8 fill, #FFFFFF text, 16px/400, 14px radius, padding 0px.
- **button-primary-hover:** background #0A31A6, text #FFFFFF on hover.
- **button-outline (“How it works”):** #FFFFFF fill, #161618 text, 15px/550, 14px radius, padding 0px 20px, shadow `rgba(22, 22, 24, 0.2) 0px 2px 6px -1px, rgba(22, 22, 24, 0.16) 0px 0px 0px 1px`.
- **button-outline-hover:** background #FFFFFF, text #0D44E8 on hover.
- **button-ghost (“Product”):** transparent fill, #161618 text, 15px/550, 14px radius, padding 0px 13px 0px 16px.
- **input-field (“Your email”):** transparent fill, #FFFFFF text, 15px/450, 16px radius, padding 0px 18px, border 1px solid #FFFFFF3D.
- **card:** #FFFFFF fill, #000000 text, 16px/400, 20px radius, padding 0px, shadow `rgba(22, 22, 24, 0.02) 0px 7px 20px -8px, rgba(22, 22, 24, 0.02) 0px 29px 33px -4px, rgba(22, 22, 24, 0.05) 0px 22px 30px -8px, rgba(22, 22, 24, 0.06) 0px 0px 0px 1px`.
- **link:** transparent fill, #FFFFFFB8 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #000000, #161618, #6A6A6B.
- Do reserve #0D44E8 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 20px corners on most elements; larger surfaces also use 14px and 40px.
- Don't introduce new font families beyond Google Sans Flex.
- Don't use #0D44E8 for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.1s, 0.15s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cleanshot.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
