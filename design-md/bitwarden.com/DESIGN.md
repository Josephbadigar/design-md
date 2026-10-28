---
version: alpha
name: Bitwarden
description: "Dark interface measured from bitwarden.com: Inter Variable type, dark blue accents, flat surfaces and 20px corners."
colors:
  background: "#0A171F"
  surface: "#0A171F"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F3F6F9"
  on-surface-muted: "#B8C0CB"
  overlay: "#020F6633"
  outline: "#FFFFFF1A"
  outline-variant: "#5B5D6066"
  primary: "#0C3276"
  on-primary: "#FFFFFF"
  secondary: "#65ABFF"
  tertiary: "#FF4E63"
  success: "#6BF178"
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
    backgroundColor: "{colors.on-surface}"
    textColor: "#000000"
    typography: "{typography.label-md}"
    padding: 12px 20px
    height: 52px
  button-primary-hover:
    backgroundColor: "#A2F4FD"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "#1D3248"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px 16px
    height: 40px
  button-secondary-hover:
    backgroundColor: "{colors.on-surface-variant}"
  button-outline:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 0px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.lg}"
    padding: 0px 16px
  input-field:
    backgroundColor: "#1D3248"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px 32px 0px 40px
  link:
    textColor: "#CBD2DEE6"
---

# Bitwarden Design System

## Overview

Bitwarden describes itself as: “Bitwarden is the trusted, open source password manager for individuals, teams, and enterprises. Securely store, share, and manage passwords, passkeys, and secrets. Free to start.” The interface is dark, built on **Deep Blue (#0A171F)** with **White (#FFFFFF)** text, and **Dark Blue (#0C3276)** as the main accent.

Type is set in **Inter Variable**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 20px.

Measured from [bitwarden.com](https://bitwarden.com/) on October 21, 2026 at 1440×900 and 390×844 from 381 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #65ABFF.

- **Deep Blue (#0A171F):** Page background, seen 4 times. Token `background`, CSS `--color-secondary-900`.
- **White (#FFFFFF):** Primary text and headings, seen 96 times. Token `on-surface`, CSS `--color-white`.
- **Cool Snow (#F3F6F9):** Secondary text, seen 14 times. Token `on-surface-variant`.
- **Light Blue (#B8C0CB):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **Deep Indigo 20% (#020F6633):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 2 times. Token `outline`.
- **Slate 40% (#5B5D6066):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Dark Blue (#0C3276):** Brand color in the header. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#65ABFF):** Secondary buttons, seen 40 times. Token `secondary`.
- **Red (#FF4E63):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.
- **Green (#6BF178):** Success and positive states, seen 1 time. Token `success`.

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

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #FFFFFF1A borders.

## Shapes

Most elements use 20px corners. Measured radii, most used first:

- **md (20px):** 36 elements.
- **sm (8px):** 20 elements.
- **lg (29px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started Free”):** #FFFFFF fill, #000000 text, 16px/500, 3.35544e+07px radius, padding 12px 20px, border 2px solid #FFFFFF.
- **button-primary-hover:** background #A2F4FD, text #000000 on hover.
- **button-secondary (“Accept All”):** #65ABFF fill, #1D3248 text, 14px/600, 20px radius, padding 0px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-secondary-hover:** background #F3F6F9, text #1D3248 on hover.
- **button-outline (“Reject All”):** transparent fill, #F3F6F9 text, 14px/600, 29px radius, padding 0px 16px, border 1px solid #F3F6F9, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-ghost (“Reject All”):** transparent fill, #F3F6F9 text, 14px/600, 29px radius, padding 0px 16px, border 1px solid #F3F6F9, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **input-field:** #1D3248 fill, #F3F6F9 text, 16px/300, 8px radius, padding 0px 32px 0px 40px, border 1px solid #8F98A6.
- **link:** transparent fill, #CBD2DEE6 text, padding 0px.

## Do's and Don'ts

- Do use #0A171F for the page.
- Do keep text in 3 levels: #FFFFFF, #F3F6F9, #B8C0CB.
- Do use #0C3276 as the brand accent: header, logo and key highlights.
- Do set headlines in Inter Variable with tight tracking (-0.014em).
- Do keep spacing on the 4px grid.
- Do use 20px corners on most elements; larger surfaces also use 8px and 29px.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Inter Variable.
- Don't use #0C3276 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.2s, 0.25s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/bitwarden.com/), the free DESIGN.md generator.
