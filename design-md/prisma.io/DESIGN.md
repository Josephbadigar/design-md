---
version: alpha
name: Prisma
description: "Light monochrome interface measured from prisma.io: Sora type with Inter, tonal surfaces and 8px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#3A3B3C"
  on-background: "#3A3B3C"
  on-surface-strong: "#151515"
  on-surface-variant: "#646567"
  on-surface-muted: "#929394"
  surface-container-low: "#EEFFFF"
  surface-container: "#DCFDFF"
  surface-container-high: "#F4F7F7"
  surface-container-highest: "#E5E5E5"
  overlay: "#3A3B3C1A"
  overlay-strong: "#F5F5F599"
  outline: "#E5E5E5"
  outline-variant: "#0000000F"
  primary: "#000000"
  on-primary: "#FFFFFF"
  secondary: "#01D7E4"
  tertiary: "#006772"
typography:
  headline-display:
    fontFamily: Sora
    fontSize: 62px
    fontWeight: 500
    lineHeight: 1.06
  headline-lg:
    fontFamily: Sora
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.1
  headline-md:
    fontFamily: Sora
    fontSize: 30px
    fontWeight: 500
    lineHeight: 1.2
  headline-sm:
    fontFamily: Sora
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.33
  title-lg:
    fontFamily: Sora
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.4
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 380
    lineHeight: 1.43
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 380
    lineHeight: 1.5
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 380
    lineHeight: 1
  caption:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: 380
    lineHeight: 1
  label-lg:
    fontFamily: Sora
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.5
  label-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.63
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.63
  headline-display-mobile:
    fontFamily: Sora
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.06
  headline-lg-mobile:
    fontFamily: Sora
    fontSize: 34px
    fontWeight: 500
    lineHeight: 1.1
rounded:
  xs: 6px
  sm: 8px
  md: 10px
  lg: 14px
  xl: 18px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 10px
  lg: 24px
  xl: 64px
  gutter: 10px
  section: 128px
  margin: 32px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    padding: 12px 24px
    height: 48px
  button-secondary:
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "#F9FAF5"
    typography: "{typography.body-md}"
    padding: 8px 16px
    height: 36px
  button-tertiary:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 8px 16px
    height: 36px
  button-ghost:
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 0px
  card:
    textColor: "{colors.on-surface}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.xl}"
    padding: 0px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Prisma Design System

## Overview

