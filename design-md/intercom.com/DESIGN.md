---
version: alpha
name: Intercom
description: "Light monochrome interface measured from intercom.com: Saans type with Serrif, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#111111"
  on-surface-muted: "#414141"
  on-surface-subtle: "#585858"
  surface-container-low: "#FAF9F6"
  surface-container: "#D3CEC6"
  overlay: "#00000008"
  overlay-strong: "#FFFFFF0D"
  outline: "#1111111A"
  outline-variant: "#1111110D"
  primary: "#111111"
  on-primary: "#FFFFFF"
  secondary: "#0007CB"
  tertiary: "#FF5600"
typography:
  headline-display:
    fontFamily: Saans
    fontSize: 80px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Saans
    fontSize: 54px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Saans
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.034em
  headline-sm:
    fontFamily: Saans
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.02em
  title-lg:
    fontFamily: Saans
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-md:
    fontFamily: Saans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.25
  body-lg:
    fontFamily: Serrif
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1.4
    letterSpacing: -0.01em
  label-md:
    fontFamily: Saans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-sm:
    fontFamily: LLMedium
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.5
  code:
    fontFamily: SaansMono
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: 0.05em
  headline-display-mobile:
    fontFamily: Saans
    fontSize: 40px
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: Saans
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1
    letterSpacing: -0.032em
  title-lg-mobile:
    fontFamily: Saans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
rounded:
  sm: 4px
  md: 6px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 8px
  section: 112px
  margin: 16px
  container: 1920px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
    height: 40px
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 0px 12px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 4px 14px
    height: 40px
  link:
    textColor: "{colors.on-surface}"
---

# Intercom Design System

## Overview

Intercom describes itself as: “Intercom is the only helpdesk with a natively integrated AI Agent, Fin, meaning every customer conversation improves the next one, enabling perfect experiences that were never possible before.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Saans** and **Serrif**, with **SaansMono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 4px.

Measured from [intercom.com](https://www.intercom.com/) on October 29, 2026 at 1440×900 and 390×844 from 408 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--color-report-white`.
- **Near Black (#000000):** Primary text and headings, seen 52 times. Token `on-surface`, CSS `--tw-mask-bottom-from-color`.
- **Charcoal (#111111):** Secondary text, seen 55 times. Token `on-surface-variant`, CSS `--button-secondary-foreground`.
- **Graphite (#414141):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Slate (#585858):** Subtle text and placeholders, seen 6 times. Token `on-surface-subtle`.
- **Snow (#FAF9F6):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Warm Silver (#D3CEC6):** Cards and panels, seen 24 times. Token `surface-container`.
- **Near Black 3% (#00000008):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **White 5% (#FFFFFF0D):** Stronger translucent fill, seen 1 time. Token `overlay-strong`.
- **Charcoal 10% (#1111111A):** Borders and dividers, seen 5 times. Token `outline`.
- **Charcoal 5% (#1111110D):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Charcoal (#111111):** Primary buttons and calls to action, seen 83 times. Token `primary`, CSS `--button-secondary-foreground`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Indigo (#0007CB):** Accent in text, fills and borders, seen 19 times. Token `secondary`.
- **Vivid Orange (#FF5600):** Accent in text, fills and borders, seen 9 times. Token `tertiary`, CSS `--color-fin`.

## Typography

**Saans**, **Serrif**, **LLMedium** and **SaansMono** (monospace) share the interface. Fallback stack: `Saans, Saans Fallback, Hiragino Kaku Gothic ProN, Hiragino Sans`.

- **headline-display:** Saans 80px at weight 400, line height 1, tracking -0.03em (40px on mobile). Page title (h1).
- **headline-lg:** Saans 54px at weight 400, line height 1, tracking -0.03em (30px on mobile). Section headings (h2).
- **headline-md:** Saans 28px at weight 400, line height 1, tracking -0.034em. Sub-section headings.
- **headline-sm:** Saans 24px at weight 400, line height 1, tracking -0.02em. Card and feature titles.
- **title-lg:** Saans 20px at weight 400, line height 1.2, tracking -0.01em (16px on mobile). Small titles.
- **body-md:** Saans 14px at weight 400, line height 1.25. Body text.
- **body-lg:** Serrif 16px at weight 300, line height 1.4, tracking -0.01em. Lead paragraphs.
- **label-md:** Saans 16px at weight 400, line height 1.5. Buttons, navigation and labels.
- **label-sm:** LLMedium 13px at weight 700, line height 1.5. Small labels and badges.
- **code:** SaansMono 12px at weight 400, line height 1, tracking 0.05em. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 24px, xl 48px.
- **Sections:** 112px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1920px.
- **Page margin:** 16px on each side of full-width sections.
- **Breakpoints:** 451px, 700px, 740px, 820px, 1140px, 1230px, 1370px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.75) 0px 9.841px 82.665px 0px`

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **sm (4px):** 68 elements.
- **md (6px):** 28 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start free trial”):** #111111 fill, #FFFFFF text, 14px/400, 4px radius, padding 0px 12px.
- **button-outline (“Fin AI Agent →”):** transparent fill, #000000 text, 14px/400, 4px radius, padding 0px 12px, border 1px solid #000000.
- **button-ghost (“View demo”):** transparent fill, #111111 text, 16px/400, 4px radius, padding 4px 14px, border 1px solid #111111.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FAF9F6, #D3CEC6.
- Do keep text in 4 levels: #000000, #111111, #414141, #585858.
- Do let contrast carry emphasis; primary actions use #111111 on #FFFFFF.
- Do set headlines in Saans with tight tracking (-0.03em).
- Do reuse the measured spacing steps (8px, 16px, 24px).
- Do use 4px corners on most elements; larger surfaces also use 6px.
- Don't introduce new font families beyond Saans, Serrif, LLMedium and SaansMono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.2s, 0.15s, 0.4s, 0.25s.

- **Easing:** `ease-out`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/intercom.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
