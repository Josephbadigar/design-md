---
version: alpha
name: Netlify
description: "Dark interface measured from netlify.com: Figtree type with Instrument Sans, cyan accents, tonal surfaces and 4px corners."
colors:
  background: "#12181F"
  surface: "#12181F"
  on-surface: "#DEFFFE"
  on-background: "#DEFFFE"
  on-surface-strong: "#FFFFFF"
  on-surface-variant: "#E4F0FB"
  on-surface-muted: "#7E8792"
  surface-container-low: "#12181FF2"
  surface-container: "#181A1C"
  surface-container-high: "#1E242C"
  surface-container-highest: "#0C2A2A"
  overlay: "#E9EBED1A"
  overlay-strong: "#0C2A2A33"
  outline: "#FFFFFF33"
  outline-variant: "#272F38"
  primary: "#32E6E2"
  on-primary: "#12181F"
  secondary: "#89DDFF"
  tertiary: "#C792EA"
  warning: "#FBB13D"
typography:
  headline-display:
    fontFamily: Figtree
    fontSize: 64px
    fontWeight: 800
    lineHeight: 1.1
  headline-lg:
    fontFamily: Figtree
    fontSize: 32px
    fontWeight: 800
    lineHeight: 1.1
  headline-md:
    fontFamily: Figtree
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.1
  body-md:
    fontFamily: Instrument Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Figtree
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.1
  label-md:
    fontFamily: Instrument Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: Instrument Sans
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.5
  code:
    fontFamily: Martian Mono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Figtree
    fontSize: 41px
    fontWeight: 800
    lineHeight: 1.1
  headline-lg-mobile:
    fontFamily: Figtree
    fontSize: 24px
    fontWeight: 800
    lineHeight: 1.1
rounded:
  sm: 2px
  md: 4px
  lg: 6px
  xl: 360px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 12px
  section: 96px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 10px 17px
    height: 40px
  button-primary-hover:
    backgroundColor: "#8EFBF7"
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "#014847"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 8px
    height: 34px
  button-outline:
    textColor: "{colors.primary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.md}"
    padding: 8px
    height: 34px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    padding: 4px
  input-field:
    backgroundColor: "{colors.surface-container-high}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 8px
  card:
    backgroundColor: "{colors.surface-container-highest}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 24px
  link:
    textColor: "{colors.on-surface-muted}"
---

# Netlify Design System

## Overview

