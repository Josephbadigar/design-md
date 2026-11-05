---
version: alpha
name: Shapr3D
description: "Dark interface measured from shapr3d.com: PP Fraktion Sans type with Inter, vivid blue accents, tonal surfaces and 1px corners."
colors:
  background: "#0D0D0D"
  surface: "#0D0D0D"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F2F2F2"
  on-surface-muted: "#D9D9D9"
  surface-container-low: "#1A1A1A"
  outline: "#505050"
  primary: "#1D4EFF"
  on-primary: "#FFFFFF"
  secondary: "#0099E9"
  tertiary: "#0E111B"
typography:
  headline-display:
    fontFamily: PP Fraktion Sans
    fontSize: 72px
    fontWeight: 900
    lineHeight: 0.9
    letterSpacing: -0.033em
  headline-lg:
    fontFamily: PP Fraktion Sans
    fontSize: 64px
    fontWeight: 900
    lineHeight: 0.9
    letterSpacing: -0.047em
  headline-md:
    fontFamily: PP Fraktion Sans
    fontSize: 40px
    fontWeight: 700
    lineHeight: 0.9
    letterSpacing: -0.05em
  headline-sm:
    fontFamily: PP Fraktion Sans
    fontSize: 28px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.02em
  title-lg:
    fontFamily: PP Fraktion Sans
    fontSize: 22px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.45
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: PP Fraktion Sans
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: -0.03em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  code:
    fontFamily: PP Fraktion Mono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0.03em
  headline-display-mobile:
    fontFamily: PP Fraktion Sans
    fontSize: 40px
    fontWeight: 900
    lineHeight: 0.9
    letterSpacing: -0.06em
  headline-lg-mobile:
    fontFamily: PP Fraktion Sans
    fontSize: 32px
    fontWeight: 900
    lineHeight: 0.9
    letterSpacing: -0.094em
  headline-md-mobile:
    fontFamily: PP Fraktion Sans
    fontSize: 32px
    fontWeight: 700
    lineHeight: 0.9
    letterSpacing: -0.063em
rounded:
  md: 1px
spacing:
  sm: 8px
  md: 16px
  lg: 32px
  xl: 48px
  gutter: 10px
  section: 60px
  margin: 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 8px 16px 10px 16px
    height: 42px
  button-primary-hover:
    backgroundColor: "#0A30D3"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px
    height: 38px
  button-outline-hover:
    backgroundColor: "#1D4EFF0F"
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 8px 16px 10px 16px
    height: 42px
  link:
    textColor: "{colors.on-surface}"
---

# Shapr3D Design System

## Overview

