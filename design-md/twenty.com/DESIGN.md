---
version: alpha
name: Twenty
description: "Light monochrome interface measured from twenty.com: aleo type with hostGrotesk, tonal surfaces and pill-shaped controls."
colors:
  background: "#F4F4F4"
  surface: "#F4F4F4"
  on-surface: "#1C1C1C"
  on-background: "#1C1C1C"
  on-surface-variant: "#333333"
  on-surface-muted: "#666666"
  on-surface-subtle: "#999999"
  surface-container-low: "#EEF4F1"
  surface-container: "#F9F9F9"
  surface-container-high: "#FFFFFF"
  overlay: "#1C1C1C66"
  overlay-strong: "#00000005"
  outline: "#D6D6D6"
  outline-variant: "#D3DFD9"
  primary: "#1C1C1C"
  on-primary: "#FFFFFF"
  secondary: "#FF5F57"
  tertiary: "#3A5BC7"
  error: "#CE2C31"
  warning: "#FEBC2E"
  success: "#28C840"
typography:
  headline-display:
    fontFamily: aleo
    fontSize: 60px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: hostGrotesk
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.17
  headline-md:
    fontFamily: hostGrotesk
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.27
  body-md:
    fontFamily: hostGrotesk
    fontSize: 16px
    fontWeight: 400
  body-lg:
    fontFamily: hostGrotesk
    fontSize: 19px
    fontWeight: 700
  body-sm:
    fontFamily: hostGrotesk
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.55
  label-lg:
    fontFamily: hostGrotesk
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.35
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1
  label-sm:
    fontFamily: hostGrotesk
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.55
  code:
    fontFamily: azeretMono
    fontSize: 12px
    fontWeight: 500
  headline-display-mobile:
    fontFamily: aleo
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: -0.02em
  headline-md-mobile:
    fontFamily: hostGrotesk
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.33
rounded:
  sm: 2px
  md: 4px
  lg: 6px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 64px
  gutter: 8px
  section: 64px
components:
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#2F7468"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 4px 8px
    height: 24px
  button-outline-hover:
    backgroundColor: "#E3EDE7"
  button-ghost:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "#09090BEB"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px 8px
    height: 24px
  link:
    textColor: "{colors.primary}"
---

# Twenty Design System

## Overview

Twenty describes itself as: “The #1 Open Source CRM for modern teams. Modular, scalable, and built to fit your business.” The interface is light, built on **Snow (#F4F4F4)** with **Charcoal (#1C1C1C)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **aleo** and **hostGrotesk**, with **azeretMono** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [twenty.com](https://twenty.com/) on October 21, 2026 at 1440×900 and 390×844 from 344 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 19 roles.

- **Snow (#F4F4F4):** Page background, seen 5 times. Token `background`, CSS `--color-neutral`.
- **Charcoal (#1C1C1C):** Primary text and headings, seen 42 times. Token `on-surface`, CSS `--ink`.
- **Graphite (#333333):** Secondary text, seen 21 times. Token `on-surface-variant`.
- **Slate (#666666):** Muted text and metadata, seen 13 times. Token `on-surface-muted`.
- **Gray (#999999):** Subtle text and placeholders, seen 14 times. Token `on-surface-subtle`.
- **Mist (#EEF4F1):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Snow (#F9F9F9):** Cards and panels, seen 1 time. Token `surface-container`.
- **White (#FFFFFF):** Hover and pressed fills, seen 6 times. Token `surface-container-high`, CSS `--color-white`.
- **Charcoal 40% (#1C1C1C66):** Translucent fill for cards and controls, seen 4 times. Token `overlay`, CSS `--divider`.
- **Near Black 2% (#00000005):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Silver (#D6D6D6):** Borders and dividers, seen 3 times. Token `outline`.
- **Silver (#D3DFD9):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Charcoal (#1C1C1C):** Primary actions (the main text color; the palette is monochrome), seen 67 times. Token `primary`, CSS `--ink`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Red (#FF5F57):** Most used accent color, seen 3 times. Token `secondary`.
- **Blue (#3A5BC7):** Accent, seen 4 times. Token `tertiary`.
- **Red (#CE2C31):** Errors and destructive states, seen 5 times. Token `error`.
- **Vivid Amber (#FEBC2E):** Warnings and highlights, seen 2 times. Token `warning`.
- **Green (#28C840):** Success and positive states, seen 2 times. Token `success`.

## Typography

**aleo**, **hostGrotesk**, **Inter** and **azeretMono** (monospace) share the interface. Fallback stack: `aleo, aleo Fallback, serif`. Other loaded fonts: hostGrotesk Fallback, inter.

- **headline-display:** aleo 60px at weight 300, line height 1.1, tracking -0.02em (40px on mobile). Page title (h1).
- **headline-lg:** hostGrotesk 48px at weight 300, line height 1.17. Section headings (h2).
- **headline-md:** hostGrotesk 22px at weight 500, line height 1.27 (18px on mobile). Sub-section headings.
- **body-md:** hostGrotesk 16px at weight 400. Body text.
- **body-lg:** hostGrotesk 19px at weight 700. Lead paragraphs.
- **body-sm:** hostGrotesk 12px at weight 400, line height 1.55. Secondary and small text.
- **label-lg:** hostGrotesk 16px at weight 500, line height 1.35. Large buttons and tabs.
- **label-md:** Inter 13px at weight 500, line height 1. Buttons, navigation and labels.
- **label-sm:** hostGrotesk 12px at weight 500, line height 1.55. Small labels and badges.
- **code:** azeretMono 12px at weight 500. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (87% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 64px.
- **Sections:** 64px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 921px, 1281px, 1350px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.04) 0px 0px 1px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`
- `rgba(0, 0, 0, 0.04) 0px 0px 0px 1px, rgba(0, 0, 0, 0.12) 0px 1px 2px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (4px):** 76 elements.
- **full (9999px):** 40 elements.
- **sm (2px):** 28 elements.
- **lg (6px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-outline (“~/code/my-twenty-app”):** #EEF4F1 fill, #2F7468 text, 13px/500, 4px radius, padding 4px 8px, border 1px solid #D3DFD9.
- **button-outline-hover:** background #E3EDE7, text #2F7468 on hover.
- **button-ghost (“AI Chat”):** #FFFFFF fill, #09090BEB text, 13px/500, 6px radius, padding 0px 8px, border 1px solid #09090B0F, shadow `rgba(0, 0, 0, 0.04) 0px 0px 1px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`.
- **link:** transparent fill, #1C1C1C text, padding 0px.

## Do's and Don'ts

- Do use #F4F4F4 for the page and lift surfaces in small steps: #EEF4F1, #F9F9F9, #FFFFFF.
- Do keep text in 4 levels: #1C1C1C, #333333, #666666, #999999.
- Do let contrast carry emphasis; primary actions use #1C1C1C on #F4F4F4.
- Do set headlines in aleo with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't use #999999 for body text; it reaches 2.6:1 on #F4F4F4. Keep it for large text or metadata.
- Don't introduce new font families beyond aleo, hostGrotesk, Inter and azeretMono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.00001s.

## Motion

Interface transitions are quick: 1e-05s.

- **Easing:** `ease`, `cubic-bezier(0.16, 1, 0.3, 1)`, `ease-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/twenty.com/), the free DESIGN.md generator.
