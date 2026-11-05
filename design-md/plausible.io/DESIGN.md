---
version: alpha
name: Plausible
description: "Light interface measured from plausible.io: system-ui type, vivid indigo accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#F9FAFB"
  surface: "#F9FAFB"
  on-surface: "#4B5563"
  on-background: "#4B5563"
  on-surface-strong: "#161E2E"
  on-surface-variant: "#6B7280"
  on-surface-muted: "#9FA6B2"
  surface-container-low: "#FFFFFF"
  surface-container: "#EEF1F6"
  outline: "#FACA15"
  outline-variant: "#E5E7EB"
  primary: "#5850EC"
  on-primary: "#FFFFFF"
  inverse-surface: "#252F3F"
  secondary: "#3182CE"
  tertiary: "#0E9F6E"
typography:
  headline-display:
    fontFamily: system-ui
    fontSize: 48px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: system-ui
    fontSize: 36px
    fontWeight: 800
    lineHeight: 1.5
  headline-md:
    fontFamily: system-ui
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.5
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: system-ui
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.78
  body-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: system-ui
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: system-ui
    fontSize: 30px
    fontWeight: 800
    lineHeight: 1.2
rounded:
  sm: 3px
  md: 6px
  lg: 8px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px 20px
    height: 42px
  button-primary-hover:
    backgroundColor: "#6875F5"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.md}"
    padding: 16px 40px
    height: 58px
  button-outline-hover:
    textColor: "#6875F5"
  input-field:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.inverse-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px
  link:
    textColor: "#D2D6DC"
---

# Plausible Design System

## Overview

Plausible describes itself as: “Plausible is a lightweight and open-source Google Analytics alternative. Your website data is 100% yours and the privacy of your visitors is respected.” The interface is light, built on **Snow (#F9FAFB)** with **Dark Blue (#4B5563)** text, and **Vivid Indigo (#5850EC)** as the main accent.

Type is set in **system-ui**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [plausible.io](https://plausible.io/) on November 4, 2026 at 1440×900 and 390×844 from 321 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Snow (#F9FAFB):** Page background, seen 1 time. Token `background`.
- **Dark Blue (#4B5563):** Primary text and headings, seen 41 times. Token `on-surface`.
- **Deep Blue (#161E2E):** Headings and emphasis, seen 13 times. Token `on-surface-strong`.
- **Cool Slate (#6B7280):** Secondary text, seen 16 times. Token `on-surface-variant`.
- **Blue (#9FA6B2):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **Cool Mist (#EEF1F6):** Cards and panels, seen 1 time. Token `surface-container`.
- **Vivid Amber (#FACA15):** Borders and dividers, seen 1 time. Token `outline`.
- **Cool Mist (#E5E7EB):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Indigo (#5850EC):** Primary buttons and calls to action, seen 45 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Blue (#252F3F):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Blue (#3182CE):** Accent in text, fills and borders, seen 7 times. Token `secondary`.
- **Dark Teal (#0E9F6E):** Accent, seen 8 times. Token `tertiary`.

## Typography

**system-ui** carries the whole interface. Fallback stack: `system-ui, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** system-ui 48px at weight 800, line height 1, tracking -0.025em (30px on mobile). Page title (h1).
- **headline-lg:** system-ui 36px at weight 800, line height 1.5. Section headings (h2).
- **headline-md:** system-ui 24px at weight 600, line height 1.5. Sub-section headings.
- **body-md:** system-ui 16px at weight 400, line height 1.5. Body text.
- **body-lg:** system-ui 18px at weight 400, line height 1.78. Lead paragraphs.
- **body-sm:** system-ui 14px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** system-ui 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** system-ui 14px at weight 600, line height 1.43. Small labels and badges.

## Layout

Spacing follows a 4px grid: 95% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 40px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 768px, 1024px, 1280px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (6px):** 36 elements.
- **full (9999px):** 16 elements.
- **sm (3px):** 4 elements.
- **lg (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start free trial”):** #5850EC fill, #FFFFFF text, 16px/500, 6px radius, padding 8px 20px.
- **button-primary-hover:** background #6875F5, text #FFFFFF on hover.
- **button-outline (“View live demo”):** #FFFFFF fill, #5850EC text, 18px/500, 6px radius, padding 16px 40px.
- **button-outline-hover:** background #FFFFFF, text #6875F5 on hover.
- **input-field:** #EEF1F6 fill, #252F3F text, 16px/400, 3px radius, padding 0px, shadow `rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`.
- **link:** transparent fill, #D2D6DC text, padding 0px.

## Do's and Don'ts

- Do use #F9FAFB for the page and lift surfaces in small steps: #FFFFFF, #EEF1F6.
- Do keep text in 4 levels: #4B5563, #161E2E, #6B7280, #9FA6B2.
- Do reserve #5850EC for primary actions and key highlights.
- Do set headlines in system-ui with tight tracking (-0.025em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 6px corners.
- Don't use #9FA6B2 for body text; it reaches 2.34:1 on #F9FAFB. Keep it for large text or metadata.
- Don't introduce new font families beyond system-ui.
- Don't use #5850EC for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/plausible.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
