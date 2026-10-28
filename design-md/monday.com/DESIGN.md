---
version: alpha
name: monday.com
description: "Light interface measured from monday.com: Poppins type, indigo accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#000000"
  on-background: "#000000"
  on-surface-variant: "#535768"
  on-surface-muted: "#585965"
  on-surface-subtle: "#7C7B7B"
  surface-container-low: "#F3F4F5"
  surface-container: "#CCCCCC"
  outline: "#E6E7EAB3"
  outline-variant: "#F3F4F5"
  primary: "#6161FF"
  on-primary: "#FFFFFF"
  secondary: "#00C875"
  tertiary: "#4A3AFF"
typography:
  headline-display:
    fontFamily: Poppins
    fontSize: 128px
    fontWeight: 500
    lineHeight: 0.8
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Poppins
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: -0.03em
  headline-md:
    fontFamily: Poppins
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Poppins
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: -0.02em
  body-md:
    fontFamily: Poppins
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.43
  body-lg:
    fontFamily: Poppins
    fontSize: 16px
    fontWeight: 300
    lineHeight: 1
  body-sm:
    fontFamily: Poppins
    fontSize: 13px
    fontWeight: 300
  label-md:
    fontFamily: Poppins
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.25
  headline-lg-mobile:
    fontFamily: Poppins
    fontSize: 32px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.04em
  headline-md-mobile:
    fontFamily: Poppins
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.02em
rounded:
  xs: 16px
  sm: 24px
  md: 28px
  lg: 32px
  xl: 160px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 48px
  gutter: 8px
  container: 1372px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.xl}"
    padding: 14px 32px
    height: 50px
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xl}"
    padding: 12px 16px
    height: 42px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "#323338"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 8px 12px
    height: 32px
  button-outline-hover:
    backgroundColor: "#E6E7EA"
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 12px
---

# monday.com Design System

## Overview

monday.com describes itself as: “Get more work done with AI agents that work side by side with your people. Execute, manage, and operate together on one AI Workspace to drive business results.” The interface is light, built on **White (#FFFFFF)** with **Near Black (#000000)** text, and **Indigo (#6161FF)** as the main accent.

Type is set in **Poppins**. Headlines run large with tight negative tracking; body text is 14px. Depth comes from soft drop shadows. Controls are pill-shaped.

Measured from [monday.com](https://monday.com/) on October 21, 2026 at 1440×900 and 390×844 from 333 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles, plus gradient stops #FE9B0BD9, #FF81E4D9.

- **White (#FFFFFF):** Page background, seen 17 times. Token `background`, CSS `--text-color--white`.
- **Near Black (#000000):** Primary text and headings, seen 31 times. Token `on-surface`, CSS `--text-color--black`.
- **Dark Indigo (#535768):** Secondary text, seen 3 times. Token `on-surface-variant`.
- **Cool Slate (#585965):** Muted text and metadata, seen 44 times. Token `on-surface-muted`.
- **Slate (#7C7B7B):** Subtle text and placeholders, seen 10 times. Token `on-surface-subtle`, CSS `--clay--grey-ink`.
- **Snow (#F3F4F5):** Raised areas one step from the page, seen 15 times. Token `surface-container-low`, CSS `--surface-light`.
- **Silver (#CCCCCC):** Cards and panels, seen 4 times. Token `surface-container`.
- **Mist 70% (#E6E7EAB3):** Borders and dividers, seen 14 times. Token `outline`.
- **Snow (#F3F4F5):** Secondary dividers, seen 7 times. Token `outline-variant`, CSS `--surface-light`.
- **Indigo (#6161FF):** Primary buttons and calls to action, seen 10 times. Token `primary`, CSS `--_agents---agent-03`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Teal (#00C875):** Brand accent (CSS variable), seen 24 times. Token `secondary`.
- **Vivid Indigo (#4A3AFF):** Brand accent (CSS variable), seen 12 times. Token `tertiary`.

## Typography

**Poppins** carries the whole interface. Fallback stack: `Poppins, Arial, sans-serif`.

- **headline-display:** Poppins 128px at weight 500, line height 0.8, tracking -0.04em. Page title (h1).
- **headline-lg:** Poppins 56px at weight 400, line height 1.2, tracking -0.03em (32px on mobile). Section headings (h2).
- **headline-md:** Poppins 44px at weight 400, line height 1.1, tracking -0.02em (24px on mobile). Sub-section headings.
- **headline-sm:** Poppins 24px at weight 400, line height 1.4, tracking -0.02em. Card and feature titles.
- **body-md:** Poppins 14px at weight 400, line height 1.43. Body text.
- **body-lg:** Poppins 16px at weight 300, line height 1. Lead paragraphs.
- **body-sm:** Poppins 13px at weight 300. Secondary and small text.
- **label-md:** Poppins 16px at weight 400, line height 1.25. Buttons, navigation and labels.

## Layout

Spacing is mostly on a 4px grid (89% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 48px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Container:** content is capped at 1372px.
- **Breakpoints:** 479px, 767px, 768px, 991px.

## Elevation & Depth

Raised elements use soft drop shadows. The most used recipes:

- `rgba(0, 0, 0, 0.1) 0px 1.5px 8px 0px`

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 112 elements.
- **xl (160px):** 72 elements.
- **sm (24px):** 44 elements.
- **xs (16px):** 36 elements.
- **lg (32px):** 28 elements.
- **md (28px):** 24 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started”):** #6161FF fill, #FFFFFF text, 16px/400, 160px radius, padding 14px 32px.
- **button-secondary (“Get Started”):** #6161FF fill, #FFFFFF text, 13px/300, 160px radius, padding 12px 16px, border 1px solid #6161FF.
- **button-outline (“Operations”):** #F3F4F5 fill, #323338 text, 14px/400, 32px radius, padding 8px 12px, border 1px solid #F3F4F5.
- **button-outline-hover:** background #E6E7EA, text #323338 on hover.
- **card:** #FFFFFF fill, #FFFFFF text, 16px/400, 24px radius, padding 12px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F3F4F5, #CCCCCC.
- Do keep text in 4 levels: #000000, #535768, #585965, #7C7B7B.
- Do reserve #6161FF for primary actions and key highlights.
- Do set headlines in Poppins with tight tracking (-0.04em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do make buttons and chips fully rounded (9999px); most other elements use 160px corners.
- Don't use #7C7B7B for body text; it reaches 4.2:1 on #FFFFFF. Keep it for large text or metadata.
- Don't introduce new font families beyond Poppins.
- Don't use #6161FF for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.25s, 0.4s, 0.2s, 0.5s. Longer ambient animations run 6s.

- **Easing:** `ease`, `ease-in-out`, `cubic-bezier(0.731, -0.238, 0.257, 1.224)`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/monday.com/), the free DESIGN.md generator.
