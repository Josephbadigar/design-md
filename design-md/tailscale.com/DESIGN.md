---
version: alpha
name: Tailscale
description: "Light interface measured from tailscale.com: inter type with mdio, red accents, tonal surfaces and 8px corners."
colors:
  background: "#F9F7F6"
  surface: "#F9F7F6"
  on-surface: "#2E2D2D"
  on-background: "#2E2D2D"
  on-surface-strong: "#181717"
  on-surface-variant: "#1F1E1E"
  on-surface-muted: "#575555"
  surface-container-low: "#FFFFFF"
  surface-container: "#EEEBEA"
  outline: "#EEEBEA"
  outline-variant: "#1F1E1E1A"
  primary: "#D04841"
  on-primary: "#000000"
  secondary: "#5A82DE"
  tertiary: "#09825D"
typography:
  headline-display:
    fontFamily: inter
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: inter
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
  headline-md:
    fontFamily: inter
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: -0.01em
  label-lg:
    fontFamily: inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.01em
  label-md:
    fontFamily: inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.01em
  label-sm:
    fontFamily: mdio
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0.05em
  headline-display-mobile:
    fontFamily: inter
    fontSize: 37.5px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.01em
rounded:
  sm: 8px
  md: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 64px
  gutter: 8px
  section: 64px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.surface-container-low}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 10px 12px
  link:
    textColor: "{colors.on-surface}"
---

# Tailscale Design System

## Overview

Tailscale describes itself as: “The connectivity platform for devs, IT, and security teams. Zero Trust identity-based access that deploys in minutes and scales to every resource. Start free.” The interface is light, built on **Snow (#F9F7F6)** with **Graphite (#2E2D2D)** text, and **Red (#D04841)** as the main accent.

Type is set in **inter** and **mdio**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 8px.

Measured from [tailscale.com](https://tailscale.com/) on November 4, 2026 at 1440×900 and 390×844 from 345 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **Snow (#F9F7F6):** Page background, seen 1 time. Token `background`.
- **Graphite (#2E2D2D):** Primary text and headings, seen 51 times. Token `on-surface`.
- **Charcoal (#181717):** Headings and emphasis, seen 8 times. Token `on-surface-strong`.
- **Charcoal (#1F1E1E):** Secondary text, seen 8 times. Token `on-surface-variant`.
- **Slate (#575555):** Muted text and metadata, seen 43 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 7 times. Token `surface-container-low`, CSS `--k-consentGate-header-background`.
- **Mist (#EEEBEA):** Cards and panels, seen 4 times. Token `surface-container`, CSS `--color-neutral-300`.
- **Mist (#EEEBEA):** Borders and dividers, seen 17 times. Token `outline`, CSS `--color-neutral-300`.
- **Charcoal 10% (#1F1E1E1A):** Secondary dividers, seen 3 times. Token `outline-variant`.
- **Red (#D04841):** Brand color on large areas, seen 6 times. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Blue (#5A82DE):** Accent, seen 9 times. Token `secondary`.
- **Dark Teal (#09825D):** Accent, seen 6 times. Token `tertiary`, CSS `--color-green-500`.

## Typography

**inter** and **mdio** share the interface. Fallback stack: `inter, inter Fallback, ui-sans-serif, system-ui`.

- **headline-display:** inter 64px at weight 500, line height 1.1, tracking -0.01em (37.5px on mobile). Page title (h1).
- **headline-lg:** inter 48px at weight 500, line height 1.1, tracking -0.01em. Section headings (h2).
- **headline-md:** inter 20px at weight 500, line height 1.2, tracking -0.01em. Sub-section headings.
- **body-md:** inter 16px at weight 400, line height 1.5, tracking -0.01em. Body text.
- **label-lg:** inter 16px at weight 500, line height 1.5, tracking -0.01em. Large buttons and tabs.
- **label-md:** inter 14px at weight 500, line height 1.5, tracking -0.01em. Buttons, navigation and labels.
- **label-sm:** mdio 12px at weight 500, line height 1, tracking 0.05em, uppercase. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (90% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 420px, 480px, 769px, 1024px, 1440px, 1920px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#FFFFFF → #EEEBEA) and #EEEBEA borders.

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 208 elements.
- **md (16px):** 20 elements.
- **full (9999px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started - it’s free!”):** #1F1E1E fill, #FFFFFF text, 16px/500, 8px radius, padding 8px 12px.
- **button-ghost (“Platform”):** transparent fill, #181717 text, 14px/500, 8px radius, padding 10px 12px.
- **link:** transparent fill, #2E2D2D text, padding 0px.

## Do's and Don'ts

- Do use #F9F7F6 for the page and lift surfaces in small steps: #FFFFFF, #EEEBEA.
- Do keep text in 4 levels: #2E2D2D, #181717, #1F1E1E, #575555.
- Do use #D04841 as the brand accent: header, logo and key highlights.
- Do set headlines in inter with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 12px, 20px).
- Do use 8px corners on most elements; larger surfaces also use 16px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond inter and mdio.
- Don't use #D04841 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/tailscale.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
