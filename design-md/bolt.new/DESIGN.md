---
version: alpha
name: bolt.new
description: "Dark interface measured from bolt.new: Schibsted Grotesk type with Silkscreen, vivid blue accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#111114"
  surface: "#111114"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#F9F6F9"
  on-surface-muted: "#D6D5DE"
  on-surface-subtle: "#B8B8B9"
  surface-container-low: "#171719"
  surface-container: "#000000"
  surface-container-high: "#1E1E21"
  overlay: "#10141C8C"
  overlay-strong: "#FFFFFF0F"
  outline: "#96BEFF29"
  outline-variant: "#3C3C41"
  primary: "#2BA6FF"
  on-primary: "#FFFFFF"
  inverse-surface: "#A4A3AC"
  secondary: "#1488FC"
  tertiary: "#0258C7"
typography:
  headline-display:
    fontFamily: Schibsted Grotesk
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Schibsted Grotesk
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: 0.01em
  body-md:
    fontFamily: Schibsted Grotesk
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Schibsted Grotesk
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.56
    letterSpacing: 0.01em
  body-sm:
    fontFamily: Schibsted Grotesk
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
    letterSpacing: 0.01em
  caption:
    fontFamily: Schibsted Grotesk
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
    letterSpacing: 0.01em
  label-lg:
    fontFamily: Schibsted Grotesk
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.57
    letterSpacing: 0.01em
  label-md:
    fontFamily: Schibsted Grotesk
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.33
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Silkscreen
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.136em
  headline-display-mobile:
    fontFamily: Schibsted Grotesk
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
    letterSpacing: -0.025em
  headline-lg-mobile:
    fontFamily: Schibsted Grotesk
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.56
    letterSpacing: 0.01em
rounded:
  xs: 2px
  sm: 4px
  md: 6px
  lg: 12px
  xl: 16px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 18px
  xl: 40px
  gutter: 8px
  section: 120px
  margin: 72px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 36px
  button-outline:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 0px 8px
    height: 28px
  button-outline-hover:
    backgroundColor: "#2BA6FF29"
    textColor: "{colors.on-surface-variant}"
  button-secondary:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xs}"
    padding: 0px 18px
    height: 38px
  button-ghost:
    textColor: "#FFFFFFBF"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: 8px 14px
  link:
    textColor: "{colors.on-surface-subtle}"
---

# bolt.new Design System

## Overview

