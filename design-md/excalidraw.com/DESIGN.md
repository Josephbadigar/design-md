---
version: alpha
name: Excalidraw
description: "Light interface measured from excalidraw.com: Times New Roman type with Assistant, indigo accents, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1B1B1F"
  on-background: "#1B1B1F"
  on-surface-variant: "#B8B8B8"
  surface-container-low: "#F0EFFF"
  surface-container: "#ECECF4"
  outline: "#D7D5FF"
  primary: "#6965DB"
  on-primary: "#FFFFFF"
  secondary: "#030064"
typography:
  headline-display:
    fontFamily: Times New Roman
    fontSize: 32px
    fontWeight: 700
  headline-lg:
    fontFamily: Assistant
    fontSize: 24px
    fontWeight: 700
  body-md:
    fontFamily: Arial
    fontSize: 14px
    fontWeight: 400
  body-lg:
    fontFamily: Times New Roman
    fontSize: 16px
    fontWeight: 400
  label-md:
    fontFamily: Assistant
    fontSize: 16px
    fontWeight: 400
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 19.92px
  gutter: 8px
  margin: 16px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
    padding: 10px
    height: 36px
  button-primary-hover:
    backgroundColor: "#5B57D1"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 14px 0px 10px
    height: 36px
  button-outline-hover:
    backgroundColor: "#E3E2FE"
  button-ghost:
    textColor: "#999999"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px
---

# Excalidraw Design System

## Overview

Excalidraw describes itself as: “Excalidraw is a virtual collaborative whiteboard tool that lets you easily sketch diagrams that have a hand-drawn feel to them.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1B1B1F)** text, and **Indigo (#6965DB)** as the main accent.

Type is set in **Times New Roman** and **Assistant**. Headlines run large; body text is 14px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are mostly 8px.

Measured from [excalidraw.com](https://excalidraw.com/) on October 21, 2026 at 1440×900 and 390×844 from 151 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background. Token `background`.
- **Charcoal (#1B1B1F):** Primary text and headings, seen 3 times. Token `on-surface`.
- **Silver (#B8B8B8):** Secondary text, seen 10 times. Token `on-surface-variant`.
- **Cool Snow (#F0EFFF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`.
- **Cool Mist (#ECECF4):** Cards and panels, seen 2 times. Token `surface-container`.
- **Pale Indigo (#D7D5FF):** Borders and dividers, seen 1 time. Token `outline`.
- **Indigo (#6965DB):** Primary buttons and calls to action, seen 8 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Indigo (#030064):** Accent, seen 5 times. Token `secondary`.

## Typography

**Times New Roman**, **Assistant** and **Arial** share the interface. Fallback stack: `Times New Roman`. Other loaded fonts: Excalifont.

- **headline-display:** Times New Roman 32px at weight 700. Page title (h1).
- **headline-lg:** Assistant 24px at weight 700. Section headings (h2).
- **body-md:** Arial 14px at weight 400. Body text.
- **body-lg:** Times New Roman 16px at weight 400. Lead paragraphs.
- **label-md:** Assistant 16px at weight 400. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 49% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 19.92px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 320px, 379px, 450px, 460px, 600px, 800px, 860px, 861px, 1024px, 1200px, 1536px, 1921px.

## Elevation & Depth

The design avoids drop shadows. Layers are separated by tonal surface steps (#F0EFFF → #ECECF4) and hairline rings:

- `rgb(255, 255, 255) 0px 0px 0px 1px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **lg (8px):** 76 elements.
- **md (6px):** 16 elements.
- **sm (4px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Share”):** #6965DB fill, #FFFFFF text, 13.3328px/400, 8px radius, padding 10px, border 1px solid #6965DB, shadow `rgb(255, 255, 255) 0px 0px 0px 1px`.
- **button-primary-hover:** background #5B57D1, text #FFFFFF on hover.
- **button-outline (“Try Excalidraw+ 14-day free tria”):** #F0EFFF fill, #6965DB text, 16px/500, 8px radius, padding 0px 14px 0px 10px, border 1px solid #D7D5FF.
- **button-outline-hover:** background #E3E2FE, text #6965DB on hover.
- **button-ghost (“Open Ctrl+O”):** transparent fill, #999999 text, 14px/400, 6px radius, padding 12px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F0EFFF, #ECECF4.
- Do keep text in 2 levels: #1B1B1F, #B8B8B8.
- Do reserve #6965DB for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 10px, 19.92px).
- Do use 8px corners on most elements; larger surfaces also use 6px and 4px.
- Don't use #B8B8B8 for body text; it reaches 2.0:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use hairline rings and tonal surfaces.
- Don't introduce new font families beyond Times New Roman, Assistant and Arial.
- Don't use #6965DB for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.25s, 0.15s.

- **Easing:** `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/excalidraw.com/), the free DESIGN.md generator.
