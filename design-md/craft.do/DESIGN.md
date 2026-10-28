---
version: alpha
name: Craft
description: "Light interface measured from craft.do: UntitledSerifFont type with UntitledSansFont, light blue accents, tonal surfaces and 24px corners."
colors:
  background: "#FCF9F7"
  surface: "#FCF9F7"
  on-surface: "#030302"
  on-background: "#030302"
  on-surface-variant: "#1B1B1A"
  on-surface-muted: "#41413F"
  on-surface-subtle: "#777879"
  surface-container-low: "#FFFFFFE6"
  surface-container: "#FFFFFF"
  surface-container-high: "#EFEFEF"
  surface-container-highest: "#DBEDFE"
  overlay: "#0000000D"
  overlay-strong: "#0000000A"
  outline: "#FFFFFF4D"
  outline-variant: "#03030217"
  primary: "#B8CAF5"
  on-primary: "#000000"
  secondary: "#AADAF1"
  tertiary: "#0087FF"
typography:
  headline-display:
    fontFamily: UntitledSerifFont
    fontSize: 66px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: UntitledSerifFont
    fontSize: 54px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: UntitledSerifFont
    fontSize: 46px
    fontWeight: 400
    lineHeight: 1.22
    letterSpacing: -0.03em
  headline-sm:
    fontFamily: UntitledSerifFont
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.22
    letterSpacing: -0.03em
  title-lg:
    fontFamily: UntitledSerifFont
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.03em
  body-md:
    fontFamily: UntitledSansFont
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: apple-system
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: apple-system
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.02em
  label-md:
    fontFamily: UntitledSansFont
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: UntitledSansFont
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0.01em
  headline-display-mobile:
    fontFamily: UntitledSerifFont
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.04em
  headline-lg-mobile:
    fontFamily: UntitledSerifFont
    fontSize: 38px
    fontWeight: 400
    lineHeight: 0.99
    letterSpacing: -0.02em
rounded:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 14px
  xl: 24px
spacing:
  xs: 2px
  sm: 5px
  md: 16px
  lg: 24px
  xl: 60px
  gutter: 24px
  section: 60px
  margin: 24px
  container: 920px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.surface-container}"
    typography: "{typography.label-md}"
    padding: 8px 14px
    height: 36px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-muted}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "#FF4500"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 24px
  link:
    textColor: "{colors.surface-container}"
---

# Craft Design System

## Overview

