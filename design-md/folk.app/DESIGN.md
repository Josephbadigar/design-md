---
version: alpha
name: Folk
description: "Light interface measured from folk.app: Uxumgrotesque type with Inter, vivid amber accents, flat surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1F1E1C"
  on-background: "#1F1E1C"
  on-surface-variant: "#333333"
  on-surface-muted: "#5C5C5C"
  on-surface-subtle: "#626262"
  overlay: "#12120008"
  overlay-strong: "#030200E3"
  outline: "#D4D4D4"
  primary: "#FFC53D"
  on-primary: "#000000"
  inverse-surface: "#21201C"
  secondary: "#8145B5"
typography:
  headline-display:
    fontFamily: Uxumgrotesque
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Uxumgrotesque
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.023em
  headline-md:
    fontFamily: Uxumgrotesque
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.021em
  headline-sm:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.21
    letterSpacing: -0.021em
  body-md:
    fontFamily: Foundersgrotesk
    fontSize: 14.5px
    fontWeight: 400
    lineHeight: 1.6
  body-lg:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.23
    letterSpacing: -0.017em
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.33
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.38
    letterSpacing: -0.003em
  code:
    fontFamily: Geist Mono
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1
  headline-display-mobile:
    fontFamily: Uxumgrotesque
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.025em
  headline-lg-mobile:
    fontFamily: Uxumgrotesque
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.023em
  headline-md-mobile:
    fontFamily: Uxumgrotesque
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.021em
rounded:
  sm: 20px
  md: 100px
  full: 9999px
spacing:
  base: 4px
  xs: 2px
  sm: 8px
  md: 16px
  lg: 20px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.overlay-strong}"
    textColor: "{colors.background}"
    rounded: 0px
    padding: 0px 16px
    height: 48px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 8px 12px
    height: 32px
  button-outline-hover:
    backgroundColor: "#0F08000F"
  input-field:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface-variant}"
    rounded: 0px
    padding: 0px 10px 0px 16px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.inverse-surface}"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 12px 32px 12px 16px
---

# Folk Design System

## Overview

Folk describes itself as: “One platform for your entire sales motion. Prospect, engage, and close deals with the only AI CRM your team needs. Trusted by 5,000+ companies.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1F1E1C)** text, and **Vivid Amber (#FFC53D)** as the main accent.

Type is set in **Uxumgrotesque** and **Inter**, with **Geist Mono** for code. Headlines run large with tight negative tracking; body text is 14.5px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [folk.app](https://www.folk.app/) on October 29, 2026 at 1440×900 and 390×844 from 291 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 12 roles.

- **White (#FFFFFF):** Page background, seen 25 times. Token `background`, CSS `--_folk-2026---ui--surface-alt`.
- **Charcoal (#1F1E1C):** Primary text and headings. Token `on-surface`.
- **Graphite (#333333):** Secondary text, seen 2 times. Token `on-surface-variant`.
- **Slate (#5C5C5C):** Muted text and metadata, seen 2 times. Token `on-surface-muted`.
- **Slate (#626262):** Subtle text and placeholders, seen 6 times. Token `on-surface-subtle`.
- **Deep Yellow 3% (#12120008):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Near Black 89% (#030200E3):** Stronger translucent fill, seen 2 times. Token `overlay-strong`, CSS `--button--hover-border`.
- **Silver (#D4D4D4):** Borders and dividers, seen 1 time. Token `outline`.
- **Vivid Amber (#FFC53D):** Brand accent (CSS variable). Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Charcoal (#21201C):** High-contrast fills, seen 1 time. Token `inverse-surface`.
- **Violet (#8145B5):** Accent in text, fills and borders, seen 2 times. Token `secondary`.

## Typography

**Uxumgrotesque**, **Inter**, **Foundersgrotesk** and **Geist Mono** (monospace) share the interface. Fallback stack: `Uxumgrotesque, sans-serif`.

- **headline-display:** Uxumgrotesque 72px at weight 500, line height 1, tracking -0.025em (32px on mobile). Page title (h1).
- **headline-lg:** Uxumgrotesque 64px at weight 500, line height 1, tracking -0.023em (32px on mobile). Section headings (h2).
- **headline-md:** Uxumgrotesque 36px at weight 500, line height 1, tracking -0.021em (28px on mobile). Sub-section headings.
- **headline-sm:** Inter 28px at weight 400, line height 1.21, tracking -0.021em. Card and feature titles.
- **body-md:** Foundersgrotesk 14.5px at weight 400, line height 1.6. Body text.
- **body-lg:** Inter 20px at weight 400, line height 1.23, tracking -0.017em. Lead paragraphs.
- **body-sm:** Inter 12px at weight 400, line height 1.33. Secondary and small text.
- **label-md:** Inter 13px at weight 500, line height 1.38, tracking -0.003em. Buttons, navigation and labels.
- **code:** Geist Mono 13px at weight 400, line height 1. Code and technical values.

## Layout

Spacing follows a 4px grid: 92% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 2px, sm 8px, md 16px, lg 20px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 480px, 767px, 768px, 991px, 1440px, 1920px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 4px 12px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **sm (20px):** 28 elements.
- **full (9999px):** 20 elements.
- **md (100px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Start for free”):** #030200E3 fill, #FFFFFF text, 14px/400, padding 0px 16px.
- **button-outline (“Get a demo”):** #FFFFFF fill, #030200E3 text, 14.4px/400, 20px radius, padding 8px 12px, border 1px solid #D4D4D4.
- **button-outline-hover:** background #0F08000F, text #030200E3 on hover.
- **input-field (“What's your work email?”):** #12120008 fill, #333333 text, 14px/400, padding 0px 10px 0px 16px.
- **card:** #FFFFFF fill, #21201C text, 14.4px/400, padding 12px 32px 12px 16px, shadow `rgba(0, 0, 0, 0.1) 0px 4px 12px 0px`.

## Do's and Don'ts

- Do use #FFFFFF for the page.
- Do keep text in 4 levels: #1F1E1C, #333333, #5C5C5C, #626262.
- Do use #FFC53D as the brand accent: header, logo and key highlights.
- Do set headlines in Uxumgrotesque with tight tracking (-0.025em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 20px corners.
- Don't introduce new font families beyond Uxumgrotesque, Inter, Foundersgrotesk and Geist Mono.
- Don't use #FFC53D for large backgrounds or body text.
- Don't make interface transitions slower than 0.15s.

## Motion

Interface transitions are quick: 0.15s.

- **Easing:** `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/folk.app/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
