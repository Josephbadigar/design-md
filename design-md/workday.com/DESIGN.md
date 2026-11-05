---
version: alpha
name: Workday
description: "Light interface measured from workday.com: Workday Body type, dark blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#F6F5F1"
  surface: "#F6F5F1"
  on-surface: "#525D6A"
  on-background: "#525D6A"
  surface-container-low: "#FFFFFF"
  overlay: "#FFFFFF1F"
  overlay-strong: "#00000014"
  primary: "#0F2E66"
  on-primary: "#FFFFFF"
  secondary: "#022043"
typography:
  headline-display:
    fontFamily: Workday Body
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.4
  body-md:
    fontFamily: Workday Body
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Workday Body
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.5
  label-md:
    fontFamily: Workday Body
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
rounded:
  md: 36px
  full: 9999px
spacing:
  base: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 36px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.full}"
    padding: 18px
    height: 72px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.full}"
    padding: 12px
    height: 48px
  button-outline-hover:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.full}"
    padding: 12px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.headline-display}"
    rounded: 0px
    padding: 0px
  card:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "{colors.on-primary}"
---

# Workday Design System

## Overview

Workday describes itself as: “Experience a new way to work with Sana and agentic AI from Workday.” The interface is light, built on **Mist (#F6F5F1)** with **Dark Blue (#525D6A)** text, and **Dark Blue (#0F2E66)** as the main accent.

Type is set in **Workday Body**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [workday.com](https://www.workday.com/) on November 4, 2026 at 1440×900 and 390×844 from 360 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 8 roles.

- **Mist (#F6F5F1):** Page background, seen 1 time. Token `background`.
- **Dark Blue (#525D6A):** Primary text and headings, seen 2 times. Token `on-surface`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`, CSS `--vp-bar-ink`.
- **White 12% (#FFFFFF1F):** Translucent fill for cards and controls, seen 6 times. Token `overlay`.
- **Near Black 8% (#00000014):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Dark Blue (#0F2E66):** Primary buttons and calls to action, seen 90 times. Token `primary`, CSS `--vp-panel-ink`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Blue (#022043):** Accent in text, fills and borders, seen 3 times. Token `secondary`.

## Typography

**Workday Body** carries the whole interface. Fallback stack: `Workday Body, Arial, Helvetica, sans-serif`. Other loaded fonts: Roboto Mono, Workday Headline.

- **headline-display:** Workday Body 20px at weight 400, line height 1.4. Page title (h1).
- **body-md:** Workday Body 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Workday Body 16px at weight 300, line height 1.5. Lead paragraphs.
- **label-md:** Workday Body 16px at weight 400, line height 1.5, uppercase. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** sm 8px, md 12px, lg 24px, xl 36px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 374.98px, 375px, 380px, 520px, 521px, 600px, 640px, 750px, 767.98px, 768px, 920px, 991.98px, 992px, 1119.98px, 1200px, 1920px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.24) 0px 2px 12px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 376 elements.
- **md (36px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Open AI Concierge”):** #0F2E66 fill, #FFFFFF text, 13.3333px/400, 9999px radius, padding 18px, border 1px solid #0F2E66, shadow `rgba(0, 0, 0, 0.24) 0px 2px 12px 0px`.
- **button-outline (“Request a Demo”):** #FFFFFF fill, #0F2E66 text, 16px/700, 9999px radius, padding 12px.
- **button-outline-hover:** background #022043, text #FFFFFF on hover.
- **button-ghost (“Agents”):** transparent fill, #FFFFFF text, 16px/700, 9999px radius, padding 12px.
- **input-field:** transparent fill, #525D6A text, 20px/400, padding 0px.
- **card:** #FFFFFF1F fill, #FFFFFF text, 16px/400, 36px radius, padding 0px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #F6F5F1 for the page and lift surfaces in small steps: #FFFFFF.
- Do reserve #0F2E66 for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 36px corners.
- Don't introduce new font families beyond Workday Body.
- Don't use #0F2E66 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.4s, 0.288s.

- **Easing:** `ease-out`, `ease-in-out`, `ease`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/workday.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
