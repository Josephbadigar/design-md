---
version: alpha
name: Storybook
description: "Dark monochrome interface measured from storybook.js.org: Nunito Sans type, tonal surfaces and pill-shaped controls."
colors:
  background: "#0D1026"
  surface: "#0D1026"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#94A3B8"
  on-surface-muted: "#9E9FA8"
  surface-container-low: "#0F172A"
  surface-container: "#020617"
  surface-container-high: "#000000"
  surface-container-highest: "#333333"
  overlay: "#00000080"
  overlay-strong: "#FFFFFF1A"
  outline: "#3F3F46"
  outline-variant: "#52525B"
  primary: "#FFFFFF"
  on-primary: "#000000"
  secondary: "#029CFD"
  tertiary: "#FF4785"
  warning: "#FFAE00"
  error: "#EF4444"
typography:
  headline-display:
    fontFamily: Nunito Sans
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.25
  headline-lg:
    fontFamily: Nunito Sans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.33
  body-md:
    fontFamily: Nunito Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  label-lg:
    fontFamily: Nunito Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Nunito Sans
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.43
  label-sm:
    fontFamily: Nunito Sans
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1.33
  headline-display-mobile:
    fontFamily: Nunito Sans
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.11
rounded:
  sm: 2px
  md: 4px
  lg: 6px
  xl: 8px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 40px
  gutter: 8px
  section: 112px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 0px 12px
    height: 32px
  button-secondary:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 6px 12px
    height: 30px
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 0px 24px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.full}"
    padding: 0px 12px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 100px 0px 16px
  link:
    textColor: "{colors.primary}"
---

# Storybook Design System

## Overview

Storybook describes itself as: “Storybook is a frontend workshop for building UI components and pages in isolation. Thousands of teams use it for UI development, testing, and documentation. It's open source and free.” The interface is dark, built on **Deep Indigo (#0D1026)** with **White (#FFFFFF)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Nunito Sans**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [storybook.js.org](https://storybook.js.org/) on October 21, 2026 at 1440×900 and 390×844 from 270 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 18 roles, plus gradient stops #4791FF, #FF4785.

- **Deep Indigo (#0D1026):** Page background. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 56 times. Token `on-surface`, CSS `--docsearch-footer-background`.
- **Blue (#94A3B8):** Secondary text, seen 12 times. Token `on-surface-variant`.
- **Cool Gray (#9E9FA8):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Deep Blue (#0F172A):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Deep Indigo (#020617):** Cards and panels, seen 1 time. Token `surface-container`.
- **Near Black (#000000):** Hover and pressed fills, seen 2 times. Token `surface-container-high`.
- **Graphite (#333333):** Highest raised elements, seen 1 time. Token `surface-container-highest`.
- **Near Black 50% (#00000080):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **White 10% (#FFFFFF1A):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Cool Graphite (#3F3F46):** Borders and dividers, seen 12 times. Token `outline`.
- **Cool Slate (#52525B):** Secondary dividers, seen 8 times. Token `outline-variant`.
- **White (#FFFFFF):** Primary buttons and calls to action, seen 82 times. Token `primary`, CSS `--docsearch-footer-background`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#029CFD):** Most used accent color, seen 17 times. Token `secondary`.
- **Pink (#FF4785):** Brand color in the logo, seen 15 times. Token `tertiary`.
- **Vivid Amber (#FFAE00):** Warnings and highlights, seen 4 times. Token `warning`.
- **Vivid Red (#EF4444):** Errors and destructive states, seen 2 times. Token `error`.

## Typography

**Nunito Sans** carries the whole interface. Fallback stack: `__Nunito_Sans_ee04dc`. Other loaded fonts: __Nunito_Sans_ee04dc.

- **headline-display:** Nunito Sans 56px at weight 700, line height 1.25 (36px on mobile). Page title (h1).
- **headline-lg:** Nunito Sans 24px at weight 700, line height 1.33. Section headings (h2).
- **body-md:** Nunito Sans 14px at weight 400, line height 1.43. Body text.
- **label-lg:** Nunito Sans 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** Nunito Sans 14px at weight 700, line height 1.43. Buttons, navigation and labels.
- **label-sm:** Nunito Sans 12px at weight 700, line height 1.33. Small labels and badges.

## Layout

Spacing follows a 4px grid: 98% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 40px.
- **Sections:** 112px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 360px, 430px, 440px, 600px, 640px, 768px, 920px, 940px, 960px, 1024px, 1040px, 1120px, 1280px, 1416px, 1440px, 1536px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 4px 6px -1px, rgba(0, 0, 0, 0.1) 0px 2px 4px -2px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 80 elements.
- **md (4px):** 76 elements.
- **lg (6px):** 64 elements.
- **sm (2px):** 36 elements.
- **xl (8px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #FFFFFF fill, #000000 text, 16px/400, 9999px radius, padding 0px 12px.
- **button-secondary (“Introducing MCP for React”):** transparent fill, #FFFFFF text, 12px/400, 9999px radius, padding 6px 12px.
- **button-outline (“npm create storybook@latest”):** transparent fill, #FFFFFF text, 16px/700, 9999px radius, padding 0px 24px, border 1px solid #FFFFFF.
- **button-ghost (“Search docs K”):** transparent fill, #FFFFFF text, 16px/500, 9999px radius, padding 0px 12px, border 1px solid #FFFFFF4D.
- **input-field (“you@domain.com”):** #0F172A fill, #FFFFFF text, 16px/400, 6px radius, padding 0px 100px 0px 16px, border 1px solid #334155.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #0D1026 for the page and lift surfaces in small steps: #0F172A, #020617, #000000, #333333.
- Do keep text in 3 levels: #FFFFFF, #94A3B8, #9E9FA8.
- Do let contrast carry emphasis; primary actions use #FFFFFF on #0D1026.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't introduce new font families beyond Nunito Sans.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s. Longer ambient animations run 8s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/storybook.js.org/), the free DESIGN.md generator.
