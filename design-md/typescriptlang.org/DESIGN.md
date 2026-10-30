---
version: alpha
name: TypeScript
description: "Dark interface measured from typescriptlang.org: Segoe UI Web (West European) type, dark blue accents, flat surfaces and square corners."
colors:
  background: "#3178C6"
  surface: "#3178C6"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#FFFFFF"
  on-surface-muted: "#EEEEEE"
  overlay: "#FF000026"
  outline: "#FFFFFF4D"
  primary: "#235A97"
  on-primary: "#FFFFFF"
  secondary: "#098658"
  tertiary: "#F7CBA4"
typography:
  headline-display:
    fontFamily: Segoe UI Web (West European)
    fontSize: 40px
    fontWeight: 200
    lineHeight: 1.12
  headline-lg:
    fontFamily: Segoe UI Web (West European)
    fontSize: 25.5px
    fontWeight: 400
    lineHeight: 1
  body-md:
    fontFamily: Segoe UI Web (West European)
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-lg:
    fontFamily: Segoe UI Web (West European)
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Segoe UI Web (West European)
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  label-md:
    fontFamily: Segoe UI Web (West European)
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.4
  code:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
rounded:
  none: 0px
spacing:
  xs: 2px
  sm: 8px
  md: 16px
  lg: 19.2px
  xl: 42px
  section: 48px
  container: 1040px
components:
  button-primary:
    backgroundColor: "{colors.on-surface-variant}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: 8px 16px
    height: 61px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-muted}"
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: 8px 0px
  input-field:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.none}"
    padding: 1px 2px
  link:
    textColor: "{colors.on-surface-variant}"
---

# TypeScript Design System

## Overview

TypeScript describes itself as: “TypeScript extends JavaScript by adding types to the language. TypeScript speeds up your development experience by catching errors and providing fixes before you even run your code.” The interface is dark, built on **Blue (#3178C6)** with **Near Black (#000000)** text, and **Dark Blue (#235A97)** as the main accent.

Type is set in **Segoe UI Web (West European)**, with **JetBrains Mono** for code. Headlines run large; body text is 16px. Depth comes from soft drop shadows. Corners are square.

Measured from [typescriptlang.org](https://www.typescriptlang.org/) on October 29, 2026 at 1440×900 and 390×844 from 260 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Blue (#3178C6):** Page background, seen 4 times. Token `background`.
- **Near Black (#000000):** Primary text and headings, seen 38 times. Token `on-surface`, CSS `--sidebar-link-border-color`.
- **White (#FFFFFF):** Secondary text, seen 37 times. Token `on-surface-variant`, CSS `--playground-dropdown-bg`.
- **Mist (#EEEEEE):** Muted text and metadata, seen 12 times. Token `on-surface-muted`, CSS `--sidebar-background-color`.
- **Vivid Red 15% (#FF000026):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **White 30% (#FFFFFF4D):** Borders and dividers, seen 1 time. Token `outline`.
- **Dark Blue (#235A97):** Brand color on large areas, seen 1 time. Token `primary`, CSS `--link-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Teal (#098658):** Accent in text, fills and borders, seen 4 times. Token `secondary`.
- **Light Orange (#F7CBA4):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

## Typography

**Segoe UI Web (West European)** and **JetBrains Mono** (monospace) share the interface. Fallback stack: `Segoe UI Web (West European), Segoe UI, -apple-system, BlinkMacSystemFont`. Other loaded fonts: Cascadia Mono-SemiLight.

- **headline-display:** Segoe UI Web (West European) 40px at weight 200, line height 1.12. Page title (h1).
- **headline-lg:** Segoe UI Web (West European) 25.5px at weight 400, line height 1. Section headings (h2).
- **body-md:** Segoe UI Web (West European) 16px at weight 400, line height 1.4. Body text.
- **body-lg:** Segoe UI Web (West European) 19px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** Segoe UI Web (West European) 14px at weight 400, line height 1.4. Secondary and small text.
- **label-md:** Segoe UI Web (West European) 16px at weight 600, line height 1.4. Buttons, navigation and labels.
- **code:** JetBrains Mono 16px at weight 400, line height 1.4. Code and technical values.

## Layout

Spacing does not follow a strict grid: 41% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 8px, md 16px, lg 19.2px, xl 42px.
- **Sections:** 48px vertical padding between major sections.
- **Container:** content is capped at 1040px.
- **Breakpoints:** 480px, 767px, 768px, 790px, 800px, 900px, 1050px, 1084px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.25) 0px 4px 20px -6px`

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try TypeScript Now Online or via”):** #FFFFFF fill, #000000 text, 16px/400, padding 8px 16px.
- **button-primary-hover:** background #EEEEEE, text #000000 on hover.
- **button-ghost (“Read”):** transparent fill, #000000 text, 16px/400, padding 8px 0px, border 1px solid #000000.
- **input-field (“Search Docs”):** #235A97 fill, #FFFFFF text, 16px/600, padding 1px 2px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #3178C6 for the page.
- Do keep text in 3 levels: #000000, #FFFFFF, #EEEEEE.
- Do use #235A97 as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 19.2px).
- Don't use #EEEEEE for body text; it reaches 3.91:1 on #3178C6. Keep it for large text or metadata.
- Don't introduce new font families beyond Segoe UI Web (West European) and JetBrains Mono.
- Don't use #235A97 for large backgrounds or body text.

Generated by [Sitepeel](https://sitepeel.dev/design-md/typescriptlang.org/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
