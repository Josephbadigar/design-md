---
version: alpha
name: Miro
description: "Light interface measured from miro.com: Apris Regular type with Roobert PRO Regular, amber accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#1C1C1E"
  on-surface-muted: "#555A6A"
  on-surface-subtle: "#666666"
  surface-container-low: "#FBFAF7"
  surface-container: "#FDE0F0"
  outline: "#C7CAD5"
  outline-variant: "#E9EAEF"
  primary: "#FDE050"
  on-primary: "#1C1C1E"
  secondary: "#0000EE"
  tertiary: "#FFDD33"
typography:
  headline-display:
    fontFamily: Apris Regular
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.1
  headline-lg:
    fontFamily: Roobert PRO Regular
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.15
  headline-md:
    fontFamily: Roobert PRO Regular
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.19
  headline-sm:
    fontFamily: Roobert PRO Regular
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.5
  body-md:
    fontFamily: Roobert PRO Regular
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Roobert PRO Medium
    fontSize: 18px
    fontWeight: 400
    letterSpacing: 0.01em
  body-sm:
    fontFamily: sans-serif
    fontSize: 12px
    fontWeight: 400
  label-md:
    fontFamily: Noto Sans
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: -0.01em
  label-sm:
    fontFamily: Roobert PRO SemiBold
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.6
  headline-display-mobile:
    fontFamily: Apris Regular
    fontSize: 34px
    fontWeight: 400
    lineHeight: 1.1
rounded:
  sm: 8px
  md: 20px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 28px
  xl: 48px
  gutter: 8px
  margin: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 40px
  button-secondary:
    textColor: "{colors.background}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 1px 6px
    height: 48px
  button-tertiary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.background}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 16px
  link:
    textColor: "{colors.secondary}"
---

# Miro Design System

## Overview

Miro describes itself as: “Speed up product development from ideation to launch. Align teams, break tool silos, and ship what customers need in one AI-powered visual platform.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Amber (#FDE050)** as the main accent.

Type is set in **Apris Regular** and **Roobert PRO Regular**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 8px.

Measured from [miro.com](https://miro.com/) on October 29, 2026 at 1440×900 and 390×844 from 366 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 1 time. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 21 times. Token `on-surface`.
- **Charcoal (#1C1C1E):** Secondary text, seen 31 times. Token `on-surface-variant`.
- **Dark Blue (#555A6A):** Muted text and metadata, seen 7 times. Token `on-surface-muted`, CSS `--tw-color-input-active`.
- **Slate (#666666):** Subtle text and placeholders, seen 8 times. Token `on-surface-subtle`.
- **Snow (#FBFAF7):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Pale Pink (#FDE0F0):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--tw-color-pink`.
- **Cool Silver (#C7CAD5):** Borders and dividers, seen 1 time. Token `outline`.
- **Cool Mist (#E9EAEF):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--tw-color-gray-150`.
- **Amber (#FDE050):** Primary buttons and calls to action, seen 2 times. Token `primary`.
- **Charcoal (#1C1C1E):** Text and icons on primary. Token `on-primary`.
- **Vivid Indigo (#0000EE):** Links and interactive text, seen 78 times. Token `secondary`.
- **Vivid Amber (#FFDD33):** Accent in the logo, seen 2 times. Token `tertiary`.

## Typography

**Apris Regular**, **Roobert PRO Regular**, **Roobert PRO Medium**, **sans-serif**, **Noto Sans** and **Roobert PRO SemiBold** share the interface. Fallback stack: `Apris Regular, Apris Regular Placeholder, sans-serif`.

- **headline-display:** Apris Regular 48px at weight 400, line height 1.1 (34px on mobile). Page title (h1).
- **headline-lg:** Roobert PRO Regular 36px at weight 400, line height 1.15. Section headings (h2).
- **headline-md:** Roobert PRO Regular 24px at weight 400, line height 1.19. Sub-section headings.
- **headline-sm:** Roobert PRO Regular 20px at weight 400, line height 1.5. Card and feature titles.
- **body-md:** Roobert PRO Regular 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Roobert PRO Medium 18px at weight 400, tracking 0.01em. Lead paragraphs.
- **body-sm:** sans-serif 12px at weight 400. Secondary and small text.
- **label-md:** Noto Sans 16px at weight 600, line height 1.5, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** Roobert PRO SemiBold 14px at weight 600, line height 1.6. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 67% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 28px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 390px, 576px, 639.98px, 640px, 768px, 809px, 809.98px, 810px, 992px, 1024px, 1199px, 1200px, 1279.98px, 1280px, 1366px, 1400px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FBFAF7 → #FDE0F0) and #C7CAD5 borders.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 72 elements.
- **md (20px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“See here why we rebuilt Miro →”):** #FDE050 fill, #1C1C1E text, 16px/900, 8px radius, padding 8px 12px.
- **button-secondary (“Get Started Free”):** transparent fill, #FFFFFF text, 16px/600, 8px radius, padding 1px 6px.
- **button-tertiary (“Get started free”):** #1C1C1E fill, #FFFFFF text, 14px/600, 8px radius, padding 8px 12px.
- **button-ghost (“Product”):** transparent fill, #1C1C1E text, 14px/500, 8px radius, padding 8px 12px.
- **input-field (“Enter your work email”):** #FFFFFF fill, #1C1C1E text, 16px/400, 8px radius, padding 16px, border 1px solid #E9EAEF.
- **link:** transparent fill, #0000EE text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FBFAF7, #FDE0F0.
- Do keep text in 4 levels: #000000, #1C1C1E, #555A6A, #666666.
- Do reserve #FDE050 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 10px, 28px).
- Do use 8px corners on most elements; larger surfaces also use 20px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Apris Regular, Roobert PRO Regular, Roobert PRO Medium, sans-serif, Noto Sans and Roobert PRO SemiBold.
- Don't use #FDE050 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.15s, 0.6s, 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.16, 1, 0.3, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/miro.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
