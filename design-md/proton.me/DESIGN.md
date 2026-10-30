---
version: alpha
name: Proton
description: "Light interface measured from proton.me: ProtonSerif type with ProtonSans, indigo accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#4B5563"
  on-background: "#4B5563"
  on-surface-variant: "#A6ACB7"
  overlay: "#9CA3AF66"
  overlay-strong: "#9CA3AF1A"
  outline: "#D1D5DB99"
  outline-variant: "#C5B7FF"
  primary: "#6D4AFF"
  on-primary: "#FFFFFF"
  inverse-surface: "#9CA3AF"
  secondary: "#372580"
typography:
  headline-display:
    fontFamily: ProtonSerif
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1.06
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: ProtonSerif
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  headline-md:
    fontFamily: ProtonSerif
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.16
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: ProtonSerif
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.13
    letterSpacing: -0.04em
  title-lg:
    fontFamily: ProtonSans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.5
  body-md:
    fontFamily: ProtonSans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
  body-lg:
    fontFamily: ProtonSans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.55
  body-sm:
    fontFamily: ProtonSans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: ProtonSans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: ProtonSans
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.57
  headline-display-mobile:
    fontFamily: ProtonSerif
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.11
    letterSpacing: -0.04em
  headline-md-mobile:
    fontFamily: ProtonSerif
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.16
    letterSpacing: -0.04em
rounded:
  full: 9999px
spacing:
  xs: 4px
  sm: 6px
  md: 16px
  lg: 20px
  xl: 48px
  gutter: 8px
  section: 48px
  margin: 64px
  container: 1920px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 4px 12px
    height: 30px
  button-primary-hover:
    backgroundColor: "#4A2DC5"
  button-ghost:
    textColor: "{colors.secondary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 6px 16px
  link:
    textColor: "{colors.secondary}"
---

# Proton Design System

## Overview

Proton describes itself as: “Over 100 million people use Proton to stay private and secure online. Get a free Proton account and take back your privacy.” The interface is light, built on **White (#FFFFFF)** with **Dark Blue (#4B5563)** text, and **Indigo (#6D4AFF)** as the main accent.

Type is set in **ProtonSerif** and **ProtonSans**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [proton.me](https://proton.me/) on October 29, 2026 at 1440×900 and 390×844 from 398 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Dark Blue (#4B5563):** Primary text and headings, seen 59 times. Token `on-surface`.
- **Cool Gray (#A6ACB7):** Secondary text, seen 5 times. Token `on-surface-variant`.
- **Blue 40% (#9CA3AF66):** Translucent fill for cards and controls, seen 10 times. Token `overlay`.
- **Blue 10% (#9CA3AF1A):** Stronger translucent fill, seen 5 times. Token `overlay-strong`.
- **Cool Silver 60% (#D1D5DB99):** Borders and dividers, seen 3 times. Token `outline`.
- **Light Indigo (#C5B7FF):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Indigo (#6D4AFF):** Primary buttons and calls to action, seen 71 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#9CA3AF):** High-contrast fills, seen 4 times. Token `inverse-surface`.
- **Dark Indigo (#372580):** Links and interactive text, seen 54 times. Token `secondary`.

## Typography

**ProtonSerif** and **ProtonSans** share the interface. Fallback stack: `ProtonSerif, ProtonSerifFallback, ProtonScript, ui-serif`.

- **headline-display:** ProtonSerif 60px at weight 400, line height 1.06, tracking -0.04em (36px on mobile). Page title (h1).
- **headline-lg:** ProtonSerif 48px at weight 400, line height 1.13, tracking -0.04em. Section headings (h2).
- **headline-md:** ProtonSerif 36px at weight 400, line height 1.16, tracking -0.04em (24px on mobile). Sub-section headings.
- **headline-sm:** ProtonSerif 30px at weight 400, line height 1.13, tracking -0.04em. Card and feature titles.
- **title-lg:** ProtonSans 20px at weight 600, line height 1.5. Small titles.
- **body-md:** ProtonSans 14px at weight 400, line height 1.57. Body text.
- **body-lg:** ProtonSans 18px at weight 400, line height 1.55. Lead paragraphs.
- **body-sm:** ProtonSans 12px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** ProtonSans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** ProtonSans 14px at weight 600, line height 1.57. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (85% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 16px, lg 20px, xl 48px.
- **Sections:** 48px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1920px.
- **Page margin:** 64px on each side of full-width sections.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps and hairline rings:

- `rgb(255, 255, 255) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 2px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgb(255, 255, 255) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 1px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgb(109, 74, 255) 0px 0px 0px 2px inset`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 228 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Create a free account”):** #6D4AFF fill, #FFFFFF text, 14px/600, 9999px radius, padding 4px 12px.
- **button-primary-hover:** background #4A2DC5, text #FFFFFF on hover.
- **button-ghost (“Personal”):** transparent fill, #372580 text, 14px/600, 9999px radius, padding 6px 16px, shadow `rgb(255, 255, 255) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 1px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **link:** transparent fill, #372580 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #4B5563, #A6ACB7.
- Do reserve #6D4AFF for primary actions and key highlights.
- Do set headlines in ProtonSerif with tight tracking (-0.04em).
- Do reuse the measured spacing steps (6px, 16px, 20px).
- Do make buttons and chips fully rounded (9999px).
- Don't use #A6ACB7 for body text; it reaches 2.28:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and borders and contrast.
- Don't introduce new font families beyond ProtonSerif and ProtonSans.
- Don't use #6D4AFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/proton.me/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
