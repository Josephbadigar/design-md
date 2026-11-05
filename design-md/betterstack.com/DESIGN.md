---
version: alpha
name: Better Stack
description: "Dark interface measured from betterstack.com: Helvetica Now Display type with Helvetica Now Text, indigo accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#0B0C14"
  surface: "#0B0C14"
  on-surface: "#939DB8"
  on-background: "#939DB8"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#C9D3EE"
  on-surface-muted: "#646E87"
  surface-container-low: "#0F101A"
  surface-container: "#171926"
  overlay: "#727DA11A"
  overlay-strong: "#0B0C14CC"
  outline: "#939DB81A"
  outline-variant: "#939DB833"
  primary: "#5B63D3"
  on-primary: "#FFFFFF"
  secondary: "#E9C899"
  tertiary: "#64C28D"
  link: "#98A4F7"
typography:
  headline-display:
    fontFamily: Helvetica Now Display
    fontSize: 53px
    fontWeight: 500
    lineHeight: 1.1
  headline-lg:
    fontFamily: Helvetica Now Display
    fontSize: 40px
    fontWeight: 700
    lineHeight: 0.6
  headline-md:
    fontFamily: Helvetica Now Text
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1.17
  body-md:
    fontFamily: Helvetica Now Text
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
  body-sm:
    fontFamily: Helvetica Now Text
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.6
  caption:
    fontFamily: Helvetica Now Text
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Helvetica Now Text
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Helvetica Now Display
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: Helvetica Now Display
    fontSize: 28px
    fontWeight: 700
    lineHeight: 0.86
rounded:
  md: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 60px
  container: 1100px
components:
  button-primary:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: 8px
    padding: 0px 8px
    height: 27px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: 43px
    padding: 0px 12px
    height: 37px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: 0px
    padding: 12px 24px 12px 12px
  input-field:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: 12px
    padding: 0px 20px
  link:
    textColor: "{colors.link}"
---

# Better Stack Design System

## Overview

Better Stack describes itself as: “AI SRE and MCP server, incident management, on-call, logs, metrics, traces, and error tracking. 7,000+ happy customers. 60-day money back guarantee.” The interface is dark, built on **Cool Charcoal (#0B0C14)** with **Blue (#939DB8)** text, and **Indigo (#5B63D3)** as the main accent.

Type is set in **Helvetica Now Display** and **Helvetica Now Text**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [betterstack.com](https://betterstack.com/) on November 4, 2026 at 1440×900 and 390×844 from 323 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles, plus gradient stops #939DB8, #5B63D3, #7C87F7.

- **Cool Charcoal (#0B0C14):** Page background, seen 3 times. Token `background`.
- **Blue (#939DB8):** Primary text and headings, seen 24 times. Token `on-surface`, CSS `--color-neutral-200`.
- **White (#FFFFFF):** Headings and emphasis, seen 66 times. Token `on-surface-strong`, CSS `--tw-ring-offset-color`.
- **Pale Blue (#C9D3EE):** Secondary text, seen 14 times. Token `on-surface-variant`.
- **Blue (#646E87):** Muted text and metadata, seen 47 times. Token `on-surface-muted`, CSS `--color-neutral-300`.
- **Cool Charcoal (#0F101A):** Raised areas one step from the page, seen 37 times. Token `surface-container-low`.
- **Cool Charcoal (#171926):** Cards and panels, seen 27 times. Token `surface-container`.
- **Blue 10% (#727DA11A):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Cool Charcoal 80% (#0B0C14CC):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Blue 10% (#939DB81A):** Borders and dividers, seen 37 times. Token `outline`.
- **Blue 20% (#939DB833):** Secondary dividers, seen 27 times. Token `outline-variant`.
- **Indigo (#5B63D3):** Brand accent (CSS variable), seen 2 times. Token `primary`, CSS `--color-brand-primary-200`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Orange (#E9C899):** Accent (CSS variable). Token `secondary`.
- **Green (#64C28D):** Accent (CSS variable). Token `tertiary`.
- **Light Indigo (#98A4F7):** Inline links, seen 10 times. Token `link`.

## Typography

**Helvetica Now Display** and **Helvetica Now Text** share the interface. Fallback stack: `Helvetica Now Display, Helvetica Now Display Extended, ui-sans-serif, system-ui`.

- **headline-display:** Helvetica Now Display 53px at weight 500, line height 1.1 (40px on mobile). Page title (h1).
- **headline-lg:** Helvetica Now Display 40px at weight 700, line height 0.6 (28px on mobile). Section headings (h2).
- **headline-md:** Helvetica Now Text 28px at weight 700, line height 1.17. Sub-section headings.
- **body-md:** Helvetica Now Text 14px at weight 400, line height 1.55. Body text.
- **body-sm:** Helvetica Now Text 13px at weight 400, line height 1.6. Secondary and small text.
- **caption:** Helvetica Now Text 12px at weight 400, line height 1.5. Captions and fine print.
- **label-md:** Helvetica Now Text 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 60px.
- **Container:** content is capped at 1100px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#0F101A → #171926) and hairline rings:

- `rgba(255, 255, 255, 0.25) 0px 1px 3px 0px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (16px):** 148 elements.
- **full (9999px):** 104 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** transparent fill, #FFFFFF text, 13px/500, 8px radius, padding 0px 8px, border 1px solid #FFFFFF1C, shadow `rgba(255, 255, 255, 0.25) 0px 1px 3px 0px inset`.
- **button-outline (“Explore pricing”):** #171926 fill, #C9D3EE text, 13px/400, 43px radius, padding 0px 12px, border 1px solid #939DB833.
- **button-ghost (“Platform”):** transparent fill, #C9D3EE text, 13px/400, padding 12px 24px 12px 12px.
- **input-field (“Your work e-mail”):** transparent fill, #FFFFFF text, 16px/400, 12px radius, padding 0px 20px.
- **link:** transparent fill, #98A4F7 text, padding 0px.

## Do's and Don'ts

- Do use #0B0C14 for the page and lift surfaces in small steps: #0F101A, #171926.
- Do keep text in 4 levels: #939DB8, #FFFFFF, #C9D3EE, #646E87.
- Do use #5B63D3 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 16px corners.
- Don't use #646E87 for body text; it reaches 3.83:1 on #0B0C14. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Helvetica Now Display and Helvetica Now Text.
- Don't use #5B63D3 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.15s, 0.4s. Longer ambient animations run 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/betterstack.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
