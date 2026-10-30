---
version: alpha
name: Mercury
description: "Dark interface measured from mercury.com: arcadiaDisplay type with arcadia, indigo accents, tonal surfaces and 4px corners."
colors:
  background: "#171721"
  surface: "#171721"
  on-surface: "#EDEDF3"
  on-background: "#EDEDF3"
  on-surface-variant: "#C3C3CC"
  surface-container-low: "#1E1E2A"
  overlay: "#AFB2CE33"
  overlay-strong: "#7073931A"
  outline: "#AFB2CE5C"
  outline-variant: "#70739338"
  primary: "#5266EB"
  on-primary: "#FFFFFF"
typography:
  display-hero:
    fontFamily: arcadiaDisplay
    fontSize: 65.5px
    fontWeight: 480
    lineHeight: 1.1
  headline-display:
    fontFamily: arcadiaDisplay
    fontSize: 49.5px
    fontWeight: 480
    lineHeight: 1.1
  headline-lg:
    fontFamily: arcadiaDisplay
    fontSize: 42px
    fontWeight: 480
    lineHeight: 1.15
    letterSpacing: 0.01em
  headline-md:
    fontFamily: arcadiaDisplay
    fontSize: 32px
    fontWeight: 480
    lineHeight: 1.15
    letterSpacing: 0.015em
  headline-sm:
    fontFamily: arcadiaDisplay
    fontSize: 28px
    fontWeight: 480
    lineHeight: 1.2
    letterSpacing: 0.015em
  body-md:
    fontFamily: arcadia
    fontSize: 16px
    fontWeight: 420
    lineHeight: 1.25
  body-lg:
    fontFamily: arcadia
    fontSize: 18px
    fontWeight: 480
    lineHeight: 1.35
  body-sm:
    fontFamily: arcadia
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.02em
  label-md:
    fontFamily: arcadia
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: arcadiaDisplay
    fontSize: 28px
    fontWeight: 480
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: arcadiaDisplay
    fontSize: 28px
    fontWeight: 480
    lineHeight: 1.2
    letterSpacing: 0.015em
rounded:
  sm: 4px
  md: 32px
  lg: 40px
spacing:
  base: 4px
  xs: 2px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 20px
    height: 40px
  button-outline:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px 20px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px 20px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 0px 0px 20px
  link:
    textColor: "{colors.on-surface}"
---

# Mercury Design System

## Overview

Mercury describes itself as: “Everything you do with money. All in one place. Apply in 10 minutes for business banking that transforms how you operate.” The interface is dark, built on **Cool Charcoal (#171721)** with **Cool Mist (#EDEDF3)** text, and **Indigo (#5266EB)** as the main accent.

Type is set in **arcadiaDisplay** and **arcadia**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 4px.

Measured from [mercury.com](https://mercury.com/) on October 29, 2026 at 1440×900 and 390×844 from 419 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Cool Charcoal (#171721):** Page background, seen 2 times. Token `background`.
- **Cool Mist (#EDEDF3):** Primary text and headings, seen 37 times. Token `on-surface`, CSS `--text-default-inverted`.
- **Cool Silver (#C3C3CC):** Secondary text, seen 29 times. Token `on-surface-variant`, CSS `--color-neutral-base-300`.
- **Cool Graphite (#1E1E2A):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--text-emphasized`.
- **Light Indigo 20% (#AFB2CE33):** Translucent fill for cards and controls, seen 5 times. Token `overlay`.
- **Indigo 10% (#7073931A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`, CSS `--surface-frosted`.
- **Light Indigo 36% (#AFB2CE5C):** Borders and dividers, seen 2 times. Token `outline`, CSS `--color-neutral-magic-400-alpha-5`.
- **Indigo 22% (#70739338):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Indigo (#5266EB):** Primary buttons and calls to action, seen 2 times. Token `primary`, CSS `--surface-primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**arcadiaDisplay** and **arcadia** share the interface. Fallback stack: `arcadiaDisplay, arcadiaDisplay Fallback`.

- **display-hero:** arcadiaDisplay 65.5px at weight 480, line height 1.1. Oversized hero statements.
- **headline-display:** arcadiaDisplay 49.5px at weight 480, line height 1.1 (28px on mobile). Page title (h1).
- **headline-lg:** arcadiaDisplay 42px at weight 480, line height 1.15, tracking 0.01em (28px on mobile). Section headings (h2).
- **headline-md:** arcadiaDisplay 32px at weight 480, line height 1.15, tracking 0.015em. Sub-section headings.
- **headline-sm:** arcadiaDisplay 28px at weight 480, line height 1.2, tracking 0.015em. Card and feature titles.
- **body-md:** arcadia 16px at weight 420, line height 1.25. Body text.
- **body-lg:** arcadia 18px at weight 480, line height 1.35. Lead paragraphs.
- **body-sm:** arcadia 12px at weight 400, line height 1.4, tracking 0.02em. Secondary and small text.
- **label-md:** arcadia 16px at weight 400, line height 1.5. Buttons, navigation and labels.

## Layout

Spacing follows a 4px grid: 91% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 2px, sm 8px, md 16px, lg 32px, xl 40px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#1E1E2A) and #AFB2CE5C borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 360 elements.
- **lg (40px):** 28 elements.
- **md (32px):** 14 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Open account”):** #5266EB fill, #FFFFFF text, 16px/420, 32px radius, padding 0px 20px.
- **button-outline (“Launch demo”):** #AFB2CE33 fill, #EDEDF3 text, 16px/420, 40px radius, padding 0px 20px, border 1px solid #AFB2CE5C.
- **button-ghost (“Products”):** transparent fill, #EDEDF3 text, 16px/420, 40px radius, padding 0px 20px.
- **input-field (“Enter your email”):** transparent fill, #EDEDF3 text, 16px/420, 32px 0px 0px 32px radius, padding 0px 0px 0px 20px.
- **link:** transparent fill, #EDEDF3 text, padding 0px.

## Do's and Don'ts

- Do use #171721 for the page and lift surfaces in small steps: #1E1E2A.
- Do keep text in 2 levels: #EDEDF3, #C3C3CC.
- Do reserve #5266EB for primary actions and key highlights.
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 40px and 32px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond arcadiaDisplay and arcadia.
- Don't use #5266EB for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.5s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.6, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/mercury.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
