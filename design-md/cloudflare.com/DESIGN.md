---
version: alpha
name: Cloudflare
description: "Light interface measured from cloudflare.com: STK Bureau Sans type, vivid orange accents, flat surfaces and 6px corners."
colors:
  background: "#FF5E1F"
  surface: "#FF5E1F"
  on-surface: "#262626"
  on-background: "#262626"
  on-surface-variant: "#FFFFFF"
  outline: "#FFFFFF1A"
  primary: "#FF5F08"
  on-primary: "#000000"
  secondary: "#FF9910"
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
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.025em
  body-lg:
    fontFamily: STK Bureau Sans
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.025em
  body-sm:
    fontFamily: STK Bureau Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.25
  label-lg:
    fontFamily: STK Bureau Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.2
  label-md:
    fontFamily: STK Bureau Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
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
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 32px
  xl: 40px
  gutter: 10px
  section: 72px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "#1F1F1F"
    typography: "{typography.label-lg}"
    padding: 12px 24px
    height: 50px
  button-secondary:
    backgroundColor: "#F9F7F6"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    padding: 6px 12px
    height: 38px
  button-secondary-hover:
    textColor: "{colors.on-surface-variant}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 16px 12px
---

# Cloudflare Design System

## Overview

Cloudflare describes itself as: “Welcome to Cloudflare - Powering the next generation of applications” The interface is light, built on **Vivid Orange (#FF5E1F)** with **Graphite (#262626)** text, and **Vivid Orange (#FF5F08)** as the main accent.

Type is set in **STK Bureau Sans**. Headlines run large with tight negative tracking; body text is 18px. The surface language is flat. Corners are mostly 6px.

Measured from [cloudflare.com](https://www.cloudflare.com/) on November 18, 2026 at 1440×900 and 390×844 from 339 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Vivid Orange (#FF5E1F):** Page background, seen 2 times. Token `background`, CSS `--text-color-kumo-brand`.
- **Graphite (#262626):** Primary text and headings, seen 111 times. Token `on-surface`.
- **White (#FFFFFF):** Secondary text, seen 6 times. Token `on-surface-variant`.
- **White 10% (#FFFFFF1A):** Borders and dividers, seen 2 times. Token `outline`.
- **Vivid Orange (#FF5F08):** Brand color in the logo, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Orange (#FF9910):** Accent in the logo, seen 1 time. Token `secondary`.

## Typography

**STK Bureau Sans** carries the whole interface. Fallback stack: `STK Bureau Sans, sans-serif`. Other loaded fonts: Apercu Mono Pro.

- **headline-display:** STK Bureau Sans 56px at weight 500, line height 0.99, tracking -0.025em (40px on mobile). Page title (h1).
- **headline-lg:** STK Bureau Sans 48px at weight 500, line height 1, tracking -0.025em (32px on mobile). Section headings (h2).
- **headline-md:** STK Bureau Sans 32px at weight 500, line height 1, tracking -0.025em. Sub-section headings.
- **body-md:** STK Bureau Sans 18px at weight 500, line height 1.2, tracking -0.025em. Body text.
- **body-lg:** STK Bureau Sans 19px at weight 400, line height 1.2, tracking -0.025em. Lead paragraphs.
- **body-sm:** STK Bureau Sans 14px at weight 400, line height 1.25. Secondary and small text.
- **label-lg:** STK Bureau Sans 16px at weight 400, line height 1.2. Large buttons and tabs.
- **label-md:** STK Bureau Sans 14px at weight 500, line height 1. Buttons, navigation and labels.
- **label-sm:** STK Bureau Sans 13px at weight 500, line height 1.18. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (70% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 10px, lg 32px, xl 40px.
- **Sections:** 72px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 400px, 560px, 640px, 767px, 768px, 860px, 1120px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast and #FFFFFF1A borders.

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **sm (6px):** 88 elements.
- **full (9999px):** 16 elements.
- **md (8px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start building for free”):** #FFFFFF fill, #1F1F1F text, 16px/500, 3.35544e+07px radius, padding 12px 24px, border 1px solid #FFFFFF.
- **button-secondary (“Login”):** #F9F7F6 fill, #262626 text, 16px/500, 3.35544e+07px radius, padding 6px 12px, border 1px solid #F0F0F0.
- **button-secondary-hover:** background #F9F7F6, text #FFFFFF on hover.
- **button-ghost (“Shopify”):** transparent fill, #262626 text, 16px/400, padding 16px 12px.

## Do's and Don'ts

- Do use #FF5E1F for the page.
- Do keep text in 2 levels: #262626, #FFFFFF.
- Do use #FF5F08 as the brand accent: header, logo and key highlights.
- Do set headlines in STK Bureau Sans with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 10px, 32px).
- Do use 6px corners on most elements; larger surfaces also use 8px.
- Don't use #FFFFFF for body text; it reaches 3.06:1 on #FF5E1F. Keep it for large text or metadata.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond STK Bureau Sans.
- Don't use #FF5F08 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.2s, 0.16s, 0.4s, 0.3s. Longer ambient animations run 2s.

- **Easing:** `cubic-bezier(0.19, 1, 0.22, 1)`, `ease`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cloudflare.com/), the free DESIGN.md generator (engine 2026.10.29+f0c146f7cdfd).
