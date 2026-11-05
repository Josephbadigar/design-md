---
version: alpha
name: Streamlit
description: "Light interface measured from streamlit.io: Inter type with Helvetica, red accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#262730"
  on-background: "#262730"
  on-surface-strong: "#1C2022"
  on-surface-variant: "#697882"
  on-surface-muted: "#808495"
  surface-container-low: "#FFFAE8"
  surface-container: "#F0F2F6"
  outline: "#FFD16A"
  outline-variant: "#BFC5D3"
  primary: "#FF4B4B"
  on-primary: "#FFFFFF"
  secondary: "#1B95E0"
  tertiary: "#BD4043"
  warning: "#FFD16A"
  success: "#5CE488"
  error: "#FF6C6C"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 63px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: -0.035em
  headline-lg:
    fontFamily: Inter
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.67
    letterSpacing: -0.013em
  body-md:
    fontFamily: Helvetica
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  caption:
    fontFamily: Helvetica
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.5
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.05em
  code:
    fontFamily: Source Code Pro
    fontSize: 12px
    fontWeight: 400
    lineHeight: 2
    letterSpacing: 0.05em
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 31.5px
    fontWeight: 700
    lineHeight: 1.11
    letterSpacing: -0.025em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.78
rounded:
  sm: 1.75px
  md: 3.5px
  lg: 5.25px
  full: 9999px
spacing:
  xs: 3.5px
  sm: 7px
  md: 14px
  lg: 28px
  xl: 42px
  gutter: 10.5px
  section: 98px
  margin: 28px
  container: 1280px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.headline-lg}"
    rounded: "{rounded.lg}"
    padding: 14px 28px
    height: 63px
  button-primary-hover:
    backgroundColor: "#FF4B4BE6"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.headline-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.secondary}"
---

# Streamlit Design System

## Overview

Streamlit describes itself as: “Streamlit is an open-source Python framework for data scientists and AI/ML engineers to deliver interactive data apps – in only a few lines of code.” The interface is light, built on **White (#FFFFFF)** with **Cool Graphite (#262730)** text, and **Red (#FF4B4B)** as the main accent.

Type is set in **Inter** and **Helvetica**, with **Source Code Pro** for code. Headlines run large with tight negative tracking; body text is 16px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [streamlit.io](https://streamlit.io/) on November 4, 2026 at 1440×900 and 390×844 from 397 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 16 roles.

- **White (#FFFFFF):** Page background, seen 21 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Cool Graphite (#262730):** Primary text and headings, seen 40 times. Token `on-surface`.
- **Cool Charcoal (#1C2022):** Headings and emphasis, seen 28 times. Token `on-surface-strong`.
- **Blue (#697882):** Secondary text, seen 29 times. Token `on-surface-variant`.
- **Cool Gray (#808495):** Muted text and metadata, seen 53 times. Token `on-surface-muted`.
- **Pale Amber (#FFFAE8):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Mist (#F0F2F6):** Cards and panels, seen 2 times. Token `surface-container`.
- **Light Amber (#FFD16A):** Borders and dividers, seen 7 times. Token `outline`.
- **Light Blue (#BFC5D3):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Red (#FF4B4B):** Brand color in logos and imagery, seen 13 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Blue (#1B95E0):** Links and interactive text, seen 4 times. Token `secondary`.
- **Red (#BD4043):** Accent in the logo, seen 1 time. Token `tertiary`.
- **Light Amber (#FFD16A):** Warnings and highlights, seen 7 times. Token `warning`.
- **Green (#5CE488):** Success and positive states, seen 6 times. Token `success`.
- **Light Red (#FF6C6C):** Errors and destructive states, seen 2 times. Token `error`.

## Typography

**Inter**, **Helvetica** and **Source Code Pro** (monospace) share the interface. Fallback stack: `Inter, ui-sans-serif, system-ui, Helvetica`. Other loaded fonts: Permanent Marker.

- **headline-display:** Inter 63px at weight 700, line height 1, tracking -0.035em (31.5px on mobile). Page title (h1).
- **headline-lg:** Inter 21px at weight 400, line height 1.67, tracking -0.013em (16px on mobile). Section headings (h2).
- **body-md:** Helvetica 16px at weight 400, line height 1.4. Body text.
- **body-sm:** Inter 14px at weight 400, line height 1.5. Secondary and small text.
- **caption:** Helvetica 12px at weight 400, line height 1.4. Captions and fine print.
- **label-md:** Inter 14px at weight 600, line height 1.5. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 400, line height 1.5, tracking 0.05em. Small labels and badges.
- **code:** Source Code Pro 12px at weight 400, line height 2, tracking 0.05em. Code and technical values.

## Layout

Spacing does not follow a strict grid: 18% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 3.5px, sm 7px, md 14px, lg 28px, xl 42px.
- **Sections:** 98px vertical padding between major sections.
- **Gaps:** 10.5px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1280px.
- **Page margin:** 28px on each side of full-width sections.
- **Breakpoints:** 400px, 410px, 425px, 426px, 550px, 600px, 640px, 768px, 769px, 896px, 1024px, 1280px, 1600px, 1980px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.1) 0px 8px 10px -6px`
- `rgb(255, 75, 75) 0px 0px 4px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.25) 0px 25px 50px -12px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 68 elements.
- **md (3.5px):** 60 elements.
- **sm (1.75px):** 48 elements.
- **lg (5.25px):** 48 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started”):** #FF4B4B fill, #FFFFFF text, 21px/400, 5.25px radius, padding 14px 28px.
- **button-primary-hover:** background #FF4B4BE6, text #FFFFFF on hover.
- **button-ghost (“pip install streamlit”):** transparent fill, #FFFFFF text, 21px/400, padding 0px.
- **link:** transparent fill, #1B95E0 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFAE8, #F0F2F6.
- Do keep text in 4 levels: #262730, #1C2022, #697882, #808495.
- Do use #FF4B4B as the brand accent: header, logo and key highlights.
- Do set headlines in Inter with tight tracking (-0.035em).
- Do reuse the measured spacing steps (7px, 14px, 28px).
- Do make buttons and chips fully rounded (9999px); most other elements use 3.5px corners.
- Don't use #808495 for body text; it reaches 3.72:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter, Helvetica and Source Code Pro.
- Don't use #FF4B4B for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.075s, 0.15s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/streamlit.io/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
