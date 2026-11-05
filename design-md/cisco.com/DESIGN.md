---
version: alpha
name: Cisco
description: "Dark interface measured from cisco.com: Inter type, dark green accents, flat surfaces and 48px corners."
colors:
  background: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#536070"
  overlay: "#FFFFFF40"
  outline: "#4D4D4D"
  outline-variant: "#FFFFFF1A"
  primary: "#058103"
  on-primary: "#FFFFFF"
  secondary: "#124FC9"
  tertiary: "#02C8FF"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1.13
  headline-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.17
  headline-md:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.44
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 300
    lineHeight: 2
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.44
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 300
    lineHeight: 2
  label-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.22
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: 500
    lineHeight: 1.25
rounded:
  sm: 4px
  md: 8px
  lg: 48px
  xl: 120px
  full: 9999px
spacing:
  xs: 4px
  sm: 5px
  md: 16px
  lg: 20px
  xl: 36px
  gutter: 24px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 0px
    height: 56px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "#07182D"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 10px 20px
    height: 48px
  button-outline:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 10px 20px
    height: 46px
  button-ghost:
    textColor: "#07182D"
    typography: "{typography.body-md}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Cisco Design System

## Overview

Cisco describes itself as: “Cisco is a worldwide technology leader powering an inclusive future for all. Learn more about our products, services, solutions, and innovations.” The interface is dark, built on **Near Black (#000000)** with **White (#FFFFFF)** text, and **Dark Green (#058103)** as the main accent.

Type is set in **Inter**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 48px.

Measured from [cisco.com](https://www.cisco.com/) on November 4, 2026 at 1440×900 and 390×844 from 289 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Near Black (#000000):** Page background, seen 11 times. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 64 times. Token `on-surface`, CSS `--muse-background-neutral`.
- **Blue (#536070):** Secondary text, seen 15 times. Token `on-surface-variant`, CSS `--chat-text-subtle`.
- **White 25% (#FFFFFF40):** Translucent fill for cards and controls, seen 2 times. Token `overlay`.
- **Slate (#4D4D4D):** Borders and dividers, seen 2 times. Token `outline`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 1 time. Token `outline-variant`.
- **Dark Green (#058103):** Primary buttons and calls to action, seen 1 time. Token `primary`, CSS `--muse-border-success`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#124FC9):** Accent (CSS variable). Token `secondary`.
- **Vivid Cyan (#02C8FF):** Accent in the logo, seen 1 time. Token `tertiary`.

## Typography

**Inter** carries the whole interface. Fallback stack: `Inter, Noto Sans, CiscoSans, CiscoSansTT`.

- **headline-display:** Inter 60px at weight 500, line height 1.13 (36px on mobile). Page title (h1).
- **headline-lg:** Inter 48px at weight 500, line height 1.17 (32px on mobile). Section headings (h2).
- **headline-md:** Inter 32px at weight 500, line height 1.25. Sub-section headings.
- **headline-sm:** Inter 20px at weight 500, line height 1.44. Card and feature titles.
- **body-md:** Inter 14px at weight 300, line height 2. Body text.
- **body-lg:** Inter 18px at weight 600, line height 1.44. Lead paragraphs.
- **body-sm:** Inter 12px at weight 300, line height 2. Secondary and small text.
- **label-md:** Inter 16px at weight 400, line height 1. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 600, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (77% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 5px, md 16px, lg 20px, xl 36px.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Breakpoints:** 600px, 767px, 1024px, 1279px, 1439px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.16) 0px 1px 4px 0px, rgba(27, 28, 29, 0.2) 0px 7px 29px 0px`
- `rgba(10, 96, 255, 0.3) 0px 0px 20px 0px`

## Shapes

Most elements use 48px corners. Measured radii, most used first:

- **lg (48px):** 72 elements.
- **sm (4px):** 48 elements.
- **md (8px):** 24 elements.
- **xl (120px):** 12 elements.
- **full (9999px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Open chat”):** #058103 fill, #FFFFFF text, 16px/400, 50% radius, padding 0px.
- **button-secondary (“Watch video (01:33)”):** #FFFFFF fill, #07182D text, 16px/600, 48px radius, padding 10px 20px.
- **button-outline (“What's new”):** transparent fill, #FFFFFF text, 16px/600, 48px radius, padding 10px 20px, border 1px solid #FFFFFF.
- **button-ghost (“Products and Services”):** transparent fill, #07182D text, 14px/400, padding 0px.
- **link:** transparent fill, #536070 text, padding 0px.

## Do's and Don'ts

- Do use #000000 for the page.
- Do keep text in 2 levels: #FFFFFF, #536070.
- Do reserve #058103 for primary actions and key highlights.
- Do reuse the measured spacing steps (5px, 16px, 20px).
- Do use 48px corners on most elements; larger surfaces also use 4px, 8px and 120px.
- Don't use #536070 for body text; it reaches 3.27:1 on #000000. Keep it for large text or metadata.
- Don't introduce new font families beyond Inter.
- Don't use #058103 for large backgrounds or body text.
- Don't make interface transitions slower than 0.6s.

## Motion

Interface transitions are quick: 0.144s, 0.3s, 0.6s, 0.5s. Longer ambient animations run 0.8s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease`, `ease-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/cisco.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
