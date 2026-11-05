---
version: alpha
name: SoFi
description: "Light interface measured from sofi.com: Larsseit type with TT Norms, deep indigo accents, flat surfaces and 20px corners."
colors:
  background: "#00A2C7"
  surface: "#00A2C7"
  on-surface: "#1F1645"
  on-background: "#1F1645"
  on-surface-variant: "#1A1919"
  on-surface-muted: "#212121"
  on-surface-subtle: "#FFFFFF"
  outline: "#4087F1"
  outline-variant: "#0A0A0A1A"
  primary: "#1F1645"
  on-primary: "#FFFFFF"
  secondary: "#00819D"
  warning: "#FED881"
typography:
  headline-display:
    fontFamily: Larsseit
    fontSize: 50px
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: -0.028em
  headline-lg:
    fontFamily: Larsseit
    fontSize: 30px
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: -0.028em
  headline-md:
    fontFamily: TT Norms
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.5
  headline-sm:
    fontFamily: Larsseit
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.028em
  title-lg:
    fontFamily: TT Norms
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.11
  body-md:
    fontFamily: TT Norms
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: TT Norms
    fontSize: 12px
    fontWeight: 400
    lineHeight: 2
  label-lg:
    fontFamily: TT Norms
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.25
  label-md:
    fontFamily: Larsseit
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.71
    letterSpacing: -0.028em
  label-sm:
    fontFamily: TT Norms
    fontSize: 12px
    fontWeight: 700
  title-lg-mobile:
    fontFamily: TT Norms
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: 0.03em
  headline-display-mobile:
    fontFamily: Larsseit
    fontSize: 28px
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: -0.028em
rounded:
  sm: 12px
  md: 15px
  lg: 20px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 18px
  xl: 40px
  gutter: 12px
  section: 80px
  margin: 40px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.title-lg}"
    rounded: "{rounded.lg}"
    padding: 18px 38px
    height: 60px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-subtle}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 10px 20px
    height: 44px
  button-outline-hover:
    backgroundColor: "#0080A3"
  button-secondary:
    backgroundColor: "{colors.on-surface-subtle}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 6px 16px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 8px 16px
  input-field:
    backgroundColor: "{colors.on-surface-subtle}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px 20px
  link:
    textColor: "{colors.on-surface-variant}"
---

# SoFi Design System

## Overview

SoFi describes itself as: “Why do 17.1M members trust SoFi? Financial solutions for school, marriage, starting a family, home buying, retirement, or whatever’s next. Member FDIC.” The interface is light, built on **Cyan (#00A2C7)** with **Deep Indigo (#1F1645)** text, and **Deep Indigo (#1F1645)** as the main accent.

Type is set in **Larsseit** and **TT Norms**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 20px.

Measured from [sofi.com](https://www.sofi.com/) on November 4, 2026 at 1440×900 and 390×844 from 383 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles, plus gradient stops #00A2C7.

- **Cyan (#00A2C7):** Page background, seen 10 times. Token `background`.
- **Deep Indigo (#1F1645):** Primary text and headings, seen 57 times. Token `on-surface`.
- **Charcoal (#1A1919):** Secondary text, seen 52 times. Token `on-surface-variant`.
- **Charcoal (#212121):** Muted text and metadata, seen 11 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Subtle text and placeholders, seen 36 times. Token `on-surface-subtle`, CSS `--wp--preset--color--white`.
- **Vivid Blue (#4087F1):** Borders and dividers, seen 1 time. Token `outline`.
- **Near Black 10% (#0A0A0A1A):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Deep Indigo (#1F1645):** Primary buttons and calls to action, seen 85 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Cyan (#00819D):** Accent in text, fills and borders, seen 15 times. Token `secondary`.
- **Light Amber (#FED881):** Warnings and highlights, seen 4 times. Token `warning`.

## Typography

**Larsseit** and **TT Norms** share the interface. Fallback stack: `Larsseit, Helvetica, Arial, Lucida Grande`. Other loaded fonts: Material Symbols Outlined, superscript.

- **headline-display:** Larsseit 50px at weight 800, line height 1.2, tracking -0.028em (28px on mobile). Page title (h1).
- **headline-lg:** Larsseit 30px at weight 800, line height 1.2, tracking -0.028em. Section headings (h2).
- **headline-md:** TT Norms 24px at weight 400, line height 1.5. Sub-section headings.
- **headline-sm:** Larsseit 20px at weight 700, line height 1.2, tracking -0.028em. Card and feature titles.
- **title-lg:** TT Norms 18px at weight 700, line height 1.11, uppercase (12px on mobile). Small titles.
- **body-md:** TT Norms 16px at weight 400, line height 1.5. Body text.
- **body-sm:** TT Norms 12px at weight 400, line height 2. Secondary and small text.
- **label-lg:** TT Norms 16px at weight 500, line height 1.25. Large buttons and tabs.
- **label-md:** Larsseit 14px at weight 700, line height 1.71, tracking -0.028em. Buttons, navigation and labels.
- **label-sm:** TT Norms 12px at weight 700. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 60% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 18px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 400px, 425px, 426px, 550px, 767px, 768px, 896px, 991px, 992px, 1023px, 1024px, 1025px, 1320px, 1439px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(64, 135, 241, 0.3) 0px 2px 8px 0px`
- `rgba(20, 20, 20, 0.1) 0px 0px 1px 0px, rgba(20, 20, 20, 0.06) 0px 6px 12px -6px`
- `rgba(20, 20, 20, 0.1) 0px 0px 1.5px 0px, rgba(20, 20, 20, 0.06) 0px 7px 15px -7px`

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **lg (20px):** 64 elements.
- **sm (12px):** 50 elements.
- **md (15px):** 16 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #1F1645 fill, #FFFFFF text, 18px/700, 20px radius, padding 18px 38px, border 2px solid #1F1645.
- **button-outline (“Get Started”):** #00A2C7 fill, #FFFFFF text, 16px/700, 12px radius, padding 10px 20px.
- **button-outline-hover:** background #0080A3, text #FFFFFF on hover.
- **button-secondary (“Personal”):** #FFFFFF fill, #212121 text, 16px/700, 12px 12px 0px 0px radius, padding 6px 16px.
- **button-ghost (“Bank”):** transparent fill, #1A1919 text, 16px/500, 12px radius, padding 8px 16px.
- **input-field (“Enter your email”):** #FFFFFF fill, #1A1919 text, 16px/400, 20px radius, padding 0px 20px, border 1px solid #0A0A0A1A.
- **link:** transparent fill, #1A1919 text, padding 0px.

## Do's and Don'ts

- Do use #00A2C7 for the page.
- Do keep text in 4 levels: #1F1645, #1A1919, #212121, #FFFFFF.
- Do reserve #1F1645 for primary actions and key highlights.
- Do set headlines in Larsseit with tight tracking (-0.028em).
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do use 20px corners on most elements; larger surfaces also use 12px and 15px.
- Don't use #FFFFFF for body text; it reaches 3.00:1 on #00A2C7. Keep it for large text or metadata.
- Don't introduce new font families beyond Larsseit and TT Norms.
- Don't use #1F1645 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.2s.

- **Easing:** `ease-out`, `ease`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/sofi.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