bolt.new describes itself as: “Build and scale high-performing websites & apps using your words. Join millions and start building today.” The interface is dark, built on **Charcoal (#111114)** with **White (#FFFFFF)** text, and **Vivid Blue (#2BA6FF)** as the main accent.

Type is set in **Schibsted Grotesk** and **Silkscreen**. Headlines run large with tight negative tracking; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Controls are pill-shaped.

Measured from [bolt.new](https://bolt.new/) on October 21, 2026 at 1440×900 and 390×844 from 212 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles.

- **Charcoal (#111114):** Page background, seen 4 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 4 times. Token `on-surface`.
- **Snow (#F9F6F9):** Secondary text, seen 15 times. Token `on-surface-variant`, CSS `--cm-textColor`.
- **Cool Silver (#D6D5DE):** Muted text and metadata, seen 9 times. Token `on-surface-muted`, CSS `--cm-search-button-textColor`.
- **Silver (#B8B8B9):** Subtle text and placeholders, seen 16 times. Token `on-surface-subtle`.
- **Charcoal (#171719):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--cm-gutter-backgroundColor`.
- **Near Black (#000000):** Cards and panels, seen 2 times. Token `surface-container`.
- **Charcoal (#1E1E21):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Cool Charcoal 55% (#10141C8C):** Translucent fill for cards and controls, seen 7 times. Token `overlay`.
- **White 6% (#FFFFFF0F):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Light Blue 16% (#96BEFF29):** Borders and dividers, seen 7 times. Token `outline`.
- **Graphite (#3C3C41):** Secondary dividers, seen 3 times. Token `outline-variant`, CSS `--cm-panels-borderColor`.
- **Vivid Blue (#2BA6FF):** Primary buttons and calls to action, seen 2 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Cool Gray (#A4A3AC):** High-contrast fills, seen 29 times. Token `inverse-surface`.
- **Vivid Blue (#1488FC):** Secondary buttons, seen 31 times. Token `secondary`, CSS `--cm-selection-backgroundColorFocused`.
- **Blue (#0258C7):** Brand color in logos and imagery, seen 22 times. Token `tertiary`.

## Typography

**Schibsted Grotesk** and **Silkscreen** share the interface. Fallback stack: `Schibsted Grotesk, Inter, -apple-system, BlinkMacSystemFont`.

- **headline-display:** Schibsted Grotesk 48px at weight 600, line height 1.2, tracking -0.025em (24px on mobile). Page title (h1).
- **headline-lg:** Schibsted Grotesk 20px at weight 600, line height 1.4, tracking 0.01em (18px on mobile). Section headings (h2).
- **body-md:** Schibsted Grotesk 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Schibsted Grotesk 18px at weight 600, line height 1.56, tracking 0.01em. Lead paragraphs.
- **body-sm:** Schibsted Grotesk 14px at weight 400, line height 1.57, tracking 0.01em. Secondary and small text.
- **caption:** Schibsted Grotesk 12px at weight 400, line height 1.33, tracking 0.01em. Captions and fine print.
- **label-lg:** Schibsted Grotesk 14px at weight 500, line height 1.57, tracking 0.01em. Large buttons and tabs.
- **label-md:** Schibsted Grotesk 12px at weight 500, line height 1.33, tracking 0.01em. Buttons, navigation and labels.
- **label-sm:** Silkscreen 11px at weight 400, line height 1.5, tracking 0.136em, uppercase. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 56% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 18px, xl 40px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 72px on each side of full-width sections.
- **Breakpoints:** 480px, 600px, 639.9px, 640px, 767.9px, 768px, 900px, 1024px, 1100px, 1130px, 1280px, 1536px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#171719 → #000000 → #1E1E21):

- `rgba(255, 255, 255, 0.05) 0px 1px 0px 0px inset`

A few raised panels add a soft drop shadow: `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px`.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 60 elements.
- **md (6px):** 20 elements.
- **sm (4px):** 16 elements.
- **lg (12px):** 16 elements.
- **xl (16px):** 8 elements.
- **xs (2px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Build now”):** #2BA6FF fill, #FFFFFF text, 14px/500, 9999px radius, padding 0px 16px.
- **button-outline (“Figma”):** #10141C8C fill, #D6D5DE text, 14px/500, 9999px radius, padding 0px 8px, border 1px solid #96BEFF29, shadow `rgba(255, 255, 255, 0.05) 0px 1px 0px 0px inset`.
- **button-outline-hover:** background #2BA6FF29, text #F9F6F9 on hover.
- **button-secondary (“Get Started Get Started”):** #1488FC fill, #FFFFFF text, 14px/600, 2px radius, padding 0px 18px.
- **button-ghost (“Solutions”):** transparent fill, #FFFFFFBF text, 14px/500, 4px radius, padding 8px 14px.
- **link:** transparent fill, #FFFFFFB3 text, padding 0px.

## Do's and Don'ts

- Do use #111114 for the page and lift surfaces in small steps: #171719, #000000, #1E1E21.
- Do keep text in 4 levels: #FFFFFF, #F9F6F9, #D6D5DE, #B8B8B9.
- Do reserve #2BA6FF for primary actions and key highlights.
- Do set headlines in Schibsted Grotesk with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 10px, 18px).
- Do make buttons and chips fully rounded (9999px); most other elements use 6px corners.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond Schibsted Grotesk and Silkscreen.
- Don't use #2BA6FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.45s.

## Motion

Interface transitions are quick: 0.18s, 0.15s, 0.2s, 0.45s.

- **Easing:** `ease`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0.165, 0.84, 0.44, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/bolt.new/), the free DESIGN.md generator.
