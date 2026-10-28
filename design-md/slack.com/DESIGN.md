---
version: alpha
name: Slack
description: "Light interface measured from slack.com: Salesforce-Avant-Garde type with Salesforce-Sans, dark purple accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#1D1D1D"
  on-surface-muted: "#444444"
  on-surface-subtle: "#747474"
  surface-container-low: "#FFFFFFE6"
  surface-container: "#F9F0FF"
  overlay: "#481A541F"
  overlay-strong: "#00000080"
  outline: "#F3F3F3"
  outline-variant: "#C9C9C9"
  primary: "#730394"
  on-primary: "#FFFFFF"
  secondary: "#481A54"
  tertiary: "#0000EE"
typography:
  headline-display:
    fontFamily: Salesforce-Avant-Garde
    fontSize: 64px
    fontWeight: 700
    lineHeight: 1.06
    letterSpacing: -0.012em
  headline-lg:
    fontFamily: Salesforce-Avant-Garde
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.012em
  headline-md:
    fontFamily: Salesforce-Avant-Garde
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.004em
  body-md:
    fontFamily: Salesforce-Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: -0.001em
  body-sm:
    fontFamily: Salesforce-Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: -0.002em
  caption:
    fontFamily: Salesforce-Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: -0.001em
  label-lg:
    fontFamily: Salesforce-Sans
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
  label-md:
    fontFamily: Salesforce-Sans
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.55
    letterSpacing: -0.001em
  label-sm:
    fontFamily: Salesforce-Sans
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.29
    letterSpacing: 0.057em
  headline-display-mobile:
    fontFamily: Salesforce-Avant-Garde
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.12
    letterSpacing: -0.012em
  headline-lg-mobile:
    fontFamily: Salesforce-Sans
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: -0.008em
  headline-md-mobile:
    fontFamily: Salesforce-Avant-Garde
    fontSize: 22.5px
    fontWeight: 700
    lineHeight: 1.34
    letterSpacing: -0.004em
rounded:
  sm: 4px
  md: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 24px
  xl: 40px
  gutter: 8px
  section: 72px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 12px 16px
    height: 42px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "#181818"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 0px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 0px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.tertiary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "#5C5C5C"
---

# Slack Design System

## Overview

Slack describes itself as: “Boost productivity and save time with Slack‌ – ‌the AI work platform for managing projects, automating workflows and connecting teams securely. Start working smarter today.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Dark Purple (#730394)** as the main accent.

Type is set in **Salesforce-Avant-Garde** and **Salesforce-Sans**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [slack.com](https://slack.com/intl/en-in/) on October 21, 2026 at 1440×900 and 390×844 from 339 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 21 times. Token `background`, CSS `--article-theme-secondary`.
- **Near Black (#000000):** Primary text and headings, seen 38 times. Token `on-surface`, CSS `--attachment-color`.
- **Charcoal (#1D1D1D):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Graphite (#444444):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **Slate (#747474):** Subtle text and placeholders, seen 4 times. Token `on-surface-subtle`.
- **White 90% (#FFFFFFE6):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Snow (#F9F0FF):** Cards and panels, seen 13 times. Token `surface-container`.
- **Deep Purple 12% (#481A541F):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Near Black 50% (#00000080):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Mist (#F3F3F3):** Borders and dividers, seen 10 times. Token `outline`.
- **Silver (#C9C9C9):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Dark Purple (#730394):** Primary buttons and calls to action, seen 23 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Purple (#481A54):** Brand color on large areas, seen 57 times. Token `secondary`, CSS `--article-theme-primary`.
- **Vivid Indigo (#0000EE):** Most used accent color, seen 15 times. Token `tertiary`.

## Typography

**Salesforce-Avant-Garde** and **Salesforce-Sans** share the interface. Fallback stack: `Salesforce-Avant-Garde, system-ui, -apple-system, blinkmacsystemfont`.

- **headline-display:** Salesforce-Avant-Garde 64px at weight 700, line height 1.06, tracking -0.012em (32px on mobile). Page title (h1).
- **headline-lg:** Salesforce-Avant-Garde 32px at weight 700, line height 1.25, tracking -0.012em (14px on mobile). Section headings (h2).
- **headline-md:** Salesforce-Avant-Garde 24px at weight 700, line height 1.25, tracking -0.004em (22.5px on mobile). Sub-section headings.
- **body-md:** Salesforce-Sans 18px at weight 400, line height 1.55, tracking -0.001em. Body text.
- **body-sm:** Salesforce-Sans 14px at weight 400, line height 1.55, tracking -0.002em. Secondary and small text.
- **caption:** Salesforce-Sans 12px at weight 400, line height 1.55, tracking -0.001em. Captions and fine print.
- **label-lg:** Salesforce-Sans 16px at weight 700, line height 1.5. Large buttons and tabs.
- **label-md:** Salesforce-Sans 15px at weight 700, line height 1.55, tracking -0.001em. Buttons, navigation and labels.
- **label-sm:** Salesforce-Sans 14px at weight 700, line height 1.29, tracking 0.057em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 24px, xl 40px.
- **Sections:** 72px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#FFFFFFE6 → #F9F0FF):

- `rgb(115, 3, 148) 0px 0px 0px 1px inset`
- `rgb(255, 255, 255) 0px 0px 0px 1px inset`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0.1) 0px 0px 16px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (4px):** 84 elements.
- **md (16px):** 80 elements.
- **full (9999px):** 68 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“GET STARTED”):** #730394 fill, #FFFFFF text, 14px/700, 4px radius, padding 12px 16px.
- **button-primary-hover:** background #481A54, text #FFFFFF on hover.
- **button-outline (“Previous slide”):** #FFFFFF fill, #181818 text, 16px/400, 999px radius, padding 0px, border 1px solid #C9C9C9.
- **button-ghost (“Product”):** transparent fill, #000000 text, 15px/400, 4px radius, padding 0px.
- **card:** #FFFFFF fill, #0000EE text, 16px/400, 16px radius, padding 0px, border 1px solid #F3F3F3.
- **link:** transparent fill, #5C5C5C text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFE6, #F9F0FF.
- Do keep text in 4 levels: #000000, #1D1D1D, #444444, #747474.
- Do reserve #730394 for primary actions and key highlights.
- Do set headlines in Salesforce-Avant-Garde with tight tracking (-0.012em).
- Do reuse the measured spacing steps (8px, 10px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Salesforce-Avant-Garde and Salesforce-Sans.
- Don't use #730394 for large backgrounds or body text.
- Don't make interface transitions slower than 0.42s.

## Motion

Interface transitions are quick: 0.42s, 0.2s, 0.001s. Longer ambient animations run 0.65s, 1s.

- **Easing:** `cubic-bezier(0.165, 0.84, 0.44, 1)`, `ease`, `ease-in`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/slack.com/), the free DESIGN.md generator.
