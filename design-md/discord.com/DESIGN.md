---
version: alpha
name: Discord
description: "Dark interface measured from discord.com: Abcgintodiscordnord type with Abcgintodiscord, indigo accents, flat surfaces and 12px corners."
colors:
  background: "#1A2081"
  surface: "#1A2081"
  on-surface: "#FFFFFF"
  on-background: "#FFFFFF"
  on-surface-variant: "#BBBDD9"
  overlay: "#FFFFFF1A"
  primary: "#5865F2"
  on-primary: "#FFFFFF"
  secondary: "#161986"
typography:
  headline-display:
    fontFamily: Abcgintodiscordnord
    fontSize: 56px
    fontWeight: 700
    lineHeight: 0.86
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Abcgintodiscordnord
    fontSize: 36px
    fontWeight: 800
    lineHeight: 0.93
    letterSpacing: -0.01em
  body-md:
    fontFamily: Abcgintodiscord
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Abcgintodiscord
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.3
  label-md:
    fontFamily: Abcgintodiscord
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.2
  headline-display-mobile:
    fontFamily: Abcgintodiscordnord
    fontSize: 27px
    fontWeight: 700
    lineHeight: 0.89
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Abcgintodiscordnord
    fontSize: 27px
    fontWeight: 800
    lineHeight: 0.9
    letterSpacing: -0.01em
rounded:
  sm: 12px
  md: 16px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 56px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 19.5px 24px
    height: 65px
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "#23272A"
    typography: "{typography.body-lg}"
    rounded: "{rounded.sm}"
    padding: 15px 24px
    height: 65px
  button-secondary-hover:
    backgroundColor: "#C7C8CE"
  button-tertiary:
    backgroundColor: "{colors.on-surface}"
    textColor: "#000000"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 10px 16px
    height: 39px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 10px 16px
  link:
    textColor: "{colors.on-surface}"
---

# Discord Design System

## Overview

Discord describes itself as: “Discord is great for playing games and chilling with friends, or even building a worldwide community. Customize your own space to talk, play, and hang out.” The interface is dark, built on **Dark Indigo (#1A2081)** with **White (#FFFFFF)** text, and **Indigo (#5865F2)** as the main accent.

Type is set in **Abcgintodiscordnord** and **Abcgintodiscord**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 12px.

Measured from [discord.com](https://discord.com/) on October 21, 2026 at 1440×900 and 390×844 from 120 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Dark Indigo (#1A2081):** Page background, seen 1 time. Token `background`.
- **White (#FFFFFF):** Primary text and headings, seen 50 times. Token `on-surface`.
- **Light Indigo (#BBBDD9):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 1 time. Token `overlay`.
- **Indigo (#5865F2):** Primary buttons and calls to action, seen 1 time. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Dark Indigo (#161986):** Brand color in logos and imagery, seen 35 times. Token `secondary`.

## Typography

**Abcgintodiscordnord** and **Abcgintodiscord** share the interface. Fallback stack: `Abcgintodiscordnord, Arial, sans-serif`. Other loaded fonts: Ggsans, ABC Ginto Normal.

- **headline-display:** Abcgintodiscordnord 56px at weight 700, line height 0.86, tracking -0.01em, uppercase (27px on mobile). Page title (h1).
- **headline-lg:** Abcgintodiscordnord 36px at weight 800, line height 0.93, tracking -0.01em, uppercase (27px on mobile). Section headings (h2).
- **body-md:** Abcgintodiscord 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Abcgintodiscord 20px at weight 400, line height 1.3. Lead paragraphs.
- **label-md:** Abcgintodiscord 16px at weight 500, line height 1.2. Buttons, navigation and labels.

## Layout

Spacing does not follow a strict grid: 70% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 56px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 479px, 767px, 768px, 991px, 1280px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from color contrast.

## Shapes

Most elements use 12px corners. Measured radii, most used first:

- **sm (12px):** 48 elements.
- **md (16px):** 32 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Open Discord in your browser”):** #5865F2 fill, #FFFFFF text, 20px/400, 12px radius, padding 19.5px 24px.
- **button-secondary (“Download for Windows”):** #FFFFFF fill, #23272A text, 20px/400, 12px radius, padding 15px 24px.
- **button-secondary-hover:** background #C7C8CE, text #23272A on hover.
- **button-tertiary (“Log In”):** #FFFFFF fill, #000000 text, 16px/500, 16px radius, padding 10px 16px.
- **button-ghost (“Discover 3 of 9”):** transparent fill, #FFFFFF text, 16px/500, 12px radius, padding 10px 16px.
- **link:** transparent fill, #FFFFFF text, padding 0px.

## Do's and Don'ts

- Do use #1A2081 for the page.
- Do keep text in 2 levels: #FFFFFF, #BBBDD9.
- Do reserve #5865F2 for primary actions and key highlights.
- Do set headlines in Abcgintodiscordnord with tight tracking (-0.01em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 12px corners on most elements; larger surfaces also use 16px.
- Don't add drop shadows for depth; use borders and contrast.
- Don't introduce new font families beyond Abcgintodiscordnord and Abcgintodiscord.
- Don't use #5865F2 for large backgrounds or body text.
- Don't make interface transitions slower than 0.4s.

## Motion

Interface transitions are quick: 0.3s, 0.4s, 0.25s, 0.2s.

- **Easing:** `ease`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/discord.com/), the free DESIGN.md generator.
