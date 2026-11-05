---
version: alpha
name: HeyGen
description: "Light interface measured from heygen.com: ABC Solar Display type with TT Norms Pro, vivid cyan accents, tonal surfaces and 12px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#171717"
  on-surface-muted: "#333333"
  on-surface-subtle: "#4C4C4C"
  surface-container-low: "#FFFFFFF2"
  surface-container: "#FFFFFFE6"
  surface-container-high: "#FAFAFA"
  surface-container-highest: "#DFF8FF"
  overlay: "#FFFFFFB3"
  overlay-strong: "#00000073"
  outline: "#0000001A"
  outline-variant: "#3333330D"
  primary: "#00C3FF"
  on-primary: "#033337"
  secondary: "#F3A6FF"
  tertiary: "#3CE6AC"
typography:
  headline-display:
    fontFamily: ABC Solar Display
    fontSize: 60px
    fontWeight: 400
    lineHeight: 1
  headline-lg:
    fontFamily: ABC Solar Display
    fontSize: 56px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.025em
  headline-md:
    fontFamily: ABC Solar Display
    fontSize: 44px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.025em
  headline-sm:
    fontFamily: ABC Solar Display
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1
  title-lg:
    fontFamily: ABC Solar Display
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.1
  body-md:
    fontFamily: TT Norms Pro
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: TT Norms Pro
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: -0.008em
  label-lg:
    fontFamily: TT Norms Pro
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: ABC Solar Display
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1.47
  label-sm:
    fontFamily: TT Norms Pro
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: 0.025em
  headline-display-mobile:
    fontFamily: ABC Solar Display
    fontSize: 31px
    fontWeight: 400
    lineHeight: 1
  headline-lg-mobile:
    fontFamily: ABC Solar Display
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: -0.025em
rounded:
  xs: 6px
  sm: 12px
  md: 20px
  lg: 27px
  xl: 30px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 20px
  xl: 60px
  gutter: 8px
  section: 120px
  container: 1408px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-secondary:
    backgroundColor: "#D9D9D9"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-tertiary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 0px 16px
    height: 40px
  button-ghost:
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 10px 8px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 0px
  link:
    textColor: "#99A1AF"
---

# HeyGen Design System

## Overview

HeyGen describes itself as: “Be your best self, every time. Create clear, confident AI videos with your Personal Avatar—your face and voice, without filming every video. Try it free.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Vivid Cyan (#00C3FF)** as the main accent.

Type is set in **ABC Solar Display** and **TT Norms Pro**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 12px.

Measured from [heygen.com](https://www.heygen.com/) on November 4, 2026 at 1440×900 and 390×844 from 435 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles, plus gradient stops #BCEFFF, #DDD5FF, #FFD8E9, #F3A6FF.

- **White (#FFFFFF):** Page background, seen 18 times. Token `background`, CSS `--color-fillUpper`.
- **Near Black (#000000):** Primary text and headings, seen 77 times. Token `on-surface`.
- **Charcoal (#171717):** Secondary text, seen 18 times. Token `on-surface-variant`.
- **Graphite (#333333):** Muted text and metadata, seen 11 times. Token `on-surface-muted`, CSS `--color-heygen-gray-carbon`.
- **Graphite (#4C4C4C):** Subtle text and placeholders, seen 8 times. Token `on-surface-subtle`.
- **White 95% (#FFFFFFF2):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`.
- **White 90% (#FFFFFFE6):** Cards and panels, seen 2 times. Token `surface-container`.
- **Snow (#FAFAFA):** Hover and pressed fills, seen 4 times. Token `surface-container-high`.
- **Pale Cyan (#DFF8FF):** Highest raised elements, seen 6 times. Token `surface-container-highest`, CSS `--color-heygen-blue-light`.
- **White 70% (#FFFFFFB3):** Translucent fill for cards and controls, seen 7 times. Token `overlay`.
- **Near Black 45% (#00000073):** Stronger translucent fill, seen 4 times. Token `overlay-strong`.
- **Near Black 10% (#0000001A):** Borders and dividers, seen 15 times. Token `outline`.
- **Graphite 5% (#3333330D):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **Vivid Cyan (#00C3FF):** Primary buttons and calls to action, seen 16 times. Token `primary`.
- **Deep Cyan (#033337):** Text and icons on primary. Token `on-primary`.
- **Light Purple (#F3A6FF):** Accent (CSS variable), seen 2 times. Token `secondary`, CSS `--color-pink-500`.
- **Teal (#3CE6AC):** Accent (CSS variable). Token `tertiary`.

## Typography

**ABC Solar Display** and **TT Norms Pro** share the interface. Fallback stack: `ABC Solar Display, TT Norms Pro, Arial, Helvetica`.

- **headline-display:** ABC Solar Display 60px at weight 400, line height 1 (31px on mobile). Page title (h1).
- **headline-lg:** ABC Solar Display 56px at weight 700, line height 1.05, tracking -0.025em (32px on mobile). Section headings (h2).
- **headline-md:** ABC Solar Display 44px at weight 700, line height 1.05, tracking -0.025em. Sub-section headings.
- **headline-sm:** ABC Solar Display 30px at weight 700, line height 1. Card and feature titles.
- **title-lg:** ABC Solar Display 24px at weight 700, line height 1.1. Small titles.
- **body-md:** TT Norms Pro 14px at weight 400, line height 1.43. Body text.
- **body-lg:** TT Norms Pro 18px at weight 500, line height 1.4, tracking -0.008em. Lead paragraphs.
- **label-lg:** TT Norms Pro 16px at weight 400, line height 1.5. Large buttons and tabs.
- **label-md:** ABC Solar Display 15px at weight 700, line height 1.47. Buttons, navigation and labels.
- **label-sm:** TT Norms Pro 14px at weight 700, line height 1.5, tracking 0.025em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 16px, lg 20px, xl 60px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1408px.
- **Breakpoints:** 520px, 640px, 767px, 768px, 996px, 1160px, 1200px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 4px 6px -1px, rgba(0, 0, 0, 0.1) 0px 2px 4px -2px`

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **sm (12px):** 120 elements.
- **md (20px):** 20 elements.
- **lg (27px):** 20 elements.
- **xl (30px):** 20 elements.
- **xs (6px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign in”):** #00C3FF fill, #033337 text, 18px/700, 12px radius, padding 0px 16px.
- **button-secondary (“Book a demo”):** #D9D9D9 fill, #000000 text, 18px/700, 12px radius, padding 0px 16px.
- **button-tertiary (“Get started for free”):** #000000 fill, #00C3FF text, 18px/700, 12px radius, padding 0px 16px.
- **button-ghost (“Platform”):** transparent fill, 18px/500, 12px radius, padding 10px 8px.
- **card:** #FFFFFF fill, #171717 text, 16px/400, 20px radius, padding 0px.
- **link:** transparent fill, #99A1AF text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FFFFFFF2, #FFFFFFE6, #FAFAFA, #DFF8FF.
- Do keep text in 4 levels: #000000, #171717, #333333, #4C4C4C.
- Do reserve #00C3FF for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 20px).
- Do use 12px corners on most elements; larger surfaces also use 20px, 27px and 30px.
- Don't introduce new font families beyond ABC Solar Display and TT Norms Pro.
- Don't use #00C3FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.3s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/heygen.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
