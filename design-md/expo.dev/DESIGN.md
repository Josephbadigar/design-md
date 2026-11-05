---
version: alpha
name: Expo
description: "Light monochrome interface measured from expo.dev: Inter type, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1C2024"
  on-background: "#1C2024"
  on-surface-variant: "#60646C"
  surface-container-low: "#FCFCFD"
  surface-container: "#F0F0F3"
  surface-container-high: "#E0E1E6"
  overlay: "#F9F9FBCC"
  outline: "#E0E1E6"
  outline-variant: "#D9D9E0"
  primary: "#000000"
  on-primary: "#FFFFFF"
  secondary: "#0D74CE"
  tertiary: "#0588F0"
typography:
  headline-display:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.042em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.016em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.021em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.63
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.4
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1
  label-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.4
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.4
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.6
  code:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: -0.042em
  headline-display-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.021em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.021em
rounded:
  xs: 16px
  sm: 24px
  md: 32px
  lg: 36px
  xl: 40px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 40px
  gutter: 24px
  section: 200px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.lg}"
    padding: 0px 16px
    height: 36px
  button-primary-hover:
    backgroundColor: "{colors.on-surface-variant}"
  button-outline:
    backgroundColor: "{colors.surface-container}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px 16px
    height: 40px
  button-outline-hover:
    backgroundColor: "#E8E8EC"
  button-ghost:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.full}"
    padding: 4px 10px 4px 4px
    height: 32px
  card:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: 20px
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Expo Design System

## Overview

Expo describes itself as: “Develop, validate, deploy and monitor iOS, Android, and web apps from one codebase. Expo gives your team and its agents the infrastructure to ship apps to production.” The interface is light, built on **White (#FFFFFF)** with **Cool Charcoal (#1C2024)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Inter**, with **JetBrains Mono** for code. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [expo.dev](https://expo.dev/) on November 4, 2026 at 1440×900 and 390×844 from 393 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 23 times. Token `background`, CSS `--expo-theme-button-primary-destructive-text`.
- **Cool Charcoal (#1C2024):** Primary text and headings, seen 73 times. Token `on-surface`, CSS `--expo-theme-button-secondary-text`.
- **Cool Slate (#60646C):** Secondary text, seen 72 times. Token `on-surface-variant`.
- **Snow (#FCFCFD):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **Mist (#F0F0F3):** Cards and panels, seen 4 times. Token `surface-container`.
- **Cool Mist (#E0E1E6):** Hover and pressed fills, seen 1 time. Token `surface-container-high`.
- **Snow 80% (#F9F9FBCC):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Cool Mist (#E0E1E6):** Borders and dividers, seen 17 times. Token `outline`.
- **Cool Silver (#D9D9E0):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **Near Black (#000000):** Primary buttons and calls to action, seen 7 times. Token `primary`, CSS `--tw-mask-bottom-from-color`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Blue (#0D74CE):** Accent in text, fills and borders, seen 6 times. Token `secondary`, CSS `--expo-theme-text-link`.
- **Vivid Blue (#0588F0):** Accent on large areas. Token `tertiary`.

## Typography

**Inter** and **JetBrains Mono** (monospace) share the interface. Fallback stack: `Inter, -apple-system, system-ui, sans-serif`.

- **headline-display:** Inter 48px at weight 600, line height 1.1, tracking -0.042em (24px on mobile). Page title (h1).
- **headline-lg:** Inter 32px at weight 600, line height 1.1, tracking -0.016em (24px on mobile). Section headings (h2).
- **headline-md:** Inter 24px at weight 600, line height 1.2, tracking -0.021em. Sub-section headings.
- **body-md:** Inter 14px at weight 400, line height 1.63. Body text.
- **body-lg:** Inter 16px at weight 400, line height 1.4. Lead paragraphs.
- **body-sm:** Inter 12px at weight 400, line height 1. Secondary and small text.
- **label-lg:** Inter 16px at weight 500, line height 1.4. Large buttons and tabs.
- **label-md:** Inter 14px at weight 500, line height 1.4. Buttons, navigation and labels.
- **label-sm:** Inter 12px at weight 500, line height 1.6. Small labels and badges.
- **code:** JetBrains Mono 12px at weight 500, line height 1, tracking -0.042em. Code and technical values.

## Layout

Spacing follows a 4px grid: 94% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 16px, lg 32px, xl 40px.
- **Sections:** 200px vertical padding between major sections.
- **Gaps:** 24px is the most common gap in flex and grid layouts.
- **Breakpoints:** 468px, 767px, 787px, 788px, 900px, 1008px, 1024px, 1159px, 1200px, 1328px, 1572px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.08) 0px 3px 6px 0px, rgba(0, 0, 0, 0.07) 0px 2px 4px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 5px 10px 0px, rgba(0, 0, 0, 0.12) 0px 15px 25px 0px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.12) 0px 15px 25px 0px, rgba(0, 0, 0, 0.05) 0px 5px 10px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **xs (16px):** 68 elements.
- **full (9999px):** 56 elements.
- **xl (40px):** 28 elements.
- **lg (36px):** 24 elements.
- **md (32px):** 20 elements.
- **sm (24px):** 16 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up”):** #000000 fill, #FFFFFF text, 14px/500, 36px radius, padding 0px 16px.
- **button-primary-hover:** background #60646C, text #FFFFFF on hover.
- **button-outline (“Talk to our team”):** #F0F0F3 fill, #1C2024 text, 14px/600, 40px radius, padding 0px 16px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px`.
- **button-outline-hover:** background #E8E8EC, text #1C2024 on hover.
- **button-ghost (“New Try Observe”):** #F9F9FBCC fill, #1C2024 text, 16px/400, 9999px radius, padding 4px 10px 4px 4px, border 1px solid #D9D9E0.
- **card:** #FCFCFD fill, #1C2024 text, 16px/400, 20px radius, padding 0px, border 1px solid #E8E8EC, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.12) 0px 15px 25px 0px, rgba(0, 0, 0, 0.05) 0px 5px 10px 0px`.
- **link:** transparent fill, #60646C text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #FCFCFD, #F0F0F3, #E0E1E6.
- Do keep text in 2 levels: #1C2024, #60646C.
- Do let contrast carry emphasis; primary actions use #000000 on #FFFFFF.
- Do set headlines in Inter with tight tracking (-0.042em).
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 16px corners.
- Don't introduce new font families beyond Inter and JetBrains Mono.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.15s, 0.3s. Longer ambient animations run 2.2s, 11s, 14s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in-out`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/expo.dev/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
