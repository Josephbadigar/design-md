---
version: alpha
name: Resend
description: "Dark monochrome interface measured from resend.com: domaine type with aBCFavorit, tonal surfaces and 16px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#F0F0F0"
  on-background: "#F0F0F0"
  on-surface-variant: "#ABAFB4"
  on-surface-muted: "#A1A4A5"
  on-surface-subtle: "#A0A0A0"
  surface-container-low: "#0B0E14"
  overlay: "#D6EBFD30"
  outline: "#D9EDFE25"
  outline-variant: "#D6EBFD30"
  primary: "#0B0E14"
  on-primary: "#F0F0F0"
  secondary: "#9281F7"
typography:
  headline-display:
    fontFamily: domaine
    fontSize: 96px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: aBCFavorit
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.05em
  headline-md:
    fontFamily: aBCFavorit
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1
  body-md:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: domaine
    fontSize: 64px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: aBCFavorit
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.05em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  xl: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 16px
  section: 96px
  margin: 24px
  container: 1280px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    padding: 0px
    height: 32px
  button-primary-hover:
    backgroundColor: "#0B0E14D1"
  button-secondary:
    textColor: "#FFFFFF"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label-sm}"
    rounded: 0px
    padding: 4px 12px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Resend Design System

## Overview

Resend describes itself as: “The best way to reach humans instead of spam folders. Deliver transactional and marketing emails at scale.” The interface is dark, built on **Near Black (#000000)** with **Mist (#F0F0F0)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **domaine** and **aBCFavorit**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 16px.

Measured from [resend.com](https://resend.com/) on October 29, 2026 at 1440×900 and 390×844 from 421 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles, plus gradient stops #9281F7, #9A54DC.

- **Near Black (#000000):** Page background, seen 10 times. Token `background`.
- **Mist (#F0F0F0):** Primary text and headings, seen 19 times. Token `on-surface`.
- **Cool Gray (#ABAFB4):** Secondary text, seen 33 times. Token `on-surface-variant`.
- **Gray (#A1A4A5):** Muted text and metadata, seen 34 times. Token `on-surface-muted`.
- **Gray (#A0A0A0):** Subtle text and placeholders, seen 10 times. Token `on-surface-subtle`.
- **Cool Charcoal (#0B0E14):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Pale Blue 19% (#D6EBFD30):** Translucent fill for cards and controls, seen 3 times. Token `overlay`.
- **Pale Blue 14% (#D9EDFE25):** Borders and dividers, seen 30 times. Token `outline`.
- **Pale Blue 19% (#D6EBFD30):** Secondary dividers, seen 14 times. Token `outline-variant`.
- **Cool Charcoal (#0B0E14):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **Mist (#F0F0F0):** Text and icons on primary. Token `on-primary`.
- **Light Indigo (#9281F7):** Accent in text, fills and borders, seen 5 times. Token `secondary`.

## Typography

**domaine**, **aBCFavorit** and **inter** share the interface. Fallback stack: `domaine, ui-sans-serif, system-ui, sans-serif`. Other loaded fonts: commitMono.

- **headline-display:** domaine 96px at weight 400, line height 1, tracking -0.01em (64px on mobile). Page title (h1).
- **headline-lg:** aBCFavorit 56px at weight 400, line height 1.2, tracking -0.05em (48px on mobile). Section headings (h2).
- **headline-md:** aBCFavorit 20px at weight 400, line height 1. Sub-section headings.
- **body-md:** inter 14px at weight 400, line height 1.43. Body text.
- **body-lg:** inter 18px at weight 400, line height 1.5. Lead paragraphs.
- **body-sm:** inter 12px at weight 400, line height 1.33. Secondary and small text.
- **label-md:** inter 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** inter 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (81% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 375px, 1000px, 1160px, 1340px, 1920px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`

## Shapes

Most elements use 16px corners. Measured radii, most used first:

- **xl (16px):** 164 elements.
- **md (6px):** 120 elements.
- **lg (8px):** 80 elements.
- **sm (4px):** 60 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“What you missed at Resend Forwar”):** #0B0E14 fill, #F0F0F0 text, 14px/400, 3.35544e+07px radius, padding 0px.
- **button-primary-hover:** background #0B0E14D1, text #F0F0F0 on hover.
- **button-secondary (“Get started”):** transparent fill, #FFFFFF text, 14px/600, 16px radius, padding 0px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`.
- **button-ghost (“Features”):** transparent fill, #A1A4A5 text, 14px/500, padding 4px 12px.
- **input-field:** transparent fill, #F0F0F0 text, 16px/400, padding 0px.
- **link:** transparent fill, #F1F7FEB5 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page and lift surfaces in small steps: #0B0E14.
- Do keep text in 4 levels: #F0F0F0, #ABAFB4, #A1A4A5, #A0A0A0.
- Do let contrast carry emphasis; primary actions use #0B0E14 on #000000.
- Do set headlines in domaine with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 16px corners on most elements; larger surfaces also use 6px, 8px and 4px.
- Don't introduce new font families beyond domaine, aBCFavorit and inter.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.2s.

## Motion

Interface transitions are quick: 0.2s, 0.15s. Longer ambient animations run 30s, 1s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.4, 0, 1, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/resend.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
