---
version: alpha
name: Attio
description: "Light monochrome interface measured from attio.com: interDisplay type with inter, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1C1D1F"
  on-background: "#1C1D1F"
  on-surface-variant: "#232529"
  on-surface-muted: "#242629"
  on-surface-subtle: "#505967"
  surface-container-low: "#FAFAFB"
  surface-container: "#F4F5F6"
  surface-container-high: "#DDF9E4"
  surface-container-highest: "#F5EEFF"
  outline: "#E4E7EC"
  outline-variant: "#0000000D"
  primary: "#202124"
  on-primary: "#F3F4F6"
  inverse-surface: "#101010"
  secondary: "#407FF2"
  tertiary: "#B8D0FF"
  success: "#075A39"
  error: "#FF5B59"
  warning: "#F5B900"
typography:
  headline-display:
    fontFamily: interDisplay
    fontSize: 64px
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: interDisplay
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
  headline-md:
    fontFamily: interDisplay
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: interDisplay
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -0.01em
  body-md:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
    letterSpacing: -0.005em
  body-lg:
    fontFamily: inter
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.22
    letterSpacing: -0.01em
  body-sm:
    fontFamily: inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.38
    letterSpacing: -0.01em
  label-md:
    fontFamily: inter
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.44
    letterSpacing: -0.01em
  label-sm:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
    letterSpacing: -0.01em
  code:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.016em
  headline-display-mobile:
    fontFamily: interDisplay
    fontSize: 40px
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: interDisplay
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.13
    letterSpacing: -0.01em
rounded:
  sm: 4.8px
  md: 8px
  lg: 10px
spacing:
  xs: 4px
  sm: 5px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 0px 12px
    height: 36px
  button-primary-hover:
    textColor: "{colors.background}"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#A4ADBA"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px 24px
    height: 96px
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "#2E3238"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 0px 12px
    height: 36px
  link:
    textColor: "#B5BDC9"
---

# Attio Design System

## Overview

Attio describes itself as: “The system for revenue teams to build pipeline, accelerate deals, and grow accounts around the clock.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1C1D1F)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **interDisplay** and **inter**, with **JetBrains Mono** for code. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 8px.

Measured from [attio.com](https://attio.com/) on October 29, 2026 at 1440×900 and 390×844 from 445 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 19 roles, plus gradient stops #D06785, #4283EB, #D6A07A, #A8623D.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`.
- **Charcoal (#1C1D1F):** Primary text and headings, seen 35 times. Token `on-surface`.
- **Cool Graphite (#232529):** Secondary text, seen 12 times. Token `on-surface-variant`.
- **Graphite (#242629):** Muted text and metadata, seen 21 times. Token `on-surface-muted`.
- **Dark Blue (#505967):** Subtle text and placeholders, seen 10 times. Token `on-surface-subtle`.
- **Snow (#FAFAFB):** Raised areas one step from the page, seen 11 times. Token `surface-container-low`.
- **Snow (#F4F5F6):** Cards and panels, seen 1 time. Token `surface-container`.
- **Pale Green (#DDF9E4):** Hover and pressed fills, seen 3 times. Token `surface-container-high`.
- **Cool Snow (#F5EEFF):** Highest raised elements, seen 4 times. Token `surface-container-highest`.
- **Cool Mist (#E4E7EC):** Borders and dividers, seen 20 times. Token `outline`.
- **Near Black 5% (#0000000D):** Secondary dividers, seen 8 times. Token `outline-variant`.
- **Charcoal (#202124):** Primary buttons and calls to action, seen 12 times. Token `primary`.
- **Snow (#F3F4F6):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#101010):** High-contrast fills, seen 8 times. Token `inverse-surface`.
- **Vivid Blue (#407FF2):** Accent in text, fills and borders, seen 6 times. Token `secondary`.
- **Pale Blue (#B8D0FF):** Accent in text, fills and borders, seen 6 times. Token `tertiary`.
- **Deep Teal (#075A39):** Success and positive states, seen 3 times. Token `success`.
- **Red (#FF5B59):** Errors and destructive states, seen 1 time. Token `error`.
- **Vivid Amber (#F5B900):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**interDisplay**, **inter** and **JetBrains Mono** (monospace) share the interface. Fallback stack: `interDisplay, interDisplay Fallback`. Other loaded fonts: tiemposText.

- **headline-display:** interDisplay 64px at weight 600, line height 0.95, tracking -0.02em (40px on mobile). Page title (h1).
- **headline-lg:** interDisplay 40px at weight 500, line height 1.1, tracking -0.01em (32px on mobile). Section headings (h2).
- **headline-md:** interDisplay 32px at weight 500, line height 1, tracking -0.01em. Sub-section headings.
- **headline-sm:** interDisplay 24px at weight 500, line height 1.15, tracking -0.01em. Card and feature titles.
- **body-md:** inter 14px at weight 400, line height 1.43, tracking -0.005em. Body text.
- **body-lg:** inter 18px at weight 500, line height 1.22, tracking -0.01em. Lead paragraphs.
- **body-sm:** inter 12px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** inter 16px at weight 500, line height 1.38, tracking -0.01em. Large buttons and tabs.
- **label-md:** inter 15px at weight 500, line height 1.44, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** inter 14px at weight 500, line height 1.43, tracking -0.01em. Small labels and badges.
- **code:** JetBrains Mono 10px at weight 500, line height 1.5, tracking -0.016em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 5px, md 12px, lg 24px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 360px, 375px, 480px, 576px, 640px, 768px, 992px, 1199px, 1200px, 1400px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FAFAFB → #F4F5F6 → #DDF9E4 → #F5EEFF) and #E4E7EC borders.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **md (8px):** 292 elements.
- **lg (10px):** 88 elements.
- **sm (4.8px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #202124 fill, #F3F4F6 text, 14px/500, 10px radius, padding 0px 12px, border 1px solid #505967.
- **button-primary-hover:** background #202124, text #FFFFFF on hover.
- **button-outline (“Read the Granola customer story”):** #FAFAFB fill, #A4ADBA text, 16px/500, padding 0px 24px.
- **button-ghost (“Sign in”):** #FFFFFF fill, #2E3238 text, 14px/500, 10px radius, padding 0px 12px, border 1px solid #CAD0D9.
- **link:** transparent fill, #B5BDC9 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAFAFB, #F4F5F6, #DDF9E4, #F5EEFF.
- Do keep text in 4 levels: #1C1D1F, #232529, #242629, #505967.
- Do let contrast carry emphasis; primary actions use #202124 on #FFFFFF.
- Do set headlines in interDisplay with tight tracking (-0.02em).
- Do reuse the measured spacing steps (5px, 12px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 10px and 4.8px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond interDisplay, inter and JetBrains Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.4s, 0.2s.

- **Easing:** `cubic-bezier(0, 0, 0, 1)`, `cubic-bezier(0.2, 0, 0, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/attio.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