Netlify describes itself as: “Create with AI or code, deploy instantly on production infrastructure. One platform to build and ship.” The interface is dark, built on **Cool Charcoal (#12181F)** with **Pale Cyan (#DEFFFE)** text, and **Cyan (#32E6E2)** as the main accent.

Type is set in **Figtree** and **Instrument Sans**, with **Martian Mono** for code. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [netlify.com](https://www.netlify.com/) on October 21, 2026 at 1440×900 and 390×844 from 390 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 18 roles.

- **Cool Charcoal (#12181F):** Page background, seen 9 times. Token `background`, CSS `--ntl-button-primary-text-color`.
- **Pale Cyan (#DEFFFE):** Primary text and headings, seen 41 times. Token `on-surface`, CSS `--color-text-default`.
- **White (#FFFFFF):** Headings and emphasis, seen 20 times. Token `on-surface-strong`, CSS `--color-bg-1-inverse`.
- **Pale Blue (#E4F0FB):** Secondary text, seen 14 times. Token `on-surface-variant`.
- **Cool Gray (#7E8792):** Muted text and metadata, seen 37 times. Token `on-surface-muted`.
- **Cool Charcoal 95% (#12181FF2):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Charcoal (#181A1C):** Cards and panels, seen 1 time. Token `surface-container`.
- **Cool Graphite (#1E242C):** Hover and pressed fills, seen 2 times. Token `surface-container-high`, CSS `--ntl-neutral-700`.
- **Deep Cyan (#0C2A2A):** Highest raised elements, seen 5 times. Token `surface-container-highest`.
- **Mist 10% (#E9EBED1A):** Translucent fill for cards and controls, seen 10 times. Token `overlay`.
- **Deep Cyan 20% (#0C2A2A33):** Stronger translucent fill, seen 4 times. Token `overlay-strong`.
- **White 20% (#FFFFFF33):** Borders and dividers, seen 10 times. Token `outline`.
- **Cool Graphite (#272F38):** Secondary dividers, seen 4 times. Token `outline-variant`, CSS `--ntl-color-bg-3`.
- **Cyan (#32E6E2):** Primary buttons and calls to action, seen 30 times. Token `primary`, CSS `--search-loading-color`.
- **Cool Charcoal (#12181F):** Text and icons on primary. Token `on-primary`.
- **Light Cyan (#89DDFF):** Most used accent color, seen 15 times. Token `secondary`.
- **Light Violet (#C792EA):** Most used accent color, seen 15 times. Token `tertiary`.
- **Vivid Orange (#FBB13D):** Warnings and highlights, seen 1 time. Token `warning`.

## Typography

**Figtree**, **Instrument Sans** and **Martian Mono** (monospace) share the interface. Fallback stack: `Figtree, system-ui, Helvetica, sans-serif`.

- **headline-display:** Figtree 64px at weight 800, line height 1.1 (41px on mobile). Page title (h1).
- **headline-lg:** Figtree 32px at weight 800, line height 1.1 (24px on mobile). Section headings (h2).
- **headline-md:** Figtree 24px at weight 700, line height 1.1. Sub-section headings.
- **body-md:** Instrument Sans 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Figtree 18px at weight 600, line height 1.1. Lead paragraphs.
- **label-md:** Instrument Sans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Instrument Sans 13px at weight 700, line height 1.5. Small labels and badges.
- **code:** Martian Mono 16px at weight 400, line height 1.5. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (86% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 96px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Breakpoints:** 480px, 500px, 600px, 640px, 750px, 768px, 1024px, 1085px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.25) 0px 4px 12px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 94 elements.
- **xl (360px):** 28 elements.
- **lg (6px):** 16 elements.
- **full (9999px):** 16 elements.
- **sm (2px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #32E6E2 fill, #12181F text, 16px/700, 360px radius, padding 10px 17px, border 2px solid #32E6E2.
- **button-primary-hover:** background #8EFBF7, text #12181F on hover.
- **button-secondary (“Accept All”):** #32E6E2 fill, #014847 text, 13.008px/700, 4px radius, padding 8px, border 1px solid #32E6E2.
- **button-outline (“Reject All”):** transparent fill, #32E6E2 text, 13.008px/700, 4px radius, padding 8px, border 1px solid #32E6E2.
- **button-ghost (“Toggle platform submenu”):** transparent fill, #DEFFFE text, 16px/400, 50% radius, padding 4px.
- **input-field:** #1E242C fill, #FFFFFF text, 16px/400, 4px radius, padding 8px, border 1px solid #3B434C.
- **card:** #0C2A2A fill, #DEFFFE text, 16px/400, 6px radius, padding 24px, border 1px solid #0C2A2A.
- **link:** transparent fill, #7E8792 text, padding 0px.

## Do's and Don'ts

- Do use #12181F for the page and lift surfaces in small steps: #12181FF2, #181A1C, #1E242C, #0C2A2A.
- Do keep text in 4 levels: #DEFFFE, #FFFFFF, #E4F0FB, #7E8792.
- Do reserve #32E6E2 for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 360px, 6px and 2px.
- Don't introduce new font families beyond Figtree, Instrument Sans and Martian Mono.
- Don't use #32E6E2 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.15s.

- **Easing:** `cubic-bezier(0.22, 1, 0.36, 1)`, `cubic-bezier(0.33, 1, 0.68, 1)`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/netlify.com/), the free DESIGN.md generator.
