---
version: alpha
name: Railway
description: "Dark interface measured from railway.com: IBM Plex Serif type with Inter, violet accents, tonal surfaces and 4px corners."
colors:
  background: "#13111C"
  surface: "#13111C"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F7F7F8"
  on-surface-muted: "#DCDCE0"
  on-surface-subtle: "#A1A0AB"
  surface-container-low: "#1C1A28"
  surface-container: "#291839"
  overlay: "#00000059"
  overlay-strong: "#FFFFFF1A"
  outline: "#FFFFFF26"
  outline-variant: "#FFFFFF1A"
  primary: "#553F83"
  on-primary: "#FFFFFF"
  secondary: "#F9A8D4"
  tertiary: "#183367"
typography:
  headline-display:
    fontFamily: IBM Plex Serif
    fontSize: 54px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.036em
  headline-lg:
    fontFamily: IBM Plex Serif
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.02em
  headline-md:
    fontFamily: IBM Plex Serif
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: -0.005em
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.63
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: IBM Plex Serif
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.049em
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 48px
  gutter: 32px
  section: 96px
  margin: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
    padding: 12px 24px
    height: 58px
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "#BF93EC"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px
    height: 32px
  button-ghost:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 12px 24px
    height: 58px
  link:
    textColor: "{colors.on-surface}"
---

# Railway Design System

## Overview

Railway describes itself as: “Railway is a full-stack cloud for deploying web apps, servers, databases, and more with automatic scaling, monitoring, and security.” The interface is dark, built on **Cool Charcoal (#13111C)** with **White (#FFFFFF)** text, and **Violet (#553F83)** as the main accent.

Type is set in **IBM Plex Serif** and **Inter**. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Corners are mostly 4px.

Measured from [railway.com](https://railway.com/) on October 29, 2026 at 1440×900 and 390×844 from 374 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **Cool Charcoal (#13111C):** Page background, seen 2 times. Token `background`, CSS `--osano-toggle-on-thumb-color`.
- **White (#FFFFFF):** Primary text and headings, seen 18 times. Token `on-surface`, CSS `--osano-button-reject-all-foreground-color`.
- **Snow (#F7F7F8):** Secondary text, seen 11 times. Token `on-surface-variant`, CSS `--gray-950`.
- **Silver (#DCDCE0):** Muted text and metadata, seen 5 times. Token `on-surface-muted`.
- **Cool Gray (#A1A0AB):** Subtle text and placeholders, seen 41 times. Token `on-surface-subtle`, CSS `--gray-600`.
- **Cool Charcoal (#1C1A28):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`, CSS `--gray-50`.
- **Deep Violet (#291839):** Cards and panels, seen 1 time. Token `surface-container`.
- **Near Black 35% (#00000059):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 10% (#FFFFFF1A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **White 15% (#FFFFFF26):** Borders and dividers, seen 2 times. Token `outline`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Violet (#553F83):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Pink (#F9A8D4):** Accent in text, fills and borders, seen 12 times. Token `secondary`.
- **Dark Blue (#183367):** Accent on large areas. Token `tertiary`.

## Typography

**IBM Plex Serif** and **Inter** share the interface. Fallback stack: `IBM Plex Serif, Georgia, Cambria, Times New Roman`. Other loaded fonts: Inter Tight, JetBrains Mono.

- **headline-display:** IBM Plex Serif 54px at weight 500, line height 1.12, tracking -0.036em (40px on mobile). Page title (h1).
- **headline-lg:** IBM Plex Serif 40px at weight 400, line height 1.2, tracking -0.02em. Section headings (h2).
- **headline-md:** IBM Plex Serif 36px at weight 400, line height 1.33, tracking -0.02em. Sub-section headings.
- **body-md:** Inter 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Inter 18px at weight 500, line height 1.6, tracking -0.005em. Lead paragraphs.
- **label-md:** Inter 16px at weight 400, line height 1.63. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1.43. Small labels and badges.

## Layout

Spacing follows a 4px grid: 93% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 32px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 32px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 376px, 768px, 1200px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#1C1A28 → #291839) and #FFFFFF26 borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 270 elements.
- **md (6px):** 28 elements.
- **lg (8px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Deploy →”):** #553F83 fill, #FFFFFF text, 20px/500, 8px radius, padding 12px 24px, border 1px solid #FFFFFF26.
- **button-outline (“Network”):** #291839 fill, #BF93EC text, 16px/400, 8px radius, padding 0px.
- **button-ghost (“Agents”):** #00000059 fill, #FFFFFF text, 20px/500, 8px radius, padding 12px 24px, border 1px solid #FFFFFF40.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #13111C for the page and lift surfaces in small steps: #1C1A28, #291839.
- Do keep text in 4 levels: #FFFFFF, #F7F7F8, #DCDCE0, #A1A0AB.
- Do reserve #553F83 for primary actions and key highlights.
- Do set headlines in IBM Plex Serif with tight tracking (-0.036em).
- Do keep spacing on the 4px grid.
- Do use 4px corners on most elements; larger surfaces also use 6px and 8px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond IBM Plex Serif and Inter.
- Don't use #553F83 for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/railway.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
