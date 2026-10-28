---
version: alpha
name: Grafana Labs
description: "Light interface measured from grafana.com: Poppins type with Inter, vivid blue accents, tonal surfaces and 8px corners."
colors:
  background: "#F4F4F6"
  surface: "#F4F4F6"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#2E2E38"
  on-surface-muted: "#454554"
  on-surface-subtle: "#67677E"
  surface-container-low: "#EAF0FF"
  surface-container: "#F9F9FA"
  surface-container-high: "#FFFFFF"
  surface-container-highest: "#D0E5C2"
  overlay: "#FFBB6280"
  outline: "#D8D8DF"
  outline-variant: "#BCBCC8"
  primary: "#1B55F5"
  on-primary: "#FFFFFF"
  inverse-surface: "#2B2D32"
  secondary: "#1440E1"
typography:
  headline-display:
    fontFamily: Poppins
    fontSize: 60px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Poppins
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.13
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Poppins
    fontSize: 36px
    fontWeight: 600
    lineHeight: 1.13
  headline-sm:
    fontFamily: Poppins
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.02em
  title-lg:
    fontFamily: Poppins
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.025em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.56
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.38
  label-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.01em
  headline-display-mobile:
    fontFamily: Poppins
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.13
    letterSpacing: -0.025em
  headline-lg-mobile:
    fontFamily: Poppins
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: -0.025em
  headline-md-mobile:
    fontFamily: Poppins
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.13
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  xl: 24px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 64px
  gutter: 8px
  section: 64px
  margin: 16px
  container: 1280px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 7px 14px 9px 14px
    height: 36px
  button-primary-hover:
    backgroundColor: "{colors.secondary}"
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 10px 0px
    height: 44px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 12px 20px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface-subtle}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.lg}"
    padding: 0px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 0px
  card:
    backgroundColor: "{colors.inverse-surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Grafana Labs Design System

## Overview

Grafana Labs describes itself as: “Avoid lock-in and ensure reliability with Grafana Cloud. The AI-powered platform built on open standards unifies metrics, logs, traces, profiles, and business data.” The interface is light, built on **Snow (#F4F4F6)** with **Near Black (#000000)** text, and **Vivid Blue (#1B55F5)** as the main accent.

Type is set in **Poppins** and **Inter**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [grafana.com](https://grafana.com/) on October 21, 2026 at 1440×900 and 390×844 from 402 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles.

- **Snow (#F4F4F6):** Page background, seen 6 times. Token `background`, CSS `--gmui-input`.
- **Near Black (#000000):** Primary text and headings, seen 90 times. Token `on-surface`.
- **Cool Graphite (#2E2E38):** Secondary text, seen 8 times. Token `on-surface-variant`, CSS `--button-secondary-foreground`.
- **Cool Graphite (#454554):** Muted text and metadata, seen 6 times. Token `on-surface-muted`, CSS `--text-body`.
- **Indigo (#67677E):** Subtle text and placeholders, seen 28 times. Token `on-surface-subtle`, CSS `--gmui-color-gray-600`.
- **Pale Blue (#EAF0FF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Snow (#F9F9FA):** Cards and panels, seen 1 time. Token `surface-container`, CSS `--gmui-surface-primary-foreground`.
- **White (#FFFFFF):** Hover and pressed fills, seen 83 times. Token `surface-container-high`, CSS `--gmui-surface-brand-bold-foreground`.
- **Light Green (#D0E5C2):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Orange 50% (#FFBB6280):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Silver (#D8D8DF):** Borders and dividers, seen 3 times. Token `outline`, CSS `--color-gray-300`.
- **Cool Silver (#BCBCC8):** Secondary dividers, seen 2 times. Token `outline-variant`, CSS `--color-gray-400`.
- **Vivid Blue (#1B55F5):** Primary buttons and calls to action, seen 36 times. Token `primary`, CSS `--gmui-text-link`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Cool Graphite (#2B2D32):** High-contrast fills, seen 5 times. Token `inverse-surface`.
- **Vivid Blue (#1440E1):** Most used accent color, seen 3 times. Token `secondary`, CSS `--color-blue-700`.

## Typography

**Poppins** and **Inter** share the interface. Fallback stack: `Poppins, Poppins Fallback`. Other loaded fonts: Poppins Fallback, Inter Fallback.

- **headline-display:** Poppins 60px at weight 600, line height 1.25, tracking -0.025em (48px on mobile). Page title (h1).
- **headline-lg:** Poppins 48px at weight 600, line height 1.13, tracking -0.025em (30px on mobile). Section headings (h2).
- **headline-md:** Poppins 36px at weight 600, line height 1.13 (24px on mobile). Sub-section headings.
- **headline-sm:** Poppins 30px at weight 600, line height 1.25, tracking -0.02em. Card and feature titles.
- **title-lg:** Poppins 24px at weight 600, line height 1.25, tracking -0.025em. Small titles.
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter 18px at weight 600, line height 1.56. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** Inter 16px at weight 600, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 14px at weight 500, line height 1.38. Buttons, navigation and labels.
- **label-sm:** Inter 13px at weight 500, line height 1.5, tracking -0.01em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (74% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2px, sm 8px, md 16px, lg 32px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 1024px, 1700px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, oklab(0 0 0 / 0.05) 0px 0px 0px 1px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **lg (8px):** 116 elements.
- **xl (24px):** 28 elements.
- **md (6px):** 24 elements.
- **sm (4px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #1B55F5 fill, #FFFFFF text, 14px/500, 8px radius, padding 7px 14px 9px 14px, border 1px solid #1B55F5, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`.
- **button-primary-hover:** background #1440E1, text #FFFFFF on hover.
- **button-secondary (“Grafana Cloud AI Assistant”):** #1B55F5 fill, #1B55F5 text, 16px/600, 8px radius, padding 10px 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-outline (“Compare plans”):** #F4F4F6 fill, #2E2E38 text, 18px/600, 8px radius, padding 12px 20px, border 1px solid #F4F4F6, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`.
- **button-ghost (“Learn more”):** transparent fill, #67677E text, 13px/500, 8px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **input-field (“How do I get started with Grafan”):** transparent fill, #000000 text, 14px/400, 6px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **card:** #2B2D32 fill, #000000 text, 16px/400, 24px radius, padding 0px, border 1px solid #2B2D3280.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #F4F4F6 for the page and lift surfaces in small steps: #EAF0FF, #F9F9FA, #FFFFFF, #D0E5C2.
- Do keep text in 4 levels: #000000, #2E2E38, #454554, #67677E.
- Do reserve #1B55F5 for primary actions and key highlights.
- Do set headlines in Poppins with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 16px, 32px).
- Do use 8px corners on most elements; larger surfaces also use 24px, 6px and 4px.
- Don't introduce new font families beyond Poppins and Inter.
- Don't use #1B55F5 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.2s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/grafana.com/), the free DESIGN.md generator.
