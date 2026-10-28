---
version: alpha
name: Cloudflare
description: "Light interface measured from cloudflare.com: STK Bureau Sans type, vivid orange accents, flat surfaces and 6px corners."
colors:
  background: "#FF5E1F"
  surface: "#FF5E1F"
  on-surface: "#1F1F1F"
  on-background: "#1F1F1F"
  on-surface-variant: "#FFFBF5"
  on-surface-muted: "#F0E3DE"
  overlay: "#FF5E1F1A"
  overlay-strong: "#FFFFFF40"
  outline: "#F0E3DE20"
  outline-variant: "#FFFBF580"
  primary: "#FF5E1F"
  on-primary: "#000000"
  inverse-surface: "#151414"
  secondary: "#FF5F08"
  tertiary: "#FF9910"
  error: "#FF5B66"
typography:
  headline-display:
    fontFamily: STK Bureau Sans
    fontSize: 56px
    fontWeight: 500
    lineHeight: 0.99
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: STK Bureau Sans
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  headline-md:
    fontFamily: STK Bureau Sans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  body-md:
    fontFamily: STK Bureau Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.2
  body-lg:
    fontFamily: STK Bureau Sans
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.025em
  label-lg:
    fontFamily: STK Bureau Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: STK Bureau Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.25
  label-sm:
    fontFamily: STK Bureau Sans
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.18
  headline-display-mobile:
    fontFamily: STK Bureau Sans
    fontSize: 40px
    fontWeight: 600
    lineHeight: 0.99
    letterSpacing: -0.025em
  headline-lg-mobile:
    fontFamily: STK Bureau Sans
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
rounded:
  sm: 6px
  md: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 40px
  gutter: 8px
  section: 72px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    padding: 12px 24px
    height: 50px
  button-primary-hover:
    backgroundColor: "#2A2927"
    textColor: "{colors.on-surface-variant}"
  button-secondary:
    backgroundColor: "#2A2927"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label-lg}"
    padding: 6px 12px
    height: 38px
  button-secondary-hover:
    textColor: "{colors.on-surface-variant}"
  button-ghost:
    textColor: "#9A9390"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
---

# Cloudflare Design System

## Overview

Cloudflare describes itself as: “Welcome to Cloudflare - Powering the next generation of applications” The interface is light, built on **Vivid Orange (#FF5E1F)** with **Charcoal (#1F1F1F)** text, and **Vivid Orange (#FF5E1F)** as the main accent.

Type is set in **STK Bureau Sans**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 6px.

Measured from [cloudflare.com](https://www.cloudflare.com/) on October 21, 2026 at 1440×900 and 390×844 from 314 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles.

- **Vivid Orange (#FF5E1F):** Page background, seen 3 times. Token `background`, CSS `--text-color-kumo-brand`.
- **Charcoal (#1F1F1F):** Primary text and headings, seen 2 times. Token `on-surface`.
- **Warm Snow (#FFFBF5):** Secondary text, seen 19 times. Token `on-surface-variant`.
- **Pale Orange (#F0E3DE):** Muted text and metadata, seen 77 times. Token `on-surface-muted`, CSS `--color-border-200`.
- **Vivid Orange 10% (#FF5E1F1A):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **White 25% (#FFFFFF40):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Pale Orange 13% (#F0E3DE20):** Borders and dividers, seen 22 times. Token `outline`, CSS `--color-border-100-50`.
- **Warm Snow 50% (#FFFBF580):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Vivid Orange (#FF5E1F):** Brand color on large areas, seen 6 times. Token `primary`, CSS `--text-color-kumo-brand`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#151414):** High-contrast fills, seen 4 times. Token `inverse-surface`.
- **Vivid Orange (#FF5F08):** Brand color in the logo, seen 15 times. Token `secondary`.
- **Vivid Orange (#FF9910):** Brand color in the logo, seen 15 times. Token `tertiary`.
- **Red (#FF5B66):** Errors and destructive states, seen 2 times. Token `error`.

## Typography

**STK Bureau Sans** carries the whole interface. Fallback stack: `STK Bureau Sans, sans-serif`. Other loaded fonts: Apercu Mono Pro.

- **headline-display:** STK Bureau Sans 56px at weight 500, line height 0.99, tracking -0.025em (40px on mobile). Page title (h1).
- **headline-lg:** STK Bureau Sans 48px at weight 500, line height 1, tracking -0.025em (32px on mobile). Section headings (h2).
- **headline-md:** STK Bureau Sans 32px at weight 500, line height 1, tracking -0.025em. Sub-section headings.
- **body-md:** STK Bureau Sans 16px at weight 400, line height 1.2. Body text.
- **body-lg:** STK Bureau Sans 18px at weight 500, line height 1.2, tracking -0.025em. Lead paragraphs.
- **label-lg:** STK Bureau Sans 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** STK Bureau Sans 14px at weight 400, line height 1.25. Buttons, navigation and labels.
- **label-sm:** STK Bureau Sans 13px at weight 500, line height 1.18. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (71% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 40px.
- **Sections:** 72px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 400px, 560px, 640px, 767px, 768px, 860px, 1120px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #F0E3DE20 borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **sm (6px):** 80 elements.
- **md (8px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start building for free”):** #FFFBF5 fill, #1F1F1F text, 16px/500, 3.35544e+07px radius, padding 12px 24px, border 1px solid #FFFBF5.
- **button-primary-hover:** background #2A2927, text #FFFBF5 on hover.
- **button-secondary (“Login”):** #2A2927 fill, #F0E3DE text, 16px/500, 3.35544e+07px radius, padding 6px 12px, border 1px solid #F0E3DE20.
- **button-secondary-hover:** background #2A2927, text #FFFBF5 on hover.
- **button-ghost (“Your privacy choices”):** transparent fill, #9A9390 text, 14px/400, padding 0px.

## Do's and Don'ts

- Do use #FF5E1F for the page.
- Do keep text in 3 levels: #1F1F1F, #FFFBF5, #F0E3DE.
- Do use #FF5E1F as the brand accent: header, logo and key highlights.
- Do set headlines in STK Bureau Sans with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 12px, 32px).
- Do use 6px corners on most elements; larger surfaces also use 8px.
- Don't use #FFFBF5 for body text; it reaches 3.0:1 on #FF5E1F. Keep it for large text or metadata.
- Don't use #F0E3DE for body text; it reaches 2.4:1 on #FF5E1F. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond STK Bureau Sans.
- Don't use #FF5E1F for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.2s, 0.4s, 0.16s, 0.3s. Longer ambient animations run 2s.

- **Easing:** `cubic-bezier(0.19, 1, 0.22, 1)`, `ease-out`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cloudflare.com/), the free DESIGN.md generator.
