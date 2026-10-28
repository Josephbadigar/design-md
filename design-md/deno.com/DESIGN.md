---
version: alpha
name: Deno
description: "Dark monochrome interface measured from deno.com: Inter type, tonal surfaces and 4px corners."
colors:
  background: "#001319"
  surface: "#001319"
  on-surface: "#868789"
  on-background: "#868789"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#9EA0A5"
  on-surface-muted: "#56575A"
  surface-container-low: "#121417"
  surface-container: "#25272B"
  outline: "#25272B"
  outline-variant: "#172723"
  primary: "#25272B"
  on-primary: "#000000"
  secondary: "#F5F5F5"
  tertiary: "#3ECC5F"
  success: "#70FFAF"
  warning: "#FFD601"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 72px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Inter
    fontSize: 44px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.25
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
  code:
    fontFamily: Menlo
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 39.25px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  headline-md-mobile:
    fontFamily: Inter
    fontSize: 23.7px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
rounded:
  sm: 4px
  md: 6px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 48px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 2px
    height: 60px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    padding: 4px 10px 4px 4px
    height: 34px
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.caption}"
    rounded: 0px
    padding: 6px 16px
    height: 29px
  button-ghost:
    textColor: "{colors.outline-variant}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  input-field:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: 8px
    padding: 4px 4px 4px 32px
  link:
    textColor: "#C2C4C7"
---

# Deno Design System

## Overview

Deno describes itself as: “A drop-in JavaScript runtime with built-in TypeScript, npm support, and security by default. Run your existing Node project on Deno with no setup.” The interface is dark, built on **Deep Cyan (#001319)** with **Gray (#868789)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Inter**, with **Menlo** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [deno.com](https://deno.com/) on October 21, 2026 at 1440×900 and 390×844 from 434 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #70FFAF.

- **Deep Cyan (#001319):** Page background. Token `background`.
- **Gray (#868789):** Primary text and headings, seen 53 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 49 times. Token `on-surface-strong`, CSS `--color-white`.
- **Cool Gray (#9EA0A5):** Secondary text, seen 12 times. Token `on-surface-variant`, CSS `--color-gray-500`.
- **Slate (#56575A):** Muted text and metadata, seen 11 times. Token `on-surface-muted`.
- **Charcoal (#121417):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Cool Graphite (#25272B):** Cards and panels, seen 2 times. Token `surface-container`.
- **Cool Graphite (#25272B):** Borders and dividers, seen 10 times. Token `outline`.
- **Charcoal (#172723):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Cool Graphite (#25272B):** Primary buttons and calls to action, seen 24 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Snow (#F5F5F5):** Secondary call-to-action fill, seen 1 time. Token `secondary`.
- **Green (#3ECC5F):** Accent, seen 4 times. Token `tertiary`.
- **Light Green (#70FFAF):** Success and positive states, seen 23 times. Token `success`, CSS `--color-runtime`.
- **Vivid Amber (#FFD601):** Warnings and highlights, seen 2 times. Token `warning`.

## Typography

**Inter** and **Menlo** (monospace) share the interface. Fallback stack: `Inter, ui-sans-serif, system-ui, -apple-system`. Other loaded fonts: Moranga, Recursive.

- **headline-display:** Inter 72px at weight 700, line height 1.1, tracking -0.025em (39.25px on mobile). Page title (h1).
- **headline-lg:** Inter 44px at weight 700, line height 1.1, tracking -0.025em. Section headings (h2).
- **headline-md:** Inter 36px at weight 700, line height 1.1, tracking -0.025em (23.7px on mobile). Sub-section headings.
- **headline-sm:** Inter 20px at weight 700, line height 1.1, tracking -0.025em. Card and feature titles.
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1.43. Secondary and small text.
- **caption:** Inter 12px at weight 400, line height 1.33. Captions and fine print.
- **label-lg:** Inter 16px at weight 700, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 14px at weight 700, line height 1.25. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.33. Small labels and badges.
- **code:** Menlo 12px at weight 400, line height 1.33. Code and technical values.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 440px, 1024px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 10px 15px -3px, rgba(0, 0, 0, 0.1) 0px 4px 6px -4px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 256 elements.
- **md (6px):** 32 elements.
- **full (9999px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #25272B fill, #000000 text, 16px/400, 9999px radius, padding 2px.
- **button-outline (“v2.9 What’s new in Deno→”):** #121417 fill, #000000 text, 14px/400, 3.35544e+07px radius, padding 4px 10px 4px 4px, border 1px solid #70FFAF66.
- **button-secondary (“MacOS/Linux”):** #F5F5F5 fill, #9EA0A5 text, 12px/400, padding 6px 16px.
- **button-ghost (“Dismiss”):** transparent fill, #172723 text, 16px/400, padding 0px.
- **input-field (“Search”):** transparent fill, #000000 text, 16px/400, 8px radius, padding 4px 4px 4px 32px, border 1px solid #868789.
- **link:** transparent fill, #C2C4C7 text, padding 0px.

## Do's and Don'ts

- Do use #001319 for the page and lift surfaces in small steps: #121417, #25272B.
- Do keep text in 4 levels: #868789, #FFFFFF, #9EA0A5, #56575A.
- Do let contrast carry emphasis; primary actions use #25272B on #001319.
- Do set headlines in Inter with tight tracking (-0.025em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on cards and controls.
- Don't use #56575A for body text; it reaches 2.6:1 on #001319. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter and Menlo.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.2s, 0.5s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.