Craft describes itself as: “A free notes and productivity app that follows you across all your devices. Premium features available.” The interface is light, built on **Snow (#FCF9F7)** with **Near Black (#030302)** text, and **Light Blue (#B8CAF5)** as the main accent.

Type is set in **UntitledSerifFont** and **UntitledSansFont**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 24px.

Measured from [craft.do](https://www.craft.do/) on October 21, 2026 at 1440×900 and 390×844 from 428 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles.

- **Snow (#FCF9F7):** Page background, seen 1 time. Token `background`.
- **Near Black (#030302):** Primary text and headings, seen 84 times. Token `on-surface`, CSS `--color-black-900`.
- **Charcoal (#1B1B1A):** Secondary text, seen 13 times. Token `on-surface-variant`.
- **Graphite (#41413F):** Muted text and metadata, seen 8 times. Token `on-surface-muted`.
- **Slate (#777879):** Subtle text and placeholders, seen 6 times. Token `on-surface-subtle`.
- **White 90% (#FFFFFFE6):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **White (#FFFFFF):** Cards and panels, seen 4 times. Token `surface-container`, CSS `--card`.
- **Mist (#EFEFEF):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Pale Blue (#DBEDFE):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Near Black 5% (#0000000D):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **Near Black 4% (#0000000A):** Stronger translucent fill, seen 6 times. Token `overlay-strong`.
- **White 30% (#FFFFFF4D):** Borders and dividers, seen 4 times. Token `outline`.
- **Near Black 9% (#03030217):** Secondary dividers, seen 2 times. Token `outline-variant`, CSS `--border`.
- **Light Blue (#B8CAF5):** Brand color on large areas. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Light Cyan (#AADAF1):** Brand color in logos and imagery, seen 38 times. Token `secondary`.
- **Vivid Blue (#0087FF):** Most used accent color, seen 8 times. Token `tertiary`.

## Typography

**UntitledSerifFont**, **UntitledSansFont** and **apple-system** share the interface. Fallback stack: `UntitledSerifFont, UntitledSerifFont Fallback, apple-system-ui-serif, ui-serif`. Other loaded fonts: UntitledSansFont Fallback, InterFont, InterFont Fallback, UntitledSerifFont Fallback.

- **headline-display:** UntitledSerifFont 66px at weight 400, line height 1, tracking -0.03em (48px on mobile). Page title (h1).
- **headline-lg:** UntitledSerifFont 54px at weight 400, line height 1.1, tracking -0.02em (38px on mobile). Section headings (h2).
- **headline-md:** UntitledSerifFont 46px at weight 400, line height 1.22, tracking -0.03em. Sub-section headings.
- **headline-sm:** UntitledSerifFont 36px at weight 400, line height 1.22, tracking -0.03em. Card and feature titles.
- **title-lg:** UntitledSerifFont 30px at weight 400, line height 1, tracking -0.03em. Small titles.
- **body-md:** UntitledSansFont 14px at weight 400, line height 1.5. Body text.
- **body-lg:** apple-system 15px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** apple-system 12px at weight 400, line height 1.4, tracking -0.02em. Secondary and small text.
- **label-md:** UntitledSansFont 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** UntitledSansFont 14px at weight 500, line height 1.5, tracking 0.01em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 67% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 5px, md 16px, lg 24px, xl 60px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 920px.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 375px, 390px, 400px, 424px, 425px, 445px, 460px, 480px, 500px, 550px, 700px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.01) 0px 50px 40px 0px, rgba(0, 0, 0, 0.02) 0px 50px 40px 0px, rgba(0, 0, 0, 0.05) 0px 20px 40px 0px, rgba(0, 0, 0, 0.08) 0px 3px 10px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 12px 12px 2px, rgba(0, 0, 0, 0.06) 0px 2px 4px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`

## Shapes

Most elements use 24px corners. Measured radii, most used first:

- **xl (24px):** 36 elements.
- **xs (4px):** 28 elements.
- **sm (8px):** 24 elements.
- **md (12px):** 16 elements.
- **lg (14px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try Craft Free”):** #030302 fill, #FFFFFF text, 16px/500, 3.35544e+07px radius, padding 8px 14px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`.
- **button-primary-hover:** background #030302BF, text #FFFFFF on hover.
- **button-ghost (“Product”):** transparent fill, #030302 text, 16px/400, padding 0px.
- **card:** #FF4500 fill, #030302 text, 16px/400, 24px radius, padding 24px, shadow `rgba(0, 0, 0, 0.01) 0px 50px 40px 0px, rgba(0, 0, 0, 0.02) 0px 50px 40px 0px, rgba(0, 0, 0, 0.05) 0px 20px 40px 0px, rgba(0, 0, 0, 0.08) 0px 3px 10px 0px`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #FCF9F7 for the page and lift surfaces in small steps: #FFFFFFE6, #FFFFFF, #EFEFEF, #DBEDFE.
- Do keep text in 4 levels: #030302, #1B1B1A, #41413F, #777879.
- Do use #B8CAF5 as the brand accent: header, logo and key highlights.
- Do set headlines in UntitledSerifFont with tight tracking (-0.03em).
- Do reuse the measured spacing steps (5px, 16px, 24px).
- Do use 24px corners on most elements; larger surfaces also use 4px, 8px and 12px.
- Don't use #777879 for body text; it reaches 4.2:1 on #FCF9F7. Keep it for large text or metadata.
- Don't introduce new font families beyond UntitledSerifFont, UntitledSansFont and apple-system.
- Don't use #B8CAF5 for large backgrounds or body text.
- Don't make interface transitions slower than 0.00001s.

## Motion

Interface transitions are quick: 1e-05s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/craft.do/), the free DESIGN.md generator.
