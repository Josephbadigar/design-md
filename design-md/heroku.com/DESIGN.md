---
version: alpha
name: Heroku
description: "Light interface measured from heroku.com: Avant Garde type with Salesforce Sans, blue accents, tonal surfaces and 4px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#181818"
  on-background: "#181818"
  on-surface-variant: "#240643"
  on-surface-muted: "#333D47"
  on-surface-subtle: "#A998BF"
  surface-container-low: "#F9F9FB"
  surface-container: "#EEF1F6"
  overlay: "#FFFFFF99"
  outline: "#DDDDDD"
  outline-variant: "#79589F80"
  primary: "#0176D3"
  on-primary: "#FFFFFF"
  secondary: "#300B60"
  tertiary: "#5A1BA9"
typography:
  headline-display:
    fontFamily: Avant Garde
    fontSize: 40px
    fontWeight: 600
    lineHeight: 1.2
  headline-lg:
    fontFamily: Avant Garde
    fontSize: 32px
    fontWeight: 600
    lineHeight: 1.25
  headline-md:
    fontFamily: Salesforce Sans
    fontSize: 25px
    fontWeight: 400
    lineHeight: 1
  headline-sm:
    fontFamily: Avant Garde
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.33
  title-lg:
    fontFamily: Salesforce Sans
    fontSize: 20px
    fontWeight: 700
    lineHeight: 1.4
  body-md:
    fontFamily: Salesforce Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  body-lg:
    fontFamily: Salesforce Sans
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.28
  body-sm:
    fontFamily: BentonSans
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.33
  caption:
    fontFamily: BentonSans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
  label-lg:
    fontFamily: Salesforce Sans
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: -0.002em
  label-md:
    fontFamily: Salesforce Sans
    fontSize: 15px
    fontWeight: 700
    lineHeight: 1
  label-sm:
    fontFamily: Salesforce Sans
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: 0.05em
  headline-display-mobile:
    fontFamily: Avant Garde
    fontSize: 30px
    fontWeight: 600
    lineHeight: 1.3
rounded:
  md: 4px
spacing:
  xs: 2px
  sm: 5px
  md: 10px
  lg: 30px
  xl: 35px
  gutter: 30px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.md}"
    padding: 12px 32px
    height: 52px
  button-primary-hover:
    backgroundColor: "#0B5CAB"
  button-ghost:
    textColor: "{colors.on-primary}"
    typography: "{typography.caption}"
    rounded: 3px
    padding: 11px 16px
  link:
    textColor: "{colors.on-surface-variant}"
---

# Heroku Design System

## Overview

Heroku describes itself as: “Experience fully managed app hosting that just works. Build, deploy, and scale on the battle-tested platform that defines the industry.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#181818)** text, and **Blue (#0176D3)** as the main accent.

Type is set in **Avant Garde** and **Salesforce Sans**. Headlines run large; body text is 16px. The surface language is flat. Corners are mostly 4px.

Measured from [heroku.com](https://www.heroku.com/) on November 4, 2026 at 1440×900 and 390×844 from 357 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 14 roles, plus gradient stops #300B60, #5A1BA9.

- **White (#FFFFFF):** Page background, seen 8 times. Token `background`.
- **Charcoal (#181818):** Primary text and headings, seen 39 times. Token `on-surface`.
- **Deep Violet (#240643):** Secondary text, seen 25 times. Token `on-surface-variant`.
- **Dark Blue (#333D47):** Muted text and metadata, seen 3 times. Token `on-surface-muted`.
- **Violet (#A998BF):** Subtle text and placeholders, seen 25 times. Token `on-surface-subtle`.
- **Snow (#F9F9FB):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Cool Mist (#EEF1F6):** Cards and panels, seen 1 time. Token `surface-container`.
- **White 60% (#FFFFFF99):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Silver (#DDDDDD):** Borders and dividers, seen 9 times. Token `outline`.
- **Violet 50% (#79589F80):** Secondary dividers, seen 7 times. Token `outline-variant`.
- **Blue (#0176D3):** Primary buttons and calls to action, seen 62 times. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Deep Violet (#300B60):** Accent in logos and imagery, seen 35 times. Token `secondary`.
- **Violet (#5A1BA9):** Accent in logos and imagery, seen 8 times. Token `tertiary`.

## Typography

**Avant Garde**, **Salesforce Sans** and **BentonSans** share the interface. Fallback stack: `Avant Garde, Arial, Helvetica, sans-serif`.

- **headline-display:** Avant Garde 40px at weight 600, line height 1.2 (30px on mobile). Page title (h1).
- **headline-lg:** Avant Garde 32px at weight 600, line height 1.25. Section headings (h2).
- **headline-md:** Salesforce Sans 25px at weight 400, line height 1. Sub-section headings.
- **headline-sm:** Avant Garde 24px at weight 600, line height 1.33. Card and feature titles.
- **title-lg:** Salesforce Sans 20px at weight 700, line height 1.4. Small titles.
- **body-md:** Salesforce Sans 16px at weight 400, line height 1.6. Body text.
- **body-lg:** Salesforce Sans 18px at weight 700, line height 1.28. Lead paragraphs.
- **body-sm:** BentonSans 15px at weight 400, line height 1.33. Secondary and small text.
- **caption:** BentonSans 14px at weight 400, line height 1.6. Captions and fine print.
- **label-lg:** Salesforce Sans 16px at weight 700, line height 1.5, tracking -0.002em. Large buttons and tabs.
- **label-md:** Salesforce Sans 15px at weight 700, line height 1. Buttons, navigation and labels.
- **label-sm:** Salesforce Sans 12px at weight 700, line height 1.5, tracking 0.05em, uppercase. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 17% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 2px, sm 5px, md 10px, lg 30px, xl 35px.
- **Gaps:** 30px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 480px, 600px, 767px, 768px, 800px, 900px, 960px, 1024px, 1025px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F9F9FB → #EEF1F6) and #DDDDDD borders.

## Shapes

Most elements use 4px corners. Measured radii, most used first:

- **md (4px):** 120 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Get Started Now”):** #0176D3 fill, #FFFFFF text, 16px/700, 4px radius, padding 12px 32px, border 2px solid #0176D3.
- **button-primary-hover:** background #0B5CAB, text #FFFFFF on hover.
- **button-ghost (“Search Open Search Popup”):** transparent fill, #FFFFFF text, 14px/400, 3px radius, padding 11px 16px.
- **link:** transparent fill, #240643 text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F9F9FB, #EEF1F6.
- Do keep text in 4 levels: #181818, #240643, #333D47, #A998BF.
- Do reserve #0176D3 for primary actions and key highlights.
- Do reuse the measured spacing steps (5px, 10px, 30px).
- Do use 4px corners on most elements.
- Don't use #A998BF for body text; it reaches 2.65:1 on #FFFFFF. Keep it for large text or metadata.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond Avant Garde, Salesforce Sans and BentonSans.
- Don't use #0176D3 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.3s, 0.4s, 0.1s.

- **Easing:** `ease`, `ease-in-out`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/heroku.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
