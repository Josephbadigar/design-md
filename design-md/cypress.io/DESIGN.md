---
version: alpha
name: Cypress
description: "Light interface measured from cypress.io: Poppins type with Roboto, dark cyan accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#5A5F7A"
  on-background: "#5A5F7A"
  on-surface-strong: "#1B1E2E"
  on-surface-variant: "#003131"
  on-surface-muted: "#9095AD"
  overlay: "#C8A7F540"
  overlay-strong: "#C8A7F580"
  outline: "#E1E3ED"
  outline-variant: "#69D3A7"
  primary: "#007780"
  on-primary: "#FFFFFF"
  secondary: "#4956E3"
  tertiary: "#00595D"
  success: "#69D3A7"
typography:
  headline-display:
    fontFamily: Poppins
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.5
  headline-lg:
    fontFamily: Poppins
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.38
  body-md:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Roboto
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.56
  body-sm:
    fontFamily: Poppins
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-md:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Roboto
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
  code:
    fontFamily: Roboto Mono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Poppins
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.5
rounded:
  md: 4px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 72px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 4px 12px 4px 16px
    height: 32px
  button-primary-hover:
    backgroundColor: "{colors.tertiary}"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px
    height: 64px
  button-outline:
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 11px 20px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px 0px 0px 12px
  input-field:
    textColor: "#2E3247"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px 44px 0px 0px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 24px
  link:
    textColor: "{colors.tertiary}"
---

# Cypress Design System

## Overview

Cypress describes itself as: “Your AI writes the code. Cypress proves it works: end-to-end tests in a real browser, failures you can rewind, and coverage and accessibility on every run.” The interface is light, built on **White (#FFFFFF)** with **Indigo (#5A5F7A)** text, and **Dark Cyan (#007780)** as the main accent.

Type is set in **Poppins** and **Roboto**, with **Roboto Mono** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [cypress.io](https://www.cypress.io/#create) on November 4, 2026 at 1440×900 and 390×844 from 437 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #4956E3, #7F43C9, #00814D.

- **White (#FFFFFF):** Page background, seen 37 times. Token `background`, CSS `--osano-button-reject-all-foreground-color`.
- **Indigo (#5A5F7A):** Primary text and headings, seen 78 times. Token `on-surface`.
- **Deep Indigo (#1B1E2E):** Headings and emphasis, seen 10 times. Token `on-surface-strong`.
- **Deep Cyan (#003131):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Indigo (#9095AD):** Muted text and metadata, seen 16 times. Token `on-surface-muted`.
- **Light Violet 25% (#C8A7F540):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Light Violet 50% (#C8A7F580):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Cool Mist (#E1E3ED):** Borders and dividers, seen 28 times. Token `outline`.
- **Teal (#69D3A7):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Dark Cyan (#007780):** Primary buttons and calls to action, seen 18 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Indigo (#4956E3):** Secondary buttons, seen 20 times. Token `secondary`, CSS `--cy-indigo-500`.
- **Deep Cyan (#00595D):** Links and interactive text, seen 16 times. Token `tertiary`, CSS `--cy-teal-600`.
- **Teal (#69D3A7):** Success and positive states, seen 13 times. Token `success`.

## Typography

**Poppins**, **Roboto** and **Roboto Mono** (monospace) share the interface. Fallback stack: `Poppins, -apple-system, BlinkMacSystemFont, Segoe UI`.

- **headline-display:** Poppins 48px at weight 700, line height 1.5 (32px on mobile). Page title (h1).
- **headline-lg:** Poppins 40px at weight 700, line height 1.38. Section headings (h2).
- **body-md:** Roboto 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Roboto 18px at weight 400, line height 1.56. Lead paragraphs.
- **body-sm:** Poppins 14px at weight 400, line height 1.43. Secondary and small text.
- **label-md:** Roboto 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Roboto 14px at weight 500, line height 1.5. Small labels and badges.
- **code:** Roboto Mono 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 72px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 376px, 768px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.06) 0px 2px 12px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.06) 0px 2px 12px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (4px):** 140 elements.
- **full (9999px):** 36 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #007780 fill, #FFFFFF text, 16px/500, 9999px radius, padding 4px 12px 4px 16px.
- **button-primary-hover:** background #00595D, text #FFFFFF on hover.
- **button-secondary (“Open Support Assistant”):** #4956E3 fill, #FFFFFF text, 16px/500, 9999px radius, padding 0px, border 1px solid #4956E3.
- **button-outline (“Book a demo”):** transparent fill, #007780 text, 16px/500, 4px radius, padding 11px 20px, border 1px solid #007780.
- **button-ghost (“Contact sales”):** transparent fill, #5A5F7A text, 16px/500, padding 0px 0px 0px 12px.
- **input-field (“Install command”):** transparent fill, #2E3247 text, 16px/400, padding 0px 44px 0px 0px.
- **card:** #FFFFFF fill, #1B1E2E text, 16px/400, 4px radius, padding 24px, border 1px solid #E1E3ED, shadow `rgba(0, 0, 0, 0.06) 0px 2px 12px 0px`.
- **link:** transparent fill, #00595D text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 4 levels: #5A5F7A, #1B1E2E, #003131, #9095AD.
- Do reserve #007780 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't use #9095AD for body text; it reaches 2.96:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Poppins, Roboto and Roboto Mono.
- Don't use #007780 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s. Longer ambient animations run 4s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cypress.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
