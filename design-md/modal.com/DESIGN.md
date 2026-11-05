---
version: alpha
name: Modal
description: "Dark interface measured from modal.com: ABC Diatype type, green accents, tonal surfaces and 48px corners."
colors:
  background: "#040804"
  surface: "#040804"
  on-surface: "#A8ABA6"
  on-background: "#A8ABA6"
  on-surface-strong: "#EEF2EB"
  on-surface-variant: "#E3E5E1"
  surface-container-low: "#10120F"
  surface-container: "#181818"
  overlay: "#FFFFFF0D"
  overlay-strong: "#9EFB871A"
  outline: "#FFFFFF0D"
  outline-variant: "#FFFFFF1A"
  primary: "#7FEE64"
  on-primary: "#000000"
  secondary: "#62DE61"
  tertiary: "#09AF58"
typography:
  headline-display:
    fontFamily: ABC Diatype
    fontSize: 45px
    fontWeight: 500
    lineHeight: 1.07
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: ABC Diatype
    fontSize: 38px
    fontWeight: 500
    lineHeight: 1.16
    letterSpacing: -0.01em
  body-md:
    fontFamily: ABC Diatype
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: ABC Diatype
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.33
  body-sm:
    fontFamily: ABC Diatype
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.47
    letterSpacing: 0.01em
  label-md:
    fontFamily: ABC Diatype
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: ABC Diatype
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.54
    letterSpacing: 0.03em
  code:
    fontFamily: DM Mono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.67
    letterSpacing: 0.03em
  headline-display-mobile:
    fontFamily: ABC Diatype
    fontSize: 37px
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: ABC Diatype
    fontSize: 31px
    fontWeight: 500
    lineHeight: 1.16
rounded:
  sm: 7px
  md: 10px
  lg: 48px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 20px
  xl: 48px
  gutter: 20px
  section: 144px
  margin: 64px
  container: 1546px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 4px 12px
    height: 32px
  button-outline:
    backgroundColor: "#1A1C19"
    textColor: "#FDFD76"
    typography: "{typography.code}"
    rounded: "{rounded.md}"
    padding: 24px 32px
    height: 64px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 0px 12px
  card:
    backgroundColor: "#1A1C19"
    textColor: "{colors.on-surface-variant}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Modal Design System

## Overview

Modal describes itself as: “Cloud infrastructure for teams that develop, train, and serve AI applications at scale.” The interface is dark, built on **Near Black (#040804)** with **Gray (#A8ABA6)** text, and **Green (#7FEE64)** as the main accent.

Type is set in **ABC Diatype**, with **DM Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 48px.

Measured from [modal.com](https://modal.com/) on November 4, 2026 at 1440×900 and 390×844 from 416 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Near Black (#040804):** Page background, seen 4 times. Token `background`, CSS `--color-v2-primary-black`.
- **Gray (#A8ABA6):** Primary text and headings, seen 48 times. Token `on-surface`.
- **Mist (#EEF2EB):** Headings and emphasis, seen 34 times. Token `on-surface-strong`.
- **Mist (#E3E5E1):** Secondary text, seen 37 times. Token `on-surface-variant`.
- **Charcoal (#10120F):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Charcoal (#181818):** Cards and panels, seen 7 times. Token `surface-container`, CSS `--color-deprecated-ground`.
- **White 5% (#FFFFFF0D):** Translucent fill for cards and controls, seen 9 times. Token `overlay`.
- **Light Green 10% (#9EFB871A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 5% (#FFFFFF0D):** Borders and dividers, seen 14 times. Token `outline`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 5 times. Token `outline-variant`, CSS `--color-raw-gray-alpha-100-opacity-10`.
- **Green (#7FEE64):** Brand accent (CSS variable), seen 11 times. Token `primary`, CSS `--semantic-icon-primary-selected`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Green (#62DE61):** Accent in the logo, seen 1 time. Token `secondary`.
- **Dark Green (#09AF58):** Accent in the logo, seen 2 times. Token `tertiary`.

## Typography

**ABC Diatype** and **DM Mono** (monospace) share the interface. Fallback stack: `ABC Diatype, ABC Diatype Fallback, Arial, ui-sans-serif`.

- **headline-display:** ABC Diatype 45px at weight 500, line height 1.07, tracking -0.01em (37px on mobile). Page title (h1).
- **headline-lg:** ABC Diatype 38px at weight 500, line height 1.16, tracking -0.01em (31px on mobile). Section headings (h2).
- **body-md:** ABC Diatype 16px at weight 400, line height 1.5. Body text.
- **body-lg:** ABC Diatype 18px at weight 400, line height 1.33. Lead paragraphs.
- **body-sm:** ABC Diatype 15px at weight 400, line height 1.47, tracking 0.01em. Secondary and small text.
- **label-md:** ABC Diatype 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** ABC Diatype 13px at weight 500, line height 1.54, tracking 0.03em. Small labels and badges.
- **code:** DM Mono 12px at weight 400, line height 1.67, tracking 0.03em. Code and technical values.

## Layout

Spacing does not follow a strict grid: 64% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 6px, md 12px, lg 20px, xl 48px.
- **Sections:** 144px vertical padding between major sections.
- **Gaps:** 20px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1546px.
- **Page margin:** 64px on each side of full-width sections.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#10120F → #181818):

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

A few raised panels add a soft drop shadow: `rgba(4, 8, 4, 0.5) 0px 1px 3px 0px, rgba(4, 8, 4, 0.6) 0px 2px 32px 0px`.

## Shapes

Most elements use 48px corners. Measured radii, most used first:

- **lg (48px):** 204 elements.
- **md (10px):** 20 elements.
- **sm (7px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #E3E5E1 fill, #10120F text, 15px/500, 48px radius, padding 4px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-outline (“modal endpo |”):** #1A1C19 fill, #FDFD76 text, 12px/400, 10px radius, padding 24px 32px, shadow `rgba(4, 8, 4, 0.5) 0px 1px 3px 0px, rgba(4, 8, 4, 0.6) 0px 2px 32px 0px`.
- **button-ghost (“Product”):** transparent fill, #A8ABA6 text, 15px/400, 48px radius, padding 0px 12px.
- **card:** #1A1C19 fill, #E3E5E1 text, 10px/400, 10px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(4, 8, 4, 0.4) 0px 1px 3px 0px, rgba(4, 8, 4, 0.5) 0px 2px 32px 0px`.
- **link:** transparent fill, #A8ABA6 text, padding 0px.

## Do's and Don'ts

- Do use #040804 for the page and lift surfaces in small steps: #10120F, #181818.
- Do keep text in 3 levels: #A8ABA6, #EEF2EB, #E3E5E1.
- Do use #7FEE64 as the brand accent: header, logo and key highlights.
- Do set headlines in ABC Diatype with tight tracking (-0.01em).
- Do reuse the measured spacing steps (6px, 12px, 20px).
- Do use 48px corners on most elements; larger surfaces also use 10px and 7px.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond ABC Diatype and DM Mono.
- Don't use #7FEE64 for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.16s, 0.25s. Longer ambient animations run 1s, 3.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `cubic-bezier(0.165, 0.84, 0.44, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/modal.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
