---
version: alpha
name: OpenAI
description: "Light interface measured from openai.com: OpenAI Sans type, pink accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#666666"
  overlay: "#0000000A"
  outline: "#0000001F"
  primary: "#AB4F7A"
  on-primary: "#FFFFFF"
  secondary: "#6BC67F"
  tertiary: "#653218"
typography:
  headline-display:
    fontFamily: OpenAI Sans
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.26
    letterSpacing: -0.01em
  body-md:
    fontFamily: OpenAI Sans
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.32
    letterSpacing: -0.01em
  label-lg:
    fontFamily: OpenAI Sans
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: -0.01em
  label-md:
    fontFamily: OpenAI Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.4
  label-sm:
    fontFamily: OpenAI Sans
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.51
  headline-display-mobile:
    fontFamily: OpenAI Sans
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  sm: 4px
  md: 6.08px
  lg: 24px
  xl: 40px
  full: 9999px
spacing:
  xs: 3.9px
  sm: 8px
  md: 12px
  lg: 32px
  xl: 64px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 0px 20px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  input-field:
    textColor: "{colors.on-surface}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# OpenAI Design System

## Overview

OpenAI describes itself as: “We believe our research will eventually lead to artificial general intelligence, a system that can solve human-level problems.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Pink (#AB4F7A)** as the main accent.

Type is set in **OpenAI Sans**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [openai.com](https://openai.com/) on November 4, 2026 at 1440×900 and 390×844 from 329 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **White (#FFFFFF):** Page background, seen 2 times. Token `background`, CSS `--color-primitive-gray-0`.
- **Near Black (#000000):** Primary text and headings, seen 97 times. Token `on-surface`, CSS `--color-syntax-copy`.
- **Slate (#666666):** Secondary text, seen 14 times. Token `on-surface-variant`.
- **Near Black 4% (#0000000A):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Near Black 12% (#0000001F):** Borders and dividers, seen 5 times. Token `outline`.
- **Pink (#AB4F7A):** Brand accent (CSS variable). Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Green (#6BC67F):** Accent (CSS variable). Token `secondary`.
- **Dark Orange (#653218):** Accent (CSS variable). Token `tertiary`.

## Typography

**OpenAI Sans** carries the whole interface. Fallback stack: `OpenAI Sans, OpenAI Sans Variable Scripts, sans-serif`.

- **headline-display:** OpenAI Sans 22px at weight 500, line height 1.26, tracking -0.01em (20px on mobile). Page title (h1).
- **body-md:** OpenAI Sans 18px at weight 500, line height 1.32, tracking -0.01em. Body text.
- **label-lg:** OpenAI Sans 17px at weight 400, line height 1.65, tracking -0.01em. Large buttons and tabs.
- **label-md:** OpenAI Sans 14px at weight 500, line height 1.4. Buttons, navigation and labels.
- **label-sm:** OpenAI Sans 13px at weight 500, line height 1.51. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (85% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 3.9px, sm 8px, md 12px, lg 32px, xl 64px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 640px, 767px, 768px, 800px, 1024px, 1200px, 1201px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.02) 0px 4px 6px 0px, rgba(0, 0, 0, 0.05) 0px 0px 2px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.04) 0px 3px 6px 0px, rgba(0, 0, 0, 0.04) 0px 4px 80px 8px, rgba(0, 0, 0, 0.62) 0px 0px 1px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 28 elements.
- **sm (4px):** 16 elements.
- **xl (40px):** 12 elements.
- **md (6.08px):** 4 elements.
- **lg (24px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Try ChatGPT (opens in a new wind”):** #000000 fill, #FFFFFF text, 14px/500, 40px radius, padding 0px 20px.
- **button-ghost (“Products”):** transparent fill, #000000 text, 17px/400, padding 0px.
- **input-field:** transparent fill, #000000 text, 16px/400, padding 0px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 2 levels: #000000, #666666.
- Do use #AB4F7A as the brand accent: header, logo and key highlights.
- Do set headlines in OpenAI Sans with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 12px, 32px).
- Do make buttons and chips fully rounded (9999px); most other elements use 4px corners.
- Don't introduce new font families beyond OpenAI Sans.
- Don't use #AB4F7A for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.25s, 0.3s, 0.1s, 0.2s.

- **Easing:** `ease`, `cubic-bezier(0, 0, 1, 1)`, `cubic-bezier(0.6, 0, 0.4, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/openai.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
