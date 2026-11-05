---
version: alpha
name: Monarch
description: "Light interface measured from monarch.com: Copernicus type with ABC Oracle, vivid orange accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#F6F5F3"
  surface: "#F6F5F3"
  on-surface: "#22201D"
  on-background: "#22201D"
  on-surface-variant: "#777573"
  surface-container-low: "#EFECEA"
  surface-container: "#FFFFFF"
  outline: "#DCD9D6"
  primary: "#FF692D"
  on-primary: "#FEFCFB"
  secondary: "#F35B16"
  tertiary: "#FFBC0B"
typography:
  headline-display:
    fontFamily: Copernicus
    fontSize: 48px
    fontWeight: 350
    lineHeight: 1.2
    letterSpacing: -0.067em
  headline-lg:
    fontFamily: Copernicus
    fontSize: 40px
    fontWeight: 350
    lineHeight: 1.2
    letterSpacing: -0.06em
  headline-md:
    fontFamily: Copernicus
    fontSize: 32px
    fontWeight: 350
    lineHeight: 1.2
    letterSpacing: -0.05em
  body-md:
    fontFamily: ABC Oracle
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: ABC Oracle
    fontSize: 18px
    fontWeight: 350
    lineHeight: 1.4
    letterSpacing: -0.01em
  body-sm:
    fontFamily: ABC Oracle
    fontSize: 14px
    fontWeight: 100
    lineHeight: 1.43
  label-md:
    fontFamily: ABC Oracle
    fontSize: 14px
    fontWeight: 350
    lineHeight: 1.3
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: Copernicus
    fontSize: 32px
    fontWeight: 350
    lineHeight: 1.2
    letterSpacing: -0.1em
  headline-lg-mobile:
    fontFamily: Copernicus
    fontSize: 32px
    fontWeight: 350
    lineHeight: 1.2
    letterSpacing: -0.075em
  headline-md-mobile:
    fontFamily: Copernicus
    fontSize: 28px
    fontWeight: 350
    lineHeight: 1.2
    letterSpacing: -0.057em
rounded:
  md: 12px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 64px
  gutter: 16px
  section: 64px
  margin: 16px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 36px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 12px
  link:
    textColor: "{colors.on-surface}"
---

# Monarch Design System

## Overview

Monarch describes itself as: “Manage your money with Monarch. Track accounts, build budgets, monitor investments, plan goals, and get a clearer view of your finances in one app.” The interface is light, built on **Snow (#F6F5F3)** with **Charcoal (#22201D)** text, and **Vivid Orange (#FF692D)** as the main accent.

Type is set in **Copernicus** and **ABC Oracle**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [monarch.com](https://www.monarch.com/) on November 4, 2026 at 1440×900 and 390×844 from 323 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Snow (#F6F5F3):** Page background, seen 1 time. Token `background`.
- **Charcoal (#22201D):** Primary text and headings, seen 75 times. Token `on-surface`, CSS `--theme-none-foreground`.
- **Slate (#777573):** Secondary text, seen 9 times. Token `on-surface-variant`.
- **Mist (#EFECEA):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **White (#FFFFFF):** Cards and panels, seen 6 times. Token `surface-container`, CSS `--osano-button-background-color`.
- **Warm Silver (#DCD9D6):** Borders and dividers, seen 3 times. Token `outline`.
- **Vivid Orange (#FF692D):** Primary buttons and calls to action, seen 9 times. Token `primary`, CSS `--orange-9`.
- **Snow (#FEFCFB):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#F35B16):** Accent in text, fills and borders, seen 13 times. Token `secondary`.
- **Vivid Amber (#FFBC0B):** Accent, seen 22 times. Token `tertiary`.

## Typography

**Copernicus** and **ABC Oracle** share the interface. Fallback stack: `Copernicus, sans-serif`.

- **headline-display:** Copernicus 48px at weight 350, line height 1.2, tracking -0.067em (32px on mobile). Page title (h1).
- **headline-lg:** Copernicus 40px at weight 350, line height 1.2, tracking -0.06em (32px on mobile). Section headings (h2).
- **headline-md:** Copernicus 32px at weight 350, line height 1.2, tracking -0.05em (28px on mobile). Sub-section headings.
- **body-md:** ABC Oracle 16px at weight 400, line height 1.5. Body text.
- **body-lg:** ABC Oracle 18px at weight 350, line height 1.4, tracking -0.01em. Lead paragraphs.
- **body-sm:** ABC Oracle 14px at weight 100, line height 1.43. Secondary and small text.
- **label-md:** ABC Oracle 14px at weight 350, line height 1.3, tracking -0.01em. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 100% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 359px, 376px, 480px, 500px, 640px, 767px, 768px, 1024px, 1200px, 1280px, 1360px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(34, 32, 29, 0.05) 0px 1px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 64 elements.
- **md (12px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #FF692D fill, #FEFCFB text, 14px/350, 9999px radius, padding 0px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(34, 32, 29, 0.05) 0px 1px 2px 0px`.
- **button-primary-hover:** background #F35B16, text #FEFCFB on hover.
- **button-outline (“Sign in”):** #FFFFFF fill, #22201D text, 14px/100, 9999px radius, padding 0px 16px, border 1px solid #DCD9D6, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(34, 32, 29, 0.05) 0px 1px 2px 0px`.
- **button-ghost (“Features”):** transparent fill, #22201D text, 14px/350, 9999px radius, padding 8px 12px.
- **link:** transparent fill, #22201D text, padding 0px.

## Do's and Don'ts

- Do use #F6F5F3 for the page and lift surfaces in small steps: #EFECEA, #FFFFFF.
- Do keep text in 2 levels: #22201D, #777573.
- Do reserve #FF692D for primary actions and key highlights.
- Do set headlines in Copernicus with tight tracking (-0.067em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 12px corners.
- Don't use #777573 for body text; it reaches 4.21:1 on #F6F5F3. Keep it for large text or metadata.
- Don't introduce new font families beyond Copernicus and ABC Oracle.
- Don't use #FF692D for large backgrounds or body text.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.15s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/monarch.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
