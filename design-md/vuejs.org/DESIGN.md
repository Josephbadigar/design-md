---
version: alpha
name: Vue.js
description: "Light interface measured from vuejs.org: Inter var experimental type, teal accents, tonal surfaces and 2px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#213547"
  on-background: "#213547"
  on-surface-variant: "#476582"
  on-surface-muted: "#767676"
  surface-container-low: "#F9F9F9"
  surface-container: "#F1F1F1"
  outline: "#3C3C3C54"
  outline-variant: "#3C3C3C4A"
  primary: "#33A06F"
  on-primary: "#000000"
  secondary: "#42B883"
typography:
  headline-display:
    fontFamily: Inter var experimental
    fontSize: 76px
    fontWeight: 900
    lineHeight: 1.25
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter var experimental
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: Inter var experimental
    fontSize: 14.5px
    fontWeight: 400
    lineHeight: 1.67
    letterSpacing: 0.014em
  body-lg:
    fontFamily: Inter var experimental
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0.013em
  body-sm:
    fontFamily: Inter var experimental
    fontSize: 11px
    fontWeight: 400
    lineHeight: 2.18
    letterSpacing: 0.018em
  label-lg:
    fontFamily: Inter var experimental
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.013em
  label-md:
    fontFamily: Inter var experimental
    fontSize: 13px
    fontWeight: 500
    letterSpacing: 0.015em
  label-sm:
    fontFamily: Inter var experimental
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.67
    letterSpacing: 0.017em
  headline-display-mobile:
    fontFamily: Inter var experimental
    fontSize: 48px
    fontWeight: 900
    lineHeight: 1.25
    letterSpacing: -0.01em
rounded:
  sm: 2px
  md: 8px
  full: 9999px
spacing:
  xs: 2px
  sm: 8px
  md: 12px
  lg: 18px
  xl: 42px
  section: 96px
  margin: 32px
  container: 960px
components:
  button-primary:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 18px
    height: 44px
  button-primary-hover:
    backgroundColor: "#E5E5E5"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 8px 18px
    height: 40px
  button-outline-hover:
    backgroundColor: "#E5E5E5"
  button-ghost:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.outline}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 0px
    height: 84px
  link:
    textColor: "{colors.on-surface}"
---

# Vue.js Design System

## Overview

Vue.js describes itself as: “Vue.js - The Progressive JavaScript Framework” The interface is light, built on **White (#FFFFFF)** with **Deep Blue (#213547)** text, and **Teal (#33A06F)** as the main accent.

Type is set in **Inter var experimental**. Headlines run large with tight negative tracking; body text is 14.5px. Depth comes from soft drop shadows. Corners are mostly 2px.

Measured from [vuejs.org](https://vuejs.org/) on October 29, 2026 at 1440×900 and 390×844 from 270 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 11 roles, plus gradient stops #42D392, #647EFF.

- **White (#FFFFFF):** Page background, seen 3 times. Token `background`, CSS `--docsearch-footer-background`.
- **Deep Blue (#213547):** Primary text and headings, seen 59 times. Token `on-surface`, CSS `--vt-c-text-light-1`.
- **Blue (#476582):** Secondary text, seen 3 times. Token `on-surface-variant`, CSS `--vt-c-text-light-code`.
- **Slate (#767676):** Muted text and metadata, seen 11 times. Token `on-surface-muted`, CSS `--vt-c-text-2`.
- **Snow (#F9F9F9):** Raised areas one step from the page, seen 41 times. Token `surface-container-low`, CSS `--vt-c-white-soft`.
- **Mist (#F1F1F1):** Cards and panels, seen 3 times. Token `surface-container`, CSS `--vt-c-white-mute`.
- **Graphite 33% (#3C3C3C54):** Borders and dividers, seen 1 time. Token `outline`.
- **Graphite 29% (#3C3C3C4A):** Secondary dividers, seen 1 time. Token `outline-variant`, CSS `--vt-c-divider-light-1`.
- **Teal (#33A06F):** Brand accent (CSS variable). Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Teal (#42B883):** Accent in the logo, seen 3 times. Token `secondary`, CSS `--vt-c-green`.

## Typography

**Inter var experimental** carries the whole interface. Fallback stack: `Inter var experimental, Inter var, Inter, -apple-system`. Other loaded fonts: Inter.

- **headline-display:** Inter var experimental 76px at weight 900, line height 1.25, tracking -0.02em (48px on mobile). Page title (h1).
- **headline-lg:** Inter var experimental 20px at weight 600, line height 1.2, tracking -0.02em. Section headings (h2).
- **body-md:** Inter var experimental 14.5px at weight 400, line height 1.67, tracking 0.014em. Body text.
- **body-lg:** Inter var experimental 15px at weight 400, line height 1.6, tracking 0.013em. Lead paragraphs.
- **body-sm:** Inter var experimental 11px at weight 400, line height 2.18, tracking 0.018em. Secondary and small text.
- **label-lg:** Inter var experimental 16px at weight 400, line height 1.5, tracking 0.013em. Large buttons and tabs.
- **label-md:** Inter var experimental 13px at weight 500, tracking 0.015em. Buttons, navigation and labels.
- **label-sm:** Inter var experimental 12px at weight 500, line height 1.67, tracking 0.017em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 44% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 12px, lg 18px, xl 42px.
- **Sections:** 96px vertical padding between major sections.
- **Container:** content is capped at 960px.
- **Page margin:** 32px on each side of full-width sections.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.04) 0px 1px 2px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px`
- `rgba(0, 0, 0, 0.1) 0px 12px 32px 0px, rgba(0, 0, 0, 0.08) 0px 2px 6px 0px`

## Shapes

Most elements use 2px corners. Measured radii, most used first:

- **sm (2px):** 160 elements.
- **md (8px):** 20 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Security Updates for Vue 2”):** transparent fill, #476582 text, 16px/500, 8px radius, padding 8px 18px.
- **button-primary-hover:** background #E5E5E5, text #476582 on hover.
- **button-outline (“Get Started”):** #F1F1F1 fill, #476582 text, 16px/500, 8px radius, padding 8px 18px.
- **button-outline-hover:** background #E5E5E5, text #476582 on hover.
- **button-ghost (“Become a Sponsor”):** #F9F9F9 fill, #3C3C3C54 text, 11px/400, 2px radius, padding 0px.
- **link:** transparent fill, #213547 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F9F9F9, #F1F1F1.
- Do keep text in 3 levels: #213547, #476582, #767676.
- Do use #33A06F as the brand accent: header, logo and key highlights.
- Do set headlines in Inter var experimental with tight tracking (-0.02em).
- Do reuse the measured spacing steps (8px, 12px, 18px).
- Do use 2px corners on most elements; larger surfaces also use 8px.
- Don't introduce new font families beyond Inter var experimental.
- Don't use #33A06F for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.2s, 0.25s, 0.5s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/vuejs.org/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
