---
version: alpha
name: Semrush
description: "Light interface measured from semrush.com: Lazzer type, light violet accents, tonal surfaces and 100px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#181E15"
  on-background: "#181E15"
  on-surface-variant: "#6C6E79"
  surface-container-low: "#F3F6F6"
  surface-container: "#F0F1F2"
  surface-container-high: "#DCEEEB"
  overlay: "#FFFFFF0D"
  primary: "#C190FF"
  on-primary: "#181E15"
  secondary: "#18F0BF"
typography:
  headline-display:
    fontFamily: Lazzer
    fontSize: 84px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Lazzer
    fontSize: 64px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.04em
  headline-md:
    fontFamily: Lazzer
    fontSize: 48px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: -0.04em
  headline-sm:
    fontFamily: Lazzer
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.04em
  title-lg:
    fontFamily: Lazzer
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-md:
    fontFamily: Lazzer
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.018em
  body-sm:
    fontFamily: Lazzer
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1
  label-lg:
    fontFamily: Lazzer
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: -0.02em
  label-md:
    fontFamily: Lazzer
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
  label-sm:
    fontFamily: Lazzer
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: 0.02em
  headline-display-mobile:
    fontFamily: Lazzer
    fontSize: 52px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: -0.04em
rounded:
  sm: 5px
  md: 10px
  lg: 100px
spacing:
  xs: 4px
  sm: 6px
  md: 12px
  lg: 32px
  xl: 64px
  gutter: 16px
  section: 120px
  margin: 24px
  container: 1440px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 32px
    height: 60px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.background}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 16px 24px
    height: 48px
  button-secondary-hover:
    backgroundColor: "#B072FF"
    textColor: "{colors.on-surface}"
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.lg}"
    padding: 0px 32px
    height: 60px
  button-ghost:
    textColor: "#006DCA"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 1px 6px
  input-field:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: 0px
    padding: 0px
  link:
    textColor: "{colors.on-surface}"
---

# Semrush Design System

## Overview

Semrush describes itself as: “Semrush is the leading platform to grow and measure brand visibility across AI search, SEO, PPC, social, and more.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#181E15)** text, and **Light Violet (#C190FF)** as the main accent.

Type is set in **Lazzer**. Headlines run large with tight negative tracking; body text is 18px. Depth comes from soft drop shadows. Corners are mostly 100px.

Measured from [semrush.com](https://www.semrush.com/) on November 4, 2026 at 1440×900 and 390×844 from 346 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **White (#FFFFFF):** Page background, seen 4 times. Token `background`, CSS `--mp-white`.
- **Charcoal (#181E15):** Primary text and headings, seen 156 times. Token `on-surface`, CSS `--mp-off-black`.
- **Cool Slate (#6C6E79):** Secondary text, seen 4 times. Token `on-surface-variant`, CSS `--mp-dark-grey`.
- **Snow (#F3F6F6):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`, CSS `--mp-off-white`.
- **Mist (#F0F1F2):** Cards and panels, seen 4 times. Token `surface-container`, CSS `--mp-light-grey`.
- **Pale Teal (#DCEEEB):** Hover and pressed fills, seen 10 times. Token `surface-container-high`, CSS `--mp-mint`.
- **White 5% (#FFFFFF0D):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Light Violet (#C190FF):** Brand color on large areas, seen 11 times. Token `primary`, CSS `--mp-lavendar`.
- **Charcoal (#181E15):** Text and icons on primary. Token `on-primary`.
- **Vivid Teal (#18F0BF):** Accent in text, fills and borders, seen 6 times. Token `secondary`, CSS `--mp-aqua`.

## Typography

**Lazzer** carries the whole interface. Fallback stack: `Lazzer, sans-serif`. Other loaded fonts: Inter.

- **headline-display:** Lazzer 84px at weight 600, line height 1.1, tracking -0.04em (52px on mobile). Page title (h1).
- **headline-lg:** Lazzer 64px at weight 600, line height 1.1, tracking -0.04em. Section headings (h2).
- **headline-md:** Lazzer 48px at weight 600, line height 1, tracking -0.04em. Sub-section headings.
- **headline-sm:** Lazzer 40px at weight 600, line height 1.2, tracking -0.04em. Card and feature titles.
- **title-lg:** Lazzer 24px at weight 600, line height 1.2, tracking -0.02em. Small titles.
- **body-md:** Lazzer 18px at weight 500, line height 1.5, tracking -0.018em. Body text.
- **body-sm:** Lazzer 12px at weight 400, line height 1. Secondary and small text.
- **label-lg:** Lazzer 16px at weight 500, line height 1.5, tracking -0.02em. Large buttons and tabs.
- **label-md:** Lazzer 14px at weight 500, line height 1. Buttons, navigation and labels.
- **label-sm:** Lazzer 12px at weight 600, line height 1, tracking 0.02em. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (73% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 6px, md 12px, lg 32px, xl 64px.
- **Sections:** 120px vertical padding between major sections.
- **Gaps:** 16px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1440px.
- **Page margin:** 24px on each side of full-width sections.
- **Breakpoints:** 480px, 767px, 768px, 1024px, 1440px, 1600px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.05) 0px 2px 12px 0px`

Hairline rings and inset highlights also appear: `rgba(0, 0, 0, 0.05) 0px 4px 15px 0px inset`.

## Shapes

Most elements use 100px corners. Measured radii, most used first:

- **lg (100px):** 92 elements.
- **sm (5px):** 54 elements.
- **md (10px):** 20 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get insights”):** #C190FF fill, #181E15 text, 16px/600, 100px radius, padding 0px 32px.
- **button-secondary (“Start for free”):** #181E15 fill, #FFFFFF text, 16px/600, 100px radius, padding 16px 24px.
- **button-secondary-hover:** background #B072FF, text #181E15 on hover.
- **button-outline (“Try for free”):** #FFFFFF fill, #181E15 text, 16px/600, 100px radius, padding 0px 32px, border 1px solid #FFFFFF.
- **button-ghost (“Skip to content”):** transparent fill, #006DCA text, 16px/400, padding 1px 6px.
- **input-field (“Enter your website”):** transparent fill, #181E15 text, 16px/500, padding 0px.
- **link:** transparent fill, #181E15 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F3F6F6, #F0F1F2, #DCEEEB.
- Do keep text in 2 levels: #181E15, #6C6E79.
- Do use #C190FF as the brand accent: header, logo and key highlights.
- Do set headlines in Lazzer with tight tracking (-0.04em).
- Do reuse the measured spacing steps (6px, 12px, 32px).
- Do use 100px corners on most elements; larger surfaces also use 5px and 10px.
- Don't introduce new font families beyond Lazzer.
- Don't use #C190FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.42s.

## Motion

Interface transitions are quick: 0.2s, 0.42s, 0.1s, 0.4s.

- **Easing:** `ease-in-out`, `ease`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/semrush.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
