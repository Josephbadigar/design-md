---
version: alpha
name: Google Cloud
description: "Light interface measured from cloud.google.com: Google Sans type with Roboto, pale blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#5F6368"
  on-background: "#5F6368"
  on-surface-strong: "#202124"
  on-surface-variant: "#212226"
  on-surface-muted: "#444746"
  surface-container-low: "#F8F9FC"
  outline: "#E6EAF0"
  primary: "#D3E3FD"
  on-primary: "#0842A0"
  secondary: "#2051DA"
  tertiary: "#0B57D0"
typography:
  headline-display:
    fontFamily: Google Sans
    fontSize: 45px
    fontWeight: 500
    lineHeight: 1.16
  headline-lg:
    fontFamily: Google Sans
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.22
  body-md:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.14
  body-lg:
    fontFamily: Google Sans Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Google Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Google Sans Text
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: 0.008em
  headline-display-mobile:
    fontFamily: Google Sans
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.29
rounded:
  sm: 4px
  md: 8px
  lg: 20px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 36px
  gutter: 16px
  section: 80px
  container: 1296px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 16px
    padding: 0px 20px 0px 16px
    height: 56px
  button-primary-hover:
    backgroundColor: "#C2D7FA"
  button-ghost:
    textColor: "#000000"
    typography: "{typography.body-lg}"
    padding: 0px
  link:
    textColor: "{colors.secondary}"
---

# Google Cloud Design System

## Overview

Google Cloud describes itself as: “Meet your business challenges head on with AI and cloud computing services from Google, including security, data management, and hybrid & multi-cloud.” The interface is light, built on **White (#FFFFFF)** with **Cool Slate (#5F6368)** text, and **Pale Blue (#D3E3FD)** as the main accent.

Type is set in **Google Sans** and **Roboto**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [cloud.google.com](https://cloud.google.com/) on November 4, 2026 at 1440×900 and 390×844 from 336 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 13 times. Token `background`.
- **Cool Slate (#5F6368):** Primary text and headings, seen 24 times. Token `on-surface`.
- **Charcoal (#202124):** Headings and emphasis, seen 29 times. Token `on-surface-strong`.
- **Charcoal (#212226):** Secondary text, seen 13 times. Token `on-surface-variant`.
- **Graphite (#444746):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Snow (#F8F9FC):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`.
- **Cool Mist (#E6EAF0):** Borders and dividers, seen 9 times. Token `outline`.
- **Pale Blue (#D3E3FD):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **Dark Blue (#0842A0):** Text and icons on primary. Token `on-primary`.
- **Blue (#2051DA):** Accent in text, fills and borders, seen 15 times. Token `secondary`.
- **Vivid Blue (#0B57D0):** Accent in text, fills and borders, seen 6 times. Token `tertiary`.

## Typography

**Google Sans**, **Roboto** and **Google Sans Text** share the interface. Fallback stack: `Google Sans, Roboto, Arial, sans-serif`. Other loaded fonts: Material Icons Extended, Google Material Icons, Google Symbols.

- **headline-display:** Google Sans 45px at weight 500, line height 1.16 (28px on mobile). Page title (h1).
- **headline-lg:** Google Sans 36px at weight 500, line height 1.22. Section headings (h2).
- **body-md:** Roboto 14px at weight 400, line height 1.14. Body text.
- **body-lg:** Google Sans Text 16px at weight 400, line height 1.5. Lead paragraphs.
- **label-md:** Google Sans 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Google Sans Text 12px at weight 500, line height 1.33, tracking 0.008em, uppercase. Small labels and badges.

## Layout

Spacing follows a 4px grid: 93% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 36px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1296px.
- **Breakpoints:** 319px, 350px, 480px, 592px, 640px, 672px, 720px, 960px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(60, 64, 67, 0.3) 0px 1px 2px 0px, rgba(60, 64, 67, 0.15) 0px 1px 3px 1px`
- `rgba(60, 64, 67, 0.3) 0px 1px 3px 0px, rgba(60, 64, 67, 0.15) 0px 4px 8px 3px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **lg (20px):** 92 elements.
- **sm (4px):** 90 elements.
- **full (9999px):** 68 elements.
- **md (8px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Ask Google Cloud”):** #D3E3FD fill, #0842A0 text, 16px/500, 16px radius, padding 0px 20px 0px 16px, shadow `rgba(60, 64, 67, 0.3) 0px 1px 3px 0px, rgba(60, 64, 67, 0.15) 0px 4px 8px 3px`.
- **button-primary-hover:** background #C2D7FA, text #0842A0 on hover.
- **button-ghost (“chevron_left”):** transparent fill, #000000 text, 16px/400, 50% radius, padding 0px.
- **link:** transparent fill, #2051DA text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F8F9FC.
- Do keep text in 4 levels: #5F6368, #202124, #212226, #444746.
- Do reserve #D3E3FD for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 20px corners.
- Don't introduce new font families beyond Google Sans, Roboto and Google Sans Text.
- Don't use #D3E3FD for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.5s, 0.35s, 0.075s.

- **Easing:** `ease`, `ease-in-out`, `cubic-bezier(0.2, 0, 0, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cloud.google.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
