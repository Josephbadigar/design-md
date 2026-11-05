---
version: alpha
name: Cohere
description: "Light monochrome interface measured from cohere.com: CohereText type with Unica77 Cohere Web, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#17171C"
  on-surface-muted: "#212121"
  on-surface-subtle: "#73738A"
  surface-container-low: "#F0EEE9"
  primary: "#17171C"
  on-primary: "#FFFFFF"
  secondary: "#00AA28"
typography:
  headline-display:
    fontFamily: CohereText
    fontSize: 96px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: CohereText
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Unica77 Cohere Web
    fontSize: 48px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Unica77 Cohere Web
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.3
  body-md:
    fontFamily: Unica77 Cohere Web
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: Unica77 Cohere Web
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Unica77 Cohere Web
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: Unica77 Cohere Web
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Unica77 Cohere Web
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.4
  code:
    fontFamily: CohereMono
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.02em
  headline-display-mobile:
    fontFamily: CohereText
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: CohereText
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  headline-md-mobile:
    fontFamily: Unica77 Cohere Web
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  sm: 4px
  md: 8px
  lg: 22px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 40px
  gutter: 8px
  section: 80px
  margin: 40px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px 16px
    height: 36px
  button-primary-hover:
    backgroundColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
    height: 53px
  button-outline-hover:
    textColor: "{colors.on-surface}"
  button-ghost:
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label-md}"
    rounded: 0px
    padding: 6px 0px
  link:
    textColor: "{colors.on-surface}"
---

# Cohere Design System

## Overview

Cohere describes itself as: “Cohere builds powerful models and AI solutions enabling enterprises to automate processes, empower employees, and turn fragmented data into actionable insights.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **CohereText** and **Unica77 Cohere Web**, with **CohereMono** for code. Headlines run large with tight negative tracking; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [cohere.com](https://cohere.com/) on November 4, 2026 at 1440×900 and 390×844 from 422 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background, seen 5 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Near Black (#000000):** Primary text and headings, seen 35 times. Token `on-surface`.
- **Charcoal (#17171C):** Secondary text, seen 22 times. Token `on-surface-variant`.
- **Charcoal (#212121):** Muted text and metadata, seen 13 times. Token `on-surface-muted`, CSS `--volcanic`.
- **Cool Slate (#73738A):** Subtle text and placeholders, seen 17 times. Token `on-surface-subtle`.
- **Warm Mist (#F0EEE9):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Charcoal (#17171C):** Primary buttons and calls to action, seen 30 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Green (#00AA28):** Accent, seen 3 times. Token `secondary`.

## Typography

**CohereText**, **Unica77 Cohere Web** and **CohereMono** (monospace) share the interface. Fallback stack: `CohereText, Space Grotesk, Inter, ui-sans-serif`. Other loaded fonts: CohereIconDefault, CohereIconOutline.

- **headline-display:** CohereText 96px at weight 400, line height 1, tracking -0.02em (60px on mobile). Page title (h1).
- **headline-lg:** CohereText 60px at weight 400, line height 1, tracking -0.02em (32px on mobile). Section headings (h2).
- **headline-md:** Unica77 Cohere Web 48px at weight 400, line height 1.2, tracking -0.01em (28px on mobile). Sub-section headings.
- **headline-sm:** Unica77 Cohere Web 24px at weight 400, line height 1.3. Card and feature titles.
- **body-md:** Unica77 Cohere Web 14px at weight 400, line height 1.4. Body text.
- **body-lg:** Unica77 Cohere Web 18px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** Unica77 Cohere Web 12px at weight 400, line height 1.4. Secondary and small text.
- **label-md:** Unica77 Cohere Web 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Unica77 Cohere Web 12px at weight 500, line height 1.4. Small labels and badges.
- **code:** CohereMono 14px at weight 400, line height 1.4, tracking 0.02em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (85% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 40px.
- **Sections:** 80px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 40px on each side of full-width sections.
- **Breakpoints:** 336px, 410px, 425px, 440px, 460px, 510px, 550px, 640px, 675px, 767px, 768px, 1023px, 1024px, 1280px, 1440px, 1536px, 2560px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F0EEE9).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 48 elements.
- **sm (4px):** 12 elements.
- **md (8px):** 12 elements.
- **lg (22px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Request a demo”):** #17171C fill, #FFFFFF text, 16px/400, 9999px radius, padding 0px 16px.
- **button-primary-hover:** background #000000, text #FFFFFF on hover.
- **button-outline (“Explore now”):** #FFFFFF fill, #17171C text, 16px/400, 9999px radius, padding 12px 24px.
- **button-outline-hover:** background #FFFFFF, text #000000 on hover.
- **button-ghost (“Sign in”):** transparent fill, #212121 text, 16px/400, padding 6px 0px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F0EEE9.
- Do keep text in 4 levels: #000000, #17171C, #212121, #73738A.
- Do let contrast carry emphasis; primary actions use #17171C on #FFFFFF.
- Do set headlines in CohereText with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond CohereText, Unica77 Cohere Web and CohereMono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.3s, 0.15s, 0.2s. Longer ambient animations run 0.8s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cohere.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
