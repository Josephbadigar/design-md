---
version: alpha
name: Suno
description: "Dark interface measured from suno.com: Neue Montreal type with Editorial New, vivid green accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#101012"
  surface: "#101012"
  on-surface: "#F7F4EF"
  on-background: "#F7F4EF"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#FCFBF9"
  on-surface-muted: "#C2C2C1"
  surface-container-low: "#000000"
  overlay: "#FFFFFF0A"
  overlay-strong: "#FFFFFF33"
  outline: "#FFFFFF04"
  outline-variant: "#FFFFFF26"
  primary: "#02D95C"
  on-primary: "#000000"
  secondary: "#1F8BFF"
typography:
  headline-display:
    fontFamily: Neue Montreal
    fontSize: 72px
    fontWeight: 500
    lineHeight: 0.89
  headline-lg:
    fontFamily: Editorial New
    fontSize: 24px
    fontWeight: 300
    lineHeight: 1.5
  body-md:
    fontFamily: Neue Montreal
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Neue Montreal
    fontSize: 17px
    fontWeight: 500
    lineHeight: 1.41
  body-sm:
    fontFamily: Neue Montreal
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Neue Montreal
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Neue Montreal
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.6
  label-sm:
    fontFamily: Neue Montreal
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Neue Montreal
    fontSize: 48px
    fontWeight: 500
    lineHeight: 0.92
    letterSpacing: -0.02em
rounded:
  sm: 4px
  md: 12px
  full: 9999px
spacing:
  xs: 3px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 8px
  section: 100px
  margin: 20px
  container: 800px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 40px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    padding: 6px 12px
  input-field:
    textColor: "{colors.on-surface-strong}"
    rounded: "{rounded.md}"
    padding: 0px 4px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Suno Design System

## Overview

Suno describes itself as: “Create stunning original music for free in seconds using our AI generator. Make your own masterpieces, share with friends, and discover music from artists worldwide.” The interface is dark, built on **Charcoal (#101012)** with **Warm Mist (#F7F4EF)** text, and **Vivid Green (#02D95C)** as the main accent.

Type is set in **Neue Montreal** and **Editorial New**. Headlines run large; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [suno.com](https://suno.com/) on October 29, 2026 at 1440×900 and 390×844 from 349 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Charcoal (#101012):** Page background, seen 6 times. Token `background`.
- **Warm Mist (#F7F4EF):** Primary text and headings, seen 29 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 5 times. Token `on-surface-strong`, CSS `--color-white`.
- **Snow (#FCFBF9):** Secondary text, seen 5 times. Token `on-surface-variant`, CSS `--color-foreground-button-secondary`.
- **Silver (#C2C2C1):** Muted text and metadata, seen 23 times. Token `on-surface-muted`.
- **Near Black (#000000):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`, CSS `--tw-mask-bottom-from-color`.
- **White 4% (#FFFFFF0A):** Translucent fill for cards and controls, seen 19 times. Token `overlay`.
- **White 20% (#FFFFFF33):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 2% (#FFFFFF04):** Borders and dividers, seen 19 times. Token `outline`.
- **White 15% (#FFFFFF26):** Secondary dividers, seen 5 times. Token `outline-variant`, CSS `--color-opacity-white-15`.
- **Vivid Green (#02D95C):** Brand accent (CSS variable), seen 30 times. Token `primary`, CSS `--color-accent-green`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#1F8BFF):** Accent (CSS variable). Token `secondary`.

## Typography

**Neue Montreal** and **Editorial New** share the interface. Fallback stack: `Neue Montreal, ui-sans-serif, system-ui, sans-serif`.

- **headline-display:** Neue Montreal 72px at weight 500, line height 0.89 (48px on mobile). Page title (h1).
- **headline-lg:** Editorial New 24px at weight 300, line height 1.5. Section headings (h2).
- **body-md:** Neue Montreal 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Neue Montreal 17px at weight 500, line height 1.41. Lead paragraphs.
- **body-sm:** Neue Montreal 12px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** Neue Montreal 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Neue Montreal 15px at weight 500, line height 1.6. Buttons, navigation and labels.
- **label-sm:** Neue Montreal 14px at weight 500, line height 1.5. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (82% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 3px, sm 8px, md 16px, lg 24px, xl 40px.
- **Sections:** 100px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 800px.
- **Page margin:** 20px on each side of full-width sections.
- **Breakpoints:** 820px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#000000) and #FFFFFF04 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 68 elements.
- **md (12px):** 12 elements.
- **sm (4px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Join Suno for free”):** #F7F4EF fill, #101012 text, 15px/500, 9999.01px radius, padding 8px 16px.
- **button-outline (“Create”):** #000000 fill, #FFFFFF text, 15px/500, 9999.01px radius, padding 8px 16px.
- **button-ghost (“Products”):** transparent fill, #F7F4EF text, 15px/500, 3.35544e+07px radius, padding 6px 12px.
- **input-field (“Chat to make music”):** transparent fill, #FFFFFF text, 18px/400, 12px radius, padding 0px 4px.
- **link:** transparent fill, #C2C2C1 text, padding 0px.

## Do's and Don'ts

- Do use #101012 for the page and lift surfaces in small steps: #000000.
- Do keep text in 4 levels: #F7F4EF, #FFFFFF, #FCFBF9, #C2C2C1.
- Do use #02D95C as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 12px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Neue Montreal and Editorial New.
- Don't use #02D95C for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.075s, 0.3s, 0.2s. Longer ambient animations run 3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/suno.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
