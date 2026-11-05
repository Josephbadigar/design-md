---
version: alpha
name: OpenRouter
description: "Light interface measured from openrouter.ai: gordita type with Plus Jakarta Sans, vivid violet accents, tonal surfaces and 6px corners."
colors:
  background: "#FCFCFE"
  surface: "#FCFCFE"
  on-surface: "#03080A"
  on-background: "#03080A"
  on-surface-variant: "#505456"
  surface-container-low: "#FFFFFF"
  outline: "#03080A14"
  primary: "#7624F4"
  on-primary: "#FCFCFE"
  secondary: "#E27625"
  success: "#007544"
typography:
  headline-display:
    fontFamily: gordita
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 36px
    fontWeight: 700
    lineHeight: 1.2
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.2
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: 450
    lineHeight: 1.63
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: 450
    lineHeight: 1.35
  body-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: 450
    lineHeight: 1.35
  label-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.35
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.63
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.63
rounded:
  sm: 4px
  md: 6px
  lg: 8px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 56px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 12px
    height: 32px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#03080A7B"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 0px 12px
    height: 32px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 0px 8px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 8px 12px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# OpenRouter Design System

## Overview

OpenRouter describes itself as: “The unified interface for every model. Find the best models & prices for your prompts” The interface is light, built on **Snow (#FCFCFE)** with **Near Black (#03080A)** text, and **Vivid Violet (#7624F4)** as the main accent.

Type is set in **gordita** and **Plus Jakarta Sans**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 6px.

Measured from [openrouter.ai](https://openrouter.ai/) on November 4, 2026 at 1440×900 and 390×844 from 294 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Snow (#FCFCFE):** Page background, seen 12 times. Token `background`.
- **Near Black (#03080A):** Primary text and headings, seen 36 times. Token `on-surface`.
- **Cool Slate (#505456):** Secondary text, seen 78 times. Token `on-surface-variant`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 13 times. Token `surface-container-low`.
- **Near Black 8% (#03080A14):** Borders and dividers, seen 19 times. Token `outline`.
- **Vivid Violet (#7624F4):** Primary buttons and calls to action, seen 6 times. Token `primary`, CSS `--violet-9`.
- **Snow (#FCFCFE):** Text and icons on primary. Token `on-primary`.
- **Orange (#E27625):** Accent, seen 2 times. Token `secondary`, CSS `--color-logo-metamask-orange-muted`.
- **Dark Teal (#007544):** Success and positive states, seen 2 times. Token `success`.

## Typography

**gordita** and **Plus Jakarta Sans** share the interface. Fallback stack: `gordita, gordita Fallback, Plus Jakarta Sans, jakarta`. Other loaded fonts: geistMono.

- **headline-display:** gordita 56px at weight 700, line height 1.2, tracking -0.025em. Page title (h1).
- **headline-lg:** Plus Jakarta Sans 36px at weight 700, line height 1.2. Section headings (h2).
- **headline-md:** Plus Jakarta Sans 20px at weight 600, line height 1.2. Sub-section headings.
- **body-md:** Plus Jakarta Sans 14px at weight 450, line height 1.63. Body text.
- **body-lg:** Plus Jakarta Sans 16px at weight 450, line height 1.35. Lead paragraphs.
- **body-sm:** Plus Jakarta Sans 12px at weight 450, line height 1.35. Secondary and small text.
- **label-lg:** Plus Jakarta Sans 16px at weight 500, line height 1.35. Large buttons and tabs.
- **label-md:** Plus Jakarta Sans 14px at weight 500, line height 1.63. Buttons, navigation and labels.
- **label-sm:** Plus Jakarta Sans 12px at weight 500, line height 1.63. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Sections:** 56px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 375px, 480px, 668px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`

## Shapes

Most elements use 6px corners. Measured radii, most used first:

- **md (6px):** 64 elements.
- **lg (8px):** 54 elements.
- **sm (4px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign Up”):** #7624F4 fill, #FCFCFE text, 14px/500, 6px radius, padding 0px 12px.
- **button-outline (“Search ⌘ K”):** #FFFFFF fill, #03080A7B text, 14px/450, 6px radius, padding 0px 12px, border 1px solid #03080A14.
- **button-ghost (“Models”):** transparent fill, #03080AB0 text, 14px/500, 6px radius, padding 0px 8px.
- **input-field (“you@company.com”):** #FFFFFF fill, #03080A text, 14px/450, 6px radius, padding 8px 12px, border 1px solid #03080A14.
- **card:** #FFFFFF fill, #03080A text, 14px/450, 8px radius, padding 0px, border 1px solid #03080A14.
- **link:** transparent fill, #03080AB0 text, padding 0px.

## Do's and Don'ts

- Do use #FCFCFE for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 2 levels: #03080A, #505456.
- Do reserve #7624F4 for primary actions and key highlights.
- Do set headlines in gordita with tight tracking (-0.025em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 6px corners on most elements; larger surfaces also use 8px and 4px.
- Don't introduce new font families beyond gordita and Plus Jakarta Sans.
- Don't use #7624F4 for large backgrounds or body text.
- Don't make interface transitions slower than 0.25s.

## Motion

Interface transitions are quick: 0.15s, 0.1s, 0.25s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `cubic-bezier(0.77, 0, 0.175, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/openrouter.ai/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