Prisma describes itself as: “Prisma Compute hosts TypeScript apps (Node.js, Bun or Next.js) next to Prisma Postgres in one project. Generally available since August 2026. Free plan, no credit card. Any Postgres client works; Prisma ORM is optional. ” The interface is light, built on **White (#FFFFFF)** with **Graphite (#3A3B3C)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **Sora** and **Inter**. Headlines run large; body text is 14px. Depth comes from soft drop shadows. Corners are mostly 8px.

Measured from [prisma.io](https://www.prisma.io/) on October 29, 2026 at 1440×900 and 390×844 from 414 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 17 roles, plus gradient stops #01D7E4, #F3C306, #F37A03, #F00E5C.

- **White (#FFFFFF):** Page background, seen 52 times. Token `background`, CSS `--tw-ring-offset-color`.
- **Graphite (#3A3B3C):** Primary text and headings, seen 42 times. Token `on-surface`, CSS `--card-foreground`.
- **Charcoal (#151515):** Headings and emphasis, seen 27 times. Token `on-surface-strong`.
- **Slate (#646567):** Secondary text, seen 62 times. Token `on-surface-variant`.
- **Gray (#929394):** Muted text and metadata, seen 4 times. Token `on-surface-muted`.
- **Cool Snow (#EEFFFF):** Raised areas one step from the page, seen 1 time. Token `surface-container-low`, CSS `--color-prism-cyan-50`.
- **Pale Cyan (#DCFDFF):** Cards and panels, seen 4 times. Token `surface-container`.
- **Snow (#F4F7F7):** Hover and pressed fills, seen 4 times. Token `surface-container-high`.
- **Mist (#E5E5E5):** Highest raised elements, seen 4 times. Token `surface-container-highest`.
- **Graphite 10% (#3A3B3C1A):** Translucent fill for cards and controls, seen 12 times. Token `overlay`.
- **Snow 60% (#F5F5F599):** Stronger translucent fill, seen 3 times. Token `overlay-strong`.
- **Mist (#E5E5E5):** Borders and dividers, seen 20 times. Token `outline`.
- **Near Black 6% (#0000000F):** Secondary dividers, seen 15 times. Token `outline-variant`.
- **Near Black (#000000):** Primary buttons and calls to action, seen 3 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Vivid Cyan (#01D7E4):** Accent in text, fills and borders, seen 9 times. Token `secondary`.
- **Dark Cyan (#006772):** Accent in text, fills and borders, seen 3 times. Token `tertiary`.

## Typography

**Sora** and **Inter** share the interface. Fallback stack: `Sora, Sora Fallback`.

- **headline-display:** Sora 62px at weight 500, line height 1.06 (40px on mobile). Page title (h1).
- **headline-lg:** Sora 48px at weight 500, line height 1.1 (34px on mobile). Section headings (h2).
- **headline-md:** Sora 30px at weight 500, line height 1.2. Sub-section headings.
- **headline-sm:** Sora 24px at weight 500, line height 1.33. Card and feature titles.
- **title-lg:** Sora 20px at weight 500, line height 1.4. Small titles.
- **body-md:** Inter 14px at weight 380, line height 1.43. Body text.
- **body-lg:** Inter 16px at weight 380, line height 1.5. Lead paragraphs.
- **body-sm:** Inter 12px at weight 380, line height 1. Secondary and small text.
- **caption:** Inter 10px at weight 380, line height 1. Captions and fine print.
- **label-lg:** Sora 16px at weight 500, line height 1.5. Large buttons and tabs.
- **label-md:** Inter 15px at weight 600, line height 1.63. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 500, line height 1.63. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 63% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 10px, lg 24px, xl 64px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 10px is the most common gap in flex and grid layouts.
- **Page margin:** 32px on each side of full-width sections.
- **Breakpoints:** 350px, 601px, 639px, 750px, 940px, 961px, 1124px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.1) 0px 1px 2px -1px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(21, 21, 21, 0.16) 0px 8px 24px -12px`
- `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(21, 21, 21, 0.04) 0px 1px 2px 0px, rgba(21, 21, 21, 0.1) 0px 8px 16px -8px`

## Shapes

Most elements use 8px corners. Measured radii, most used first:

- **sm (8px):** 116 elements.
- **xl (18px):** 49 elements.
- **md (10px):** 32 elements.
- **lg (14px):** 28 elements.
- **xs (6px):** 12 elements.
- **full (9999px):** 4 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get started free”):** #000000 fill, #FFFFFF text, 16px/380, 3.35544e+07px radius, padding 12px 24px.
- **button-secondary (“Get Started”):** #151515 fill, #F9FAF5 text, 14px/600, 3.35544e+07px radius, padding 8px 16px.
- **button-tertiary (“Log in”):** transparent fill, #3A3B3C text, 14px/600, 3.35544e+07px radius, padding 8px 16px.
- **button-ghost (“Platform”):** transparent fill, #646567 text, 14px/500, 8px radius, padding 0px.
- **card:** transparent fill, #3A3B3C text, 16px/380, 18px radius, padding 0px, shadow `rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(21, 21, 21, 0.04) 0px 1px 2px 0px, rgba(21, 21, 21, 0.06) 0px 8px 16px -4px, rgba(21, 21, 21, 0.14) 0px 32px 64px -16px`.
- **link:** transparent fill, #646567 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #EEFFFF, #DCFDFF, #F4F7F7, #E5E5E5.
- Do keep text in 4 levels: #3A3B3C, #151515, #646567, #929394.
- Do let contrast carry emphasis; primary actions use #000000 on #FFFFFF.
- Do reuse the measured spacing steps (8px, 10px, 24px).
- Do use 8px corners on most elements; larger surfaces also use 18px, 10px and 14px.
- Don't use #929394 for body text; it reaches 3.08:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Sora and Inter.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.15s, 0.3s, 0.5s. Longer ambient animations run 2.2s, 7s, 2.6s.

- **Easing:** `cubic-bezier(0.4, 0, 0.2, 1)`, `ease-in-out`, `linear`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/prisma.io/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