Shapr3D describes itself as: “Experience the world’s most intuitive 3D modeling software for iPadOS, iOS, Windows & macOS. Download now and start your first professional CAD project for free.” The interface is dark, built on **Charcoal (#0D0D0D)** with **White (#FFFFFF)** text, and **Vivid Blue (#1D4EFF)** as the main accent.

Type is set in **PP Fraktion Sans** and **Inter**, with **PP Fraktion Mono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 1px.

Measured from [shapr3d.com](https://www.shapr3d.com/) on November 4, 2026 at 1440×900 and 390×844 from 323 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Charcoal (#0D0D0D):** Page background, seen 19 times. Token `background`, CSS `--shapr-text-primary`.
- **White (#FFFFFF):** Primary text and headings, seen 102 times. Token `on-surface`, CSS `--ctabackgroundprimary-new`.
- **Mist (#F2F2F2):** Secondary text, seen 6 times. Token `on-surface-variant`, CSS `--shapr-border-5th-type`.
- **Silver (#D9D9D9):** Muted text and metadata, seen 27 times. Token `on-surface-muted`, CSS `--shapr-bg-tertiary`.
- **Charcoal (#1A1A1A):** Raised areas one step from the page, seen 4 times. Token `surface-container-low`.
- **Slate (#505050):** Borders and dividers, seen 4 times. Token `outline`, CSS `--ctabackgroundsecondaryhover`.
- **Vivid Blue (#1D4EFF):** Brand color in the header, seen 8 times. Token `primary`, CSS `--ctabackgroundprimary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0099E9):** Accent (CSS variable). Token `secondary`.
- **Cool Charcoal (#0E111B):** Accent (CSS variable). Token `tertiary`.

## Typography

**PP Fraktion Sans**, **Inter** and **PP Fraktion Mono** (monospace) share the interface. Fallback stack: `PP Fraktion Sans, sans-serif`.

- **headline-display:** PP Fraktion Sans 72px at weight 900, line height 0.9, tracking -0.033em, uppercase (40px on mobile). Page title (h1).
- **headline-lg:** PP Fraktion Sans 64px at weight 900, line height 0.9, tracking -0.047em, uppercase (32px on mobile). Section headings (h2).
- **headline-md:** PP Fraktion Sans 40px at weight 700, line height 0.9, tracking -0.05em (32px on mobile). Sub-section headings.
- **headline-sm:** PP Fraktion Sans 28px at weight 700, line height 1, tracking -0.02em. Card and feature titles.
- **title-lg:** PP Fraktion Sans 22px at weight 700, line height 1.1, tracking -0.02em. Small titles.
- **body-md:** Inter 16px at weight 400, line height 1.45. Body text.
- **body-sm:** Inter 12px at weight 400, line height 1.5. Secondary and small text.
- **label-md:** PP Fraktion Sans 16px at weight 700, line height 1.5, tracking -0.03em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 400, line height 1.43. Small labels and badges.
- **code:** PP Fraktion Mono 14px at weight 400, line height 1, tracking 0.03em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** sm 8px, md 16px, lg 32px, xl 48px.
- **Sections:** 60px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Page margin:** 48px on each side of full-width sections.
- **Breakpoints:** 320px, 400px, 449px, 479px, 600px, 639px, 640px, 767px, 768px, 991px, 992px, 1160px, 1440px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.2) 0px 1px 2px 0px, rgba(0, 0, 0, 0.05) 0px 0px 0px 1px, rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(255, 255, 255, 0.05) 0px -1px 0px 0px inset`

## Shapes

Most elements use 1px corners. Measured radii, most used first:

- **md (1px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“SIGN UP”):** #1D4EFF fill, #FFFFFF text, 16px/700, padding 8px 16px 10px 16px, shadow `rgba(0, 0, 0, 0.2) 0px 1px 2px 0px, rgba(0, 0, 0, 0.05) 0px 0px 0px 1px, rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(255, 255, 255, 0.05) 0px -1px 0px 0px inset`.
- **button-primary-hover:** background #0A30D3, text #FFFFFF on hover.
- **button-outline (“LEARN IN 15 MINUTES”):** #1A1A1A fill, #D9D9D9 text, 16px/700, 1px radius, padding 8px, border 1px solid #505050.
- **button-outline-hover:** background #1D4EFF0F, text #D9D9D9 on hover.
- **button-ghost (“DOWNLOAD FOR FREE”):** #1A1A1A fill, #FFFFFF text, 16px/700, padding 8px 16px 10px 16px, shadow `rgba(0, 0, 0, 0.2) 0px 1px 2px 0px, rgba(0, 0, 0, 0.05) 0px 0px 0px 1px, rgba(255, 255, 255, 0.2) 0px 1px 0px 0px inset, rgba(255, 255, 255, 0.05) 0px -1px 0px 0px inset`.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #0D0D0D for the page and lift surfaces in small steps: #1A1A1A.
- Do keep text in 3 levels: #FFFFFF, #F2F2F2, #D9D9D9.
- Do use #1D4EFF as the brand accent: header, logo and key highlights.
- Do set headlines in PP Fraktion Sans with tight tracking (-0.033em).
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 1px corners on most elements.
- Don't introduce new font families beyond PP Fraktion Sans, Inter and PP Fraktion Mono.
- Don't use #1D4EFF for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.2s, 0.4s.

- **Easing:** `ease`, `cubic-bezier(0, 0.25, 0, 1)`, `cubic-bezier(0.16, 1, 0.3, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/shapr3d.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
