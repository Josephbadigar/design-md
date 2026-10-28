---
version: alpha
name: Cal.com
description: "Light monochrome interface measured from cal.com: Cal Sans type with Cal Sans UI Variable Light, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#111111"
  on-background: "#111111"
  on-surface-variant: "#242424"
  on-surface-muted: "#292929"
  on-surface-subtle: "#898989"
  surface-container-low: "#F5F5F5"
  surface-container: "#F4F4F4"
  overlay: "#FFFFFFCC"
  outline: "#CBCBCB"
  outline-variant: "#1414141A"
  primary: "#111111"
  on-primary: "#FFFFFF"
  secondary: "#0099FF"
  warning: "#FFC107"
  error: "#FF3D00"
typography:
  headline-display:
    fontFamily: Cal Sans
    fontSize: 64px
    fontWeight: 600
    lineHeight: 1.1
  headline-lg:
    fontFamily: Cal Sans
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.1
  headline-md:
    fontFamily: Cal Sans
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.3
  headline-sm:
    fontFamily: Cal Sans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: 0.01em
  body-md:
    fontFamily: Cal Sans UI Variable Light
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.4
  body-lg:
    fontFamily: Cal Sans UI Variable Light
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
  body-sm:
    fontFamily: Matter Regular
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.14
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.14
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1
  label-sm:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: 500
    lineHeight: 1.43
  code:
    fontFamily: Roboto Mono
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Cal Sans
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: Cal Sans
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.1
rounded:
  sm: 7px
  md: 12px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  gutter: 8px
components:
  button-primary:
    textColor: "#0000EE"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 36px
  button-secondary:
    textColor: "#0000EE"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 36px
  button-tertiary:
    textColor: "#0000EE"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 36px
  link:
    textColor: "{colors.primary}"
---

# Cal.com Design System

## Overview

Cal.com describes itself as: “A fully customizable scheduling software for individuals, businesses taking calls and developers building scheduling platforms where users meet users.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#111111)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Cal Sans** and **Cal Sans UI Variable Light**, with **Roboto Mono** for code. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [cal.com](https://cal.com/) on October 21, 2026 at 1440×900 and 390×844 from 404 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 7 times. Token `background`, CSS `--sj-tw-ring-offset-color`.
- **Charcoal (#111111):** Primary text and headings, seen 59 times. Token `on-surface`.
- **Graphite (#242424):** Secondary text, seen 47 times. Token `on-surface-variant`.
- **Graphite (#292929):** Muted text and metadata, seen 16 times. Token `on-surface-muted`.
- **Gray (#898989):** Subtle text and placeholders, seen 43 times. Token `on-surface-subtle`.
- **Snow (#F5F5F5):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F4F4F4):** Cards and panels, seen 1 time. Token `surface-container`.
- **White 80% (#FFFFFFCC):** Translucent fill for cards and controls, seen 8 times. Token `overlay`.
- **Silver (#CBCBCB):** Borders and dividers, seen 9 times. Token `outline`.
- **Charcoal 10% (#1414141A):** Secondary dividers, seen 7 times. Token `outline-variant`.
- **Charcoal (#111111):** Primary actions (the main text color; the palette is monochrome), seen 59 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0099FF):** Most used accent color, seen 3 times. Token `secondary`.
- **Vivid Amber (#FFC107):** Warnings and highlights, seen 1 time. Token `warning`.
- **Vivid Red (#FF3D00):** Errors and destructive states, seen 1 time. Token `error`.

## Typography

**Cal Sans**, **Cal Sans UI Variable Light**, **Matter Regular**, **Inter** and **Roboto Mono** (monospace) share the interface. Fallback stack: `Cal Sans, Cal Sans Placeholder, sans-serif`. Other loaded fonts: Matter SemiBold, Matter Medium.

- **headline-display:** Cal Sans 64px at weight 600, line height 1.1 (40px on mobile). Page title (h1).
- **headline-lg:** Cal Sans 48px at weight 600, line height 1.1 (32px on mobile). Section headings (h2).
- **headline-md:** Cal Sans 24px at weight 600, line height 1.3. Sub-section headings.
- **headline-sm:** Cal Sans 20px at weight 600, line height 1, tracking 0.01em. Card and feature titles.
- **body-md:** Cal Sans UI Variable Light 14px at weight 300, line height 1.4. Body text.
- **body-lg:** Cal Sans UI Variable Light 16px at weight 300, line height 1.5. Lead paragraphs.
- **body-sm:** Matter Regular 12px at weight 400, line height 1.5. Secondary and small text.
- **caption:** Inter 10px at weight 400, line height 1.14. Captions and fine print.
- **label-lg:** Inter 14px at weight 500, line height 1.14. Large buttons and tabs.
- **label-md:** Inter 12px at weight 500, line height 1. Buttons, navigation and labels.
- **label-sm:** Inter 10px at weight 500, line height 1.43. Small labels and badges.
- **code:** Roboto Mono 14px at weight 600, line height 1. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (84% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 768px, 809px, 809.98px, 810px, 1024px, 1199px, 1199.98px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#F5F5F5 → #F4F4F4):

- `rgba(255, 255, 255, 0.15) 0px 2px 0px 0px inset`
- `rgb(255, 255, 255) 0px 2px 0px 0px inset`

A few raised panels add a soft drop shadow: `rgba(34, 42, 53, 0.05) 0px 4px 8px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (12px):** 60 elements.
- **sm (7px):** 36 elements.
- **full (9999px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** transparent fill, #0000EE text, 12px/400, 12px radius, padding 8px 12px, shadow `rgba(255, 255, 255, 0.15) 0px 2px 0px 0px inset`.
- **button-secondary (“Sign up with email”):** transparent fill, #0000EE text, 12px/400, 12px radius, padding 8px 12px, shadow `rgb(255, 255, 255) 0px 2px 0px 0px inset`.
- **button-tertiary (“Book a demo”):** transparent fill, #0000EE text, 12px/400, 12px radius, padding 8px 12px, shadow `rgb(255, 255, 255) 0px 2px 0px 0px inset`.
- **link:** transparent fill, #111111 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F5F5F5, #F4F4F4.
- Do keep text in 4 levels: #111111, #242424, #292929, #898989.
- Do let contrast carry emphasis; primary actions use #111111 on #FFFFFF.
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 12px corners.
- Don't use #898989 for body text; it reaches 3.5:1 on #FFFFFF. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Cal Sans, Cal Sans UI Variable Light, Matter Regular, Inter and Roboto Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cal.com/), the free DESIGN.md generator.
