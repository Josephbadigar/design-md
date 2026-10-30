---
version: alpha
name: Granola
description: "Light interface measured from granola.ai: quadrant type with melange, yellow accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#292929"
  on-background: "#292929"
  on-surface-strong: "#0E0F0C"
  on-surface-variant: "#72726E"
  on-surface-muted: "#ACADA8"
  surface-container-low: "#F7F7F2"
  surface-container: "#EAEBE5"
  surface-container-high: "#D5D5D2"
  overlay: "#625A220F"
  outline: "#0000001A"
  outline-variant: "#47432A33"
  primary: "#B2C248"
  on-primary: "#000000"
  secondary: "#5B6F00"
  tertiary: "#E0C976"
typography:
  display-hero:
    fontFamily: quadrant
    fontSize: 108px
    fontWeight: 400
    lineHeight: 0.97
    letterSpacing: -0.02em
  headline-display:
    fontFamily: quadrant
    fontSize: 86.5px
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: quadrant
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1
  headline-md:
    fontFamily: quadrant
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: -0.01em
  body-md:
    fontFamily: melange
    fontSize: 14px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: 0.02em
  body-lg:
    fontFamily: melange
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: melange
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: melange
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.29
    letterSpacing: 0.01em
  label-md:
    fontFamily: melange
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: 0.02em
  label-sm:
    fontFamily: melange
    fontSize: 10px
    fontWeight: 600
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: quadrant
    fontSize: 48px
    fontWeight: 400
    lineHeight: 0.93
    letterSpacing: -0.02em
  display-hero-mobile:
    fontFamily: quadrant
    fontSize: 60px
    fontWeight: 400
    lineHeight: 0.97
    letterSpacing: -0.02em
  headline-md-mobile:
    fontFamily: quadrant
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: -0.01em
rounded:
  sm: 10px
  md: 28px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 8px
  section: 112px
  margin: 40px
  container: 1280px
components:
  button-primary:
    backgroundColor: "{colors.secondary}"
    textColor: "#FCFCF8"
    typography: "{typography.body-lg}"
    padding: 9px 24px
    height: 56px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    padding: 6px 12px 6px 6px
    height: 32px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 6px 12px
    height: 38px
---

# Granola Design System

## Overview

Granola describes itself as: “The AI notepad for back-to-back meetings. Notes, actions and memory. Without a meeting bot.” The interface is light, built on **White (#FFFFFF)** with **Graphite (#292929)** text, and **Yellow (#B2C248)** as the main accent.

Type is set in **quadrant** and **melange**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [granola.ai](https://www.granola.ai/) on October 29, 2026 at 1440×900 and 390×844 from 325 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles, plus gradient stops #FEBE29, #FF91E0, #CEBEF8, #D2E4F8.

- **White (#FFFFFF):** Page background, seen 3 times. Token `background`, CSS `--color-white`.
- **Graphite (#292929):** Primary text and headings, seen 65 times. Token `on-surface`, CSS `--color-oats-neutral-800`.
- **Charcoal (#0E0F0C):** Headings and emphasis, seen 7 times. Token `on-surface-strong`.
- **Slate (#72726E):** Secondary text, seen 10 times. Token `on-surface-variant`, CSS `--oats-ink-secondary-static`.
- **Gray (#ACADA8):** Muted text and metadata, seen 3 times. Token `on-surface-muted`, CSS `--color-fill-neutral`.
- **Snow (#F7F7F2):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Mist (#EAEBE5):** Cards and panels, seen 3 times. Token `surface-container`.
- **Silver (#D5D5D2):** Hover and pressed fills, seen 9 times. Token `surface-container-high`, CSS `--oats-fill-soft-opaque-hover`.
- **Dark Yellow 6% (#625A220F):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Near Black 10% (#0000001A):** Borders and dividers, seen 3 times. Token `outline`.
- **Dark Amber 20% (#47432A33):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--oats-border-hairline`.
- **Yellow (#B2C248):** Brand color on large areas, seen 1 time. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Deep Lime (#5B6F00):** Secondary buttons, seen 1 time. Token `secondary`, CSS `--oats-ink-accent-strong`.
- **Amber (#E0C976):** Accent in the header. Token `tertiary`.

## Typography

**quadrant** and **melange** share the interface. Fallback stack: `quadrant, quadrant Fallback`.

- **display-hero:** quadrant 108px at weight 400, line height 0.97, tracking -0.02em (60px on mobile). Oversized hero statements.
- **headline-display:** quadrant 86.5px at weight 400, line height 0.93, tracking -0.02em (48px on mobile). Page title (h1).
- **headline-lg:** quadrant 48px at weight 400, line height 1. Section headings (h2).
- **headline-md:** quadrant 32px at weight 400, line height 1.05, tracking -0.01em (24px on mobile). Sub-section headings.
- **body-md:** melange 14px at weight 400, line height 0.95, tracking 0.02em. Body text.
- **body-lg:** melange 16px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** melange 10px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** melange 14px at weight 500, line height 1.29, tracking 0.01em. Large buttons and tabs.
- **label-md:** melange 12px at weight 600, line height 1.5, tracking 0.02em. Buttons, navigation and labels.
- **label-sm:** melange 10px at weight 600, line height 1.5. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 70% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 24px, xl 40px.
- **Sections:** 112px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 640px, 767px, 768px, 999px, 1000px, 1024px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 8px 12px -4px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (10px):** 4 elements.
- **md (28px):** 4 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Download for free”):** #5B6F00 fill, #FCFCF8 text, 16px/430, 3.35544e+07px radius, padding 9px 24px.
- **button-outline (“New Voice typing by Granola”):** #F7F7F2 fill, #292929 text, 16px/400, 3.35544e+07px radius, padding 6px 12px 6px 6px.
- **button-ghost (“Talk to sales”):** transparent fill, #292929 text, 14px/400, 3.35544e+07px radius, padding 6px 12px, border 1px solid #47432A33.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F7F2, #EAEBE5, #D5D5D2.
- Do keep text in 4 levels: #292929, #0E0F0C, #72726E, #ACADA8.
- Do use #B2C248 as the brand accent: header, logo and key highlights.
- Do set headlines in quadrant with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 10px corners.
- Don't use #ACADA8 for body text; it reaches 2.26:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond quadrant and melange.
- Don't use #B2C248 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.15s, 0.5s, 0.2s, 0.4s. Longer ambient animations run 0.92s, 2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in-out`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/granola.ai/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
