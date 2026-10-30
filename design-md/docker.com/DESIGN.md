---
version: alpha
name: Docker
description: "Light interface measured from docker.com: Repro type with Inter, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#F9FAFB"
  surface: "#F9FAFB"
  on-surface: "#2C333F"
  on-background: "#2C333F"
  on-surface-strong: "#000000"
  on-surface-variant: "#8A93AB"
  on-surface-muted: "#94A3B8"
  surface-container-low: "#FFFFFF"
  surface-container: "#D6DCE6"
  overlay: "#FFFFFF1F"
  outline: "#A9B4C6"
  outline-variant: "#E7EAEF"
  primary: "#2560FF"
  on-primary: "#FFFFFF"
  secondary: "#00084D"
  tertiary: "#1D63ED"
  success: "#34D399"
  error: "#EF4444"
typography:
  headline-display:
    fontFamily: Repro
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Repro
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Inter
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.012em
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.013em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: ABC Repro
    fontSize: 19px
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: -0.012em
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.011em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: -0.012em
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: -0.011em
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: -0.012em
  code:
    fontFamily: ui-monospace
    fontSize: 12.5px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Repro
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.03em
rounded:
  sm: 2px
  md: 4px
  lg: 8px
  xl: 18px
  full: 9999px
spacing:
  xs: 3.5px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 36px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 36px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 12px
    height: 36px
  button-secondary:
    backgroundColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 6px 0px 6px 10px
    height: 38px
  card:
    backgroundColor: "{colors.background}"
    textColor: "#0B1220"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 28px 28px 0px 28px
  link:
    textColor: "{colors.on-surface}"
---

# Docker Design System

## Overview

Docker describes itself as: “Run AI agents and containers safely, anywhere. Docker gives builders trusted sandboxes, governance, and a secure supply chain for modern software.” The interface is light, built on **Snow (#F9FAFB)** with **Deep Blue (#2C333F)** text, and **Vivid Blue (#2560FF)** as the main accent.

Type is set in **Repro** and **Inter**, with **ui-monospace** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [docker.com](https://www.docker.com/) on October 29, 2026 at 1440×900 and 390×844 from 379 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #283045.

- **Snow (#F9FAFB):** Page background, seen 7 times. Token `background`, CSS `--backgroundColor`.
- **Deep Blue (#2C333F):** Primary text and headings, seen 58 times. Token `on-surface`, CSS `--labelColor`.
- **Near Black (#000000):** Headings and emphasis, seen 29 times. Token `on-surface-strong`, CSS `--menuLinkLabelColor`.
- **Blue (#8A93AB):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Blue (#94A3B8):** Muted text and metadata, seen 7 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 12 times. Token `surface-container-low`, CSS `--buttonPrimaryText`.
- **Cool Silver (#D6DCE6):** Cards and panels, seen 2 times. Token `surface-container`.
- **White 12% (#FFFFFF1F):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Light Blue (#A9B4C6):** Borders and dividers, seen 6 times. Token `outline`.
- **Cool Mist (#E7EAEF):** Secondary dividers, seen 4 times. Token `outline-variant`, CSS `--codeBoxBackgroundColor`.
- **Vivid Blue (#2560FF):** Primary buttons and calls to action, seen 12 times. Token `primary`, CSS `--menuLinkButtonColor`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Indigo (#00084D):** Accent in the header, seen 4 times. Token `secondary`.
- **Vivid Blue (#1D63ED):** Accent in text, fills and borders, seen 6 times. Token `tertiary`.
- **Teal (#34D399):** Success and positive states, seen 8 times. Token `success`.
- **Vivid Red (#EF4444):** Errors and destructive states, seen 2 times. Token `error`.

## Typography

**Repro**, **Inter**, **ABC Repro** and **ui-monospace** (monospace) share the interface. Fallback stack: `Repro, Helvetica, Arial, sans-serif`.

- **headline-display:** Repro 64px at weight 500, line height 1.05, tracking -0.03em (36px on mobile). Page title (h1).
- **headline-lg:** Repro 60px at weight 500, line height 1, tracking -0.025em. Section headings (h2).
- **headline-md:** Inter 22px at weight 500, line height 1.25, tracking -0.012em. Sub-section headings.
- **headline-sm:** Inter 20px at weight 500, line height 1.5, tracking -0.013em. Card and feature titles.
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** ABC Repro 19px at weight 600, line height 1.3, tracking -0.012em. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1, tracking -0.011em. Secondary and small text.
- **caption:** Inter 12px at weight 400, line height 1.3, tracking -0.012em. Captions and fine print.
- **label-lg:** Inter 14px at weight 500, line height 1.3, tracking -0.011em. Large buttons and tabs.
- **label-md:** Inter 13px at weight 600, line height 1.2, tracking 0.01em. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.3, tracking -0.012em. Small labels and badges.
- **code:** ui-monospace 12.5px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (79% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 3.5px, sm 8px, md 12px, lg 20px, xl 36px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 425px, 426px, 500px, 550px, 767px, 768px, 769px, 896px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(15, 23, 42, 0.03) 0px 1px 2px 0px`

Hairline rings and inset highlights also appear: `rgb(67, 76, 95) 0px 0px 1px 1px inset`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 52 elements.
- **lg (8px):** 28 elements.
- **xl (18px):** 28 elements.
- **sm (2px):** 24 elements.
- **md (4px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Contact Sales”):** #2560FF fill, #FFFFFF text, 14px/500, 4px radius, padding 8px 12px, border 1px solid #003DB5, shadow `rgb(192, 224, 250) 0px 0px 1px 1px inset`.
- **button-outline (“Sign In”):** #FFFFFF fill, #000000 text, 14px/500, 4px radius, padding 8px 12px, border 1px solid #A9B4C6, shadow `rgba(0, 0, 0, 0) 0px 0px 1px 1px inset`.
- **button-secondary (“Search”):** #000000 fill, #00000000 text, 16px/400, padding 6px 0px 6px 10px, border 1px solid #CCCCCC.
- **card:** #F9FAFB fill, #0B1220 text, 16px/400, padding 28px 28px 0px 28px.
- **link:** transparent fill, #2C333F text, padding 0px.

## Do's and Don'ts

- Do use #F9FAFB for the page and lift surfaces in small steps: #FFFFFF, #D6DCE6.
- Do keep text in 4 levels: #2C333F, #000000, #8A93AB, #94A3B8.
- Do reserve #2560FF for primary actions and key highlights.
- Do set headlines in Repro with tight tracking (-0.03em).
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 8px corners.
- Don't use #8A93AB for body text; it reaches 2.94:1 on #F9FAFB. Keep it for large text or metadata.
- Don't use #94A3B8 for body text; it reaches 2.45:1 on #F9FAFB. Keep it for large text or metadata.
- Don't introduce new font families beyond Repro, Inter, ABC Repro and ui-monospace.
- Don't use #2560FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.55s.

## Motion

Interface transitions are quick: 0.25s, 0.4s, 0.5s, 0.3s. Longer ambient animations run 1s, 1.1s, 1.4s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `ease-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/docker.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
