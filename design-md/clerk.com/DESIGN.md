---
version: alpha
name: Clerk
description: "Light monochrome interface measured from clerk.com: geistNumbers type with system-ui, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#131316"
  on-background: "#131316"
  on-surface-strong: "#000000"
  on-surface-variant: "#5E5F6E"
  on-surface-muted: "#747686"
  surface-container-low: "#F7F7F8"
  surface-container: "#EEEEF0"
  overlay: "#F7F7F8D9"
  overlay-strong: "#1313160D"
  outline: "#00000033"
  primary: "#42434D"
  on-primary: "#FFFFFF"
  secondary: "#6C47FF"
  tertiary: "#9785FF"
typography:
  headline-display:
    fontFamily: geistNumbers
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.14
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: geistNumbers
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.015em
  headline-md:
    fontFamily: geistNumbers
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: -0.01em
  body-md:
    fontFamily: system-ui
    fontSize: 17px
    fontWeight: 700
    lineHeight: 1.41
    letterSpacing: -0.01em
  body-sm:
    fontFamily: geistNumbers
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.54
  caption:
    fontFamily: system-ui
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.27
  label-lg:
    fontFamily: geistNumbers
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.43
    letterSpacing: -0.01em
  label-sm:
    fontFamily: geistNumbers
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.85
  headline-display-mobile:
    fontFamily: geistNumbers
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.12
    letterSpacing: -0.015em
rounded:
  sm: 6px
  md: 12px
  lg: 12.5px
  xl: 22px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 8px
  section: 164px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
    height: 30px
  button-secondary:
    backgroundColor: "#212126"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    padding: 0px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px 8px 0px 0px
  link:
    textColor: "{colors.on-surface}"
---

# Clerk Design System

## Overview

Clerk describes itself as: “The easiest way to add authentication and user management to your application. Purpose-built for React, Next.js, Remix, and “The Modern Web”.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#131316)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **geistNumbers** and **system-ui**. Headlines run large with tight negative tracking; body text is 17px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 12px.

Measured from [clerk.com](https://clerk.com/) on October 29, 2026 at 1440×900 and 390×844 from 398 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #E0876A, #D97757.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`, CSS `--color-white`.
- **Charcoal (#131316):** Primary text and headings, seen 52 times. Token `on-surface`, CSS `--typography-link`.
- **Near Black (#000000):** Headings and emphasis, seen 8 times. Token `on-surface-strong`.
- **Cool Slate (#5E5F6E):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **Cool Slate (#747686):** Muted text and metadata, seen 9 times. Token `on-surface-muted`, CSS `--color-gray-500`.
- **Snow (#F7F7F8):** Raised areas one step from the page, seen 14 times. Token `surface-container-low`.
- **Mist (#EEEEF0):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--color-gray-100`.
- **Snow 85% (#F7F7F8D9):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Charcoal 5% (#1313160D):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Near Black 20% (#00000033):** Borders and dividers, seen 10 times. Token `outline`.
- **Cool Graphite (#42434D):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Violet (#6C47FF):** Accent in text, fills and borders, seen 5 times. Token `secondary`.
- **Light Indigo (#9785FF):** Accent in text, fills and borders, seen 2 times. Token `tertiary`.

## Typography

**geistNumbers** and **system-ui** share the interface. Fallback stack: `geistNumbers, suisse, suisse Fallback`. Other loaded fonts: suisse, soehneMono, Inter.

- **headline-display:** geistNumbers 56px at weight 700, line height 1.14, tracking -0.035em (32px on mobile). Page title (h1).
- **headline-lg:** geistNumbers 32px at weight 600, line height 1.25, tracking -0.015em. Section headings (h2).
- **headline-md:** geistNumbers 24px at weight 500, line height 1.33, tracking -0.01em. Sub-section headings.
- **body-md:** system-ui 17px at weight 700, line height 1.41, tracking -0.01em. Body text.
- **body-sm:** geistNumbers 13px at weight 400, line height 1.54. Secondary and small text.
- **caption:** system-ui 11px at weight 400, line height 1.27. Captions and fine print.
- **label-lg:** geistNumbers 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** system-ui 14px at weight 700, line height 1.43, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** geistNumbers 13px at weight 500, line height 1.85. Small labels and badges.

## Layout

Spacing follows a 4px grid: 90% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 40px.
- **Sections:** 164px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F7F7F8 → #EEEEF0):

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0.999994 0.0000455678 0.0000200868 / 0.05) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, lab(84.5189 -31.4667 -23.9754 / 0.08) 0px 0px 0px 1px inset, rgba(0, 0, 0, 0) 0px 0px 0px 0px`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 0px 0px 0.5px, rgba(0, 0, 0, 0.06) 0px 2px 10px -4px, rgba(0, 0, 0, 0.06) 0px 8px 12px -4px, rgba(255, 255, 255, 0.8) 0px 0px 0px 0.5px inset, rgb(255, 255, 255) 0px 0px 24px 6px inset`.

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **md (12px):** 48 elements.
- **lg (12.5px):** 20 elements.
- **xl (22px):** 14 elements.
- **sm (6px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Skip to main content”):** #42434D fill, #FFFFFF text, 13px/500, 6px radius, padding 0px 12px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(66, 67, 77) 0px 0px 0px 0.5px, oklab(0.999994 0.0000455678 0.0000200868 / 0.07) 0px 1px 0px 0px inset, oklab(0.249859 0.00254738 -0.00901626 / 0.2) 0px 1px 3px 0px`.
- **button-secondary (“Support”):** #212126 fill, #FFFFFF text, 16px/400, 3.35544e+07px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0 0 0 / 0.075) 0px 0px 0px 6px, oklab(0.999994 0.0000455678 0.0000200868 / 0.075) 0px 1px 0px 0px inset, oklab(0.249859 0.00254738 -0.00901626 / 0.2) 0px 1px 3px 0px, rgb(33, 33, 38) 0px 0px 0px 1px`.
- **button-ghost (“Products”):** transparent fill, #131316 text, 16px/400, padding 0px 8px 0px 0px.
- **link:** transparent fill, #131316 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F7F8, #EEEEF0.
- Do keep text in 4 levels: #131316, #000000, #5E5F6E, #747686.
- Do let contrast carry emphasis; primary actions use #42434D on #FFFFFF.
- Do set headlines in geistNumbers with tight tracking (-0.035em).
- Do keep spacing on the 4px grid.
- Do use 12px corners on most elements; larger surfaces also use 12.5px, 22px and 6px.
- Don't use #747686 for body text; it reaches 4.49:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond geistNumbers and system-ui.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.45s.

## Motion

Interface transitions are quick: 0.15s, 0.45s, 0.2s, 0.35s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.33, 1, 0.68, 1)`, `linear(0 0%, 0.1812 9.09091%, 0.4669 18.1818%, 0.6943 27.2727%, 0.8403 36.3636%, 0.9233 45.4545%, 0.9664 54.5455%, 0.9869 63.6364%, 0.9958 72.7273%, 0.9992 81.8182%, 1.0003 90.9091%, 1 100%)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/clerk.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
