---
version: alpha
name: GitHub
description: "Light interface measured from github.com: Mona Sans type with Mona Sans VF, dark green accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#58635B"
  surface-container-low: "#F9FBF9"
  surface-container: "#F2F5F3"
  surface-container-high: "#D6E8DB"
  overlay: "#0000000F"
  outline: "#D2D9D4"
  outline-variant: "#E4EBE6"
  primary: "#08872B"
  on-primary: "#FFFFFF"
  inverse-surface: "#77827A"
  secondary: "#0377FF"
  tertiary: "#8534F3"
  success: "#23EA57"
typography:
  headline-display:
    fontFamily: Mona Sans
    fontSize: 56px
    fontWeight: 440
    lineHeight: 1.1
  headline-lg:
    fontFamily: Mona Sans
    fontSize: 40px
    fontWeight: 400
    lineHeight: 1.2
  headline-md:
    fontFamily: Mona Sans
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.35
  headline-sm:
    fontFamily: Mona Sans VF
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.5
  title-lg:
    fontFamily: Mona Sans
    fontSize: 22px
    fontWeight: 400
    lineHeight: 1.4
  body-md:
    fontFamily: Mona Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Mona Sans
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.01em
  body-sm:
    fontFamily: Mona Sans VF
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.3
  label-md:
    fontFamily: Mona Sans VF
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  code:
    fontFamily: Mona Sans Mono
    fontSize: 14px
    fontWeight: 480
    lineHeight: 1.5
  headline-display-mobile:
    fontFamily: Mona Sans
    fontSize: 36px
    fontWeight: 440
    lineHeight: 1.2
rounded:
  sm: 4px
  md: 6px
  lg: 8px
  xl: 24px
  full: 9999px
spacing:
  xs: 2.1px
  sm: 8px
  md: 12px
  lg: 24px
  gutter: 12px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 6px 20px
    height: 43px
  button-primary-hover:
    backgroundColor: "#077124"
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    padding: 8px
    height: 46px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: 0px 12px
    height: 32px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px 8px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 16px 12px 0px 16px
  link:
    textColor: "{colors.on-surface}"
---

# GitHub Design System

## Overview

GitHub describes itself as: “Join the world's most widely adopted, AI-powered developer platform where millions of developers, businesses, and the largest open source community build software that advances humanity.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Dark Green (#08872B)** as the main accent.

Type is set in **Mona Sans** and **Mona Sans VF**, with **Mona Sans Mono** for code. Headlines run large; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [github.com](https://github.com/) on October 29, 2026 at 1440×900 and 390×844 from 447 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 15 roles.

- **White (#FFFFFF):** Page background, seen 5 times. Token `background`, CSS `--bgColor-white`.
- **Near Black (#000000):** Primary text and headings, seen 57 times. Token `on-surface`, CSS `--brand-Testimonial-quote-color-default`.
- **Slate (#58635B):** Secondary text, seen 24 times. Token `on-surface-variant`.
- **Snow (#F9FBF9):** Raised areas one step from the page, seen 3 times. Token `surface-container-low`.
- **Mist (#F2F5F3):** Cards and panels, seen 15 times. Token `surface-container`, CSS `--brand-videoPlayer-title-fgColor`.
- **Pale Green (#D6E8DB):** Hover and pressed fills, seen 8 times. Token `surface-container-high`.
- **Near Black 6% (#0000000F):** Translucent fill for cards and controls, seen 9 times. Token `overlay`.
- **Silver (#D2D9D4):** Borders and dividers, seen 29 times. Token `outline`.
- **Mist (#E4EBE6):** Secondary dividers, seen 19 times. Token `outline-variant`.
- **Dark Green (#08872B):** Primary buttons and calls to action, seen 22 times. Token `primary`, CSS `--brand-Label-color-green-blue-start`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Slate (#77827A):** High-contrast fills, seen 4 times. Token `inverse-surface`.
- **Vivid Blue (#0377FF):** Accent (CSS variable), seen 1 time. Token `secondary`, CSS `--brand-Eyebrowbanner-fgColor-green-blue-end`.
- **Vivid Violet (#8534F3):** Accent in text, fills and borders, seen 10 times. Token `tertiary`.
- **Vivid Green (#23EA57):** Success and positive states, seen 8 times. Token `success`.

## Typography

**Mona Sans**, **Mona Sans VF** and **Mona Sans Mono** (monospace) share the interface. Fallback stack: `Mona Sans, MonaSansFallback, -apple-system, BlinkMacSystemFont`.

- **headline-display:** Mona Sans 56px at weight 440, line height 1.1 (36px on mobile). Page title (h1).
- **headline-lg:** Mona Sans 40px at weight 400, line height 1.2. Section headings (h2).
- **headline-md:** Mona Sans 28px at weight 400, line height 1.35. Sub-section headings.
- **headline-sm:** Mona Sans VF 24px at weight 600, line height 1.5. Card and feature titles.
- **title-lg:** Mona Sans 22px at weight 400, line height 1.4. Small titles.
- **body-md:** Mona Sans 14px at weight 400, line height 1.5. Body text.
- **body-lg:** Mona Sans 18px at weight 400, line height 1.5, tracking 0.01em. Lead paragraphs.
- **body-sm:** Mona Sans VF 12px at weight 400, line height 1.3. Secondary and small text.
- **label-md:** Mona Sans VF 14px at weight 400, line height 1.5. Buttons, navigation and labels.
- **code:** Mona Sans Mono 14px at weight 480, line height 1.5. Code and technical values.

## Layout

Spacing is mostly on a 4px grid (84% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 2.1px, sm 8px, md 12px, lg 24px.
- **Gaps:** 12px is the most common gap in flex and grid layouts.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F9FBF9 → #F2F5F3 → #D6E8DB) and #D2D9D4 borders.

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **md (6px):** 68 elements.
- **full (9999px):** 40 elements.
- **sm (4px):** 32 elements.
- **xl (24px):** 20 elements.
- **lg (8px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Sign up for GitHub”):** #08872B fill, #FFFFFF text, 14px/400, 6px radius, padding 6px 20px.
- **button-primary-hover:** background #077124, text #FFFFFF on hover.
- **button-outline (“GitHub Universe ‘26 Recap”):** #F9FBF9 fill, #000000 text, 14px/400, 9999.01px radius, padding 8px, border 1px solid #E4EBE6.
- **button-secondary (“Sign up”):** #000000 fill, #FFFFFF text, 16px/400, 6px radius, padding 0px 12px.
- **button-ghost (“Products”):** transparent fill, #000000 text, 14px/400, 24px radius, padding 0px 8px.
- **input-field (“you@domain.com”):** transparent fill, #000000 text, 14px/400, 8px radius, padding 16px 12px 0px 16px.
- **link:** transparent fill, #000000 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F9FBF9, #F2F5F3, #D6E8DB.
- Do keep text in 2 levels: #000000, #58635B.
- Do reserve #08872B for primary actions and key highlights.
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 6px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Mona Sans, Mona Sans VF and Mona Sans Mono.
- Don't use #08872B for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.2s, 0.3s, 0.08s. Longer ambient animations run 1.4s.

- **Easing:** `ease`, `cubic-bezier(0.16, 1, 0.3, 1)`, `cubic-bezier(0.4, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/github.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
