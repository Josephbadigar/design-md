---
version: alpha
name: Firebase
description: "Dark interface measured from firebase.google.com: Google Sans type with Material Icons, vivid orange accents, flat surfaces and 100px corners."
colors:
  background: "#1E1E1E"
  surface: "#1E1E1E"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  overlay: "#FFFFFF99"
  outline: "#323232"
  outline-variant: "#041E4933"
  primary: "#F57C00"
  on-primary: "#000000"
  secondary: "#FF9100"
  tertiary: "#1765CC"
typography:
  headline-display:
    fontFamily: Google Sans
    fontSize: 75px
    fontWeight: 700
    lineHeight: 1.33
  headline-lg:
    fontFamily: Google Sans
    fontSize: 35px
    fontWeight: 700
    lineHeight: 1.29
  body-md:
    fontFamily: Google Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Google Sans
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.33
  body-sm:
    fontFamily: Google Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.14
  caption:
    fontFamily: Google Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.3
  label-lg:
    fontFamily: Material Icons
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1
  label-md:
    fontFamily: Google Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Google Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  code:
    fontFamily: JetBrains Mono
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
  headline-display-mobile:
    fontFamily: Google Sans
    fontSize: 45px
    fontWeight: 700
    lineHeight: 1.44
  headline-lg-mobile:
    fontFamily: Google Sans
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.5
rounded:
  sm: 4px
  md: 8px
  lg: 20px
  xl: 100px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.xl}"
    padding: 10px 20px
    height: 42px
  button-primary-hover:
    backgroundColor: "#FFA000"
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.xl}"
    padding: 5px 20px
    height: 38px
  button-outline-hover:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.xl}"
    padding: 5px 20px
    height: 36px
  input-field:
    backgroundColor: "#F1F3F4"
    textColor: "#00000099"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 8px 8px 8px 40px
  card:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
    padding: 32px
  link:
    textColor: "{colors.on-primary}"
---

# Firebase Design System

## Overview

Firebase describes itself as: “Discover Firebase, Google’s mobile and web app development platform that helps developers build apps and games that users will love.” The interface is dark, built on **Charcoal (#1E1E1E)** with **White (#FFFFFF)** text, and **Vivid Orange (#F57C00)** as the main accent.

Type is set in **Google Sans** and **Material Icons**, with **JetBrains Mono** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 100px.

Measured from [firebase.google.com](https://firebase.google.com/) on November 4, 2026 at 1440×900 and 390×844 from 267 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Charcoal (#1E1E1E):** Page background. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 20 times. Token `on-surface`, CSS `--tenant-background-1`.
- **White 60% (#FFFFFF99):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Graphite (#323232):** Borders and dividers, seen 4 times. Token `outline`.
- **Deep Blue 20% (#041E4933):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Orange (#F57C00):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#FF9100):** Accent in text, fills and borders, seen 11 times. Token `secondary`, CSS `--firebase-cta-orange`.
- **Blue (#1765CC):** Accent (CSS variable). Token `tertiary`.

## Typography

**Google Sans**, **Material Icons** and **JetBrains Mono** (monospace) share the interface. Fallback stack: `Google Sans, sans-serif`.

- **headline-display:** Google Sans 75px at weight 700, line height 1.33 (45px on mobile). Page title (h1).
- **headline-lg:** Google Sans 35px at weight 700, line height 1.29 (20px on mobile). Section headings (h2).
- **body-md:** Google Sans 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Google Sans 18px at weight 700, line height 1.33. Lead paragraphs.
- **body-sm:** Google Sans 14px at weight 400, line height 1.14. Secondary and small text.
- **caption:** Google Sans 12px at weight 400, line height 1.3. Captions and fine print.
- **label-lg:** Material Icons 24px at weight 400, line height 1. Large buttons and tabs.
- **label-md:** Google Sans 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Google Sans 14px at weight 500, line height 1.43. Small labels and badges.
- **code:** JetBrains Mono 20px at weight 400, line height 1.2. Code and technical values.

## Layout

Spacing does not follow a strict grid: 63% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 40px.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 420px, 600px, 700px, 720px, 800px, 920px, 1000px, 1200px, 1280px, 1440px, 2000px, 2400px, 3200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.15) 0px 4px 12px 0px`

## Shapes

Most elements use 100px corners. Measured radii, most used first:

- **xl (100px):** 40 elements.
- **sm (4px):** 36 elements.
- **lg (20px):** 20 elements.
- **md (8px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #F57C00 fill, #000000 text, 18px/700, 100px radius, padding 10px 20px.
- **button-primary-hover:** background #FFA000, text #000000 on hover.
- **button-outline (“Get started in console”):** transparent fill, #FFFFFF text, 18px/700, 100px radius, padding 5px 20px, border 2px solid #FF9100.
- **button-outline-hover:** background #FF9100, text #000000 on hover.
- **button-ghost (“View generative AI options”):** transparent fill, #000000 text, 18px/700, 100px radius, padding 5px 20px, border 2px solid #FF9100.
- **input-field (“Search”):** #F1F3F4 fill, #00000099 text, 16px/400, padding 8px 8px 8px 40px.
- **card:** #FFFFFF99 fill, #000000 text, 22px/400, 20px radius, padding 32px, shadow `rgba(0, 0, 0, 0.15) 0px 4px 12px 0px`.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #1E1E1E for the page.
- Do reserve #F57C00 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 100px corners on most elements; larger surfaces also use 4px, 20px and 8px.
- Don't introduce new font families beyond Google Sans, Material Icons and JetBrains Mono.
- Don't use #F57C00 for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.2s, 0.25s, 0.1s.

- **Easing:** `ease`, `cubic-bezier(0, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/firebase.google.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
