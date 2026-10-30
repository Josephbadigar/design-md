---
version: alpha
name: Bitwarden
description: "Light interface measured from bitwarden.com: Inter Variable type, vivid blue accents, flat surfaces and 20px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#0A171F"
  on-surface-muted: "#33465A"
  outline: "#9EA7B5"
  outline-variant: "#0000001A"
  primary: "#175DDC"
  on-primary: "#FFFFFF"
  secondary: "#0C3276"
  tertiary: "#FF4E63"
typography:
  headline-display:
    fontFamily: Inter Variable
    fontSize: 47px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.014em
  headline-lg:
    fontFamily: Inter Variable
    fontSize: 35.5px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.019em
  headline-md:
    fontFamily: Inter Variable
    fontSize: 30px
    fontWeight: 300
    lineHeight: 1.2
  headline-sm:
    fontFamily: Inter Variable
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.024em
  title-lg:
    fontFamily: Inter Variable
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.021em
  body-md:
    fontFamily: Inter Variable
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.3
  body-sm:
    fontFamily: Inter Variable
    fontSize: 14px
    fontWeight: 300
    lineHeight: 1.43
  caption:
    fontFamily: Inter Variable
    fontSize: 12px
    fontWeight: 300
    lineHeight: 1.33
  label-lg:
    fontFamily: Inter Variable
    fontSize: 18px
    fontWeight: 300
    lineHeight: 0.22
  label-md:
    fontFamily: Inter Variable
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter Variable
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.56
  headline-sm-mobile:
    fontFamily: Inter Variable
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.031em
  headline-display-mobile:
    fontFamily: Inter Variable
    fontSize: 25px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.027em
rounded:
  sm: 8px
  md: 20px
  lg: 29px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 40px
  gutter: 12px
  margin: 36px
  container: 1472px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 12px 20px
    height: 52px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    padding: 12px 20px
    height: 52px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    padding: 12px 20px
    height: 52px
  link:
    textColor: "#1D3248E6"
---

# Bitwarden Design System

## Overview

Bitwarden describes itself as: “Bitwarden is the trusted, open source password manager for individuals, teams, and enterprises. Securely store, share, and manage passwords, passkeys, and secrets. Free to start.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Blue (#175DDC)** as the main accent.

Type is set in **Inter Variable**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 20px.

Measured from [bitwarden.com](https://bitwarden.com/) on October 29, 2026 at 1440×900 and 390×844 from 390 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles, plus gradient stops #175DDC, #0C3276.

- **White (#FFFFFF):** Page background, seen 7 times. Token `background`, CSS `--color-white`.
- **Near Black (#000000):** Primary text and headings, seen 30 times. Token `on-surface`.
- **Deep Blue (#0A171F):** Secondary text, seen 11 times. Token `on-surface-variant`, CSS `--color-secondary-900`.
- **Dark Blue (#33465A):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Blue (#9EA7B5):** Borders and dividers, seen 2 times. Token `outline`.
- **Near Black 10% (#0000001A):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Vivid Blue (#175DDC):** Primary buttons and calls to action, seen 47 times. Token `primary`, CSS `--k-banner-buttons-tertiary-text-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Blue (#0C3276):** Accent in the header, seen 1 time. Token `secondary`.
- **Red (#FF4E63):** Accent (CSS variable). Token `tertiary`.

## Typography

**Inter Variable** carries the whole interface. Fallback stack: `Inter Variable, DM Sans, system-ui, -apple-system`. Other loaded fonts: bwi-font.

- **headline-display:** Inter Variable 47px at weight 600, line height 1.1, tracking -0.014em (25px on mobile). Page title (h1).
- **headline-lg:** Inter Variable 35.5px at weight 600, line height 1.1, tracking -0.019em. Section headings (h2).
- **headline-md:** Inter Variable 30px at weight 300, line height 1.2. Sub-section headings.
- **headline-sm:** Inter Variable 28px at weight 500, line height 1.1, tracking -0.024em (22px on mobile). Card and feature titles.
- **title-lg:** Inter Variable 24px at weight 600, line height 1.2, tracking -0.021em. Small titles.
- **body-md:** Inter Variable 16px at weight 300, line height 1.3. Body text.
- **body-sm:** Inter Variable 14px at weight 300, line height 1.43. Secondary and small text.
- **caption:** Inter Variable 12px at weight 300, line height 1.33. Captions and fine print.
- **label-lg:** Inter Variable 18px at weight 300, line height 0.22. Large buttons and tabs.
- **label-md:** Inter Variable 16px at weight 500, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter Variable 15px at weight 500, line height 1.56. Small labels and badges.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 40px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1472px.
- **Page margin:** 36px on each side of full-width sections.
- **Breakpoints:** 420px, 480px, 769px, 1024px, 1440px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #9EA7B5 borders.

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **md (20px):** 36 elements.
- **sm (8px):** 24 elements.
- **lg (29px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started Free”):** #175DDC fill, #FFFFFF text, 16px/500, 3.35544e+07px radius, padding 12px 20px, border 2px solid #175DDC.
- **button-outline (“Talk to Sales”):** #FFFFFF fill, #000000 text, 16px/500, 3.35544e+07px radius, padding 12px 20px, border 2px solid #175DDC.
- **button-ghost (“Talk to Sales”):** transparent fill, #000000 text, 16px/500, 3.35544e+07px radius, padding 12px 20px, border 2px solid #175DDC.
- **link:** transparent fill, #1D3248E6 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 3 levels: #000000, #0A171F, #33465A.
- Do reserve #175DDC for primary actions and key highlights.
- Do set headlines in Inter Variable with tight tracking (-0.014em).
- Do keep spacing on the 4px grid.
- Do use 20px corners on most elements; larger surfaces also use 8px and 29px.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Inter Variable.
- Don't use #175DDC for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.2s, 0.25s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/bitwarden.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
