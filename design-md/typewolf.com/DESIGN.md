---
version: alpha
name: Typewolf
description: "Light interface measured from typewolf.com: DomaineDisplayNarrow type with DomaineText, light orange accents, tonal surfaces and square corners."
colors:
  background: "#E6DDDE"
  surface: "#E6DDDE"
  on-surface: "#443235"
  on-background: "#443235"
  on-surface-variant: "#654A4E"
  on-surface-muted: "#916A70"
  surface-container-low: "#FFFFFF"
  outline: "#F5F1F2"
  outline-variant: "#CFC6C7"
  primary: "#F6C48A"
  on-primary: "#000000"
typography:
  headline-display:
    fontFamily: DomaineDisplayNarrow
    fontSize: 42px
    fontWeight: 700
    lineHeight: 1.2
  headline-lg:
    fontFamily: DomaineDisplayNarrow
    fontSize: 26px
    fontWeight: 700
    lineHeight: 1.2
  body-md:
    fontFamily: DomaineText
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: DomaineText
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.45
  body-sm:
    fontFamily: DomaineText
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-lg:
    fontFamily: Dia
    fontSize: 15px
    fontWeight: 900
    lineHeight: 1.2
    letterSpacing: -0.03em
  label-md:
    fontFamily: Dia
    fontSize: 14px
    fontWeight: 900
    lineHeight: 1.3
  label-sm:
    fontFamily: Dia
    fontSize: 13px
    fontWeight: 900
    lineHeight: 1.3
    letterSpacing: -0.03em
  headline-lg-mobile:
    fontFamily: DomaineDisplayNarrow
    fontSize: 18px
    fontWeight: 700
    lineHeight: 1.3
rounded:
  none: 0px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 19px
  xl: 42px
  container: 1128px
components:
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: 10.5px
  link:
    textColor: "{colors.on-surface}"
---

# Typewolf Design System

## Overview

Typewolf describes itself as: “Typewolf helps designers choose the perfect font combination for their next design project—features web fonts in the wild, font recommendations and learning resources.” The interface is light, built on **Warm Mist (#E6DDDE)** with **Dark Red (#443235)** text, and **Light Orange (#F6C48A)** as the main accent.

Type is set in **DomaineDisplayNarrow** and **DomaineText**. Headlines run large; body text is 16px. Depth comes from hairline borders and inset highlights rather than drop shadows. Corners are square.

Measured from [typewolf.com](https://www.typewolf.com/) on November 4, 2026 at 1440×900 and 390×844 from 213 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 9 roles.

- **Warm Mist (#E6DDDE):** Page background, seen 1 time. Token `background`.
- **Dark Red (#443235):** Primary text and headings, seen 42 times. Token `on-surface`.
- **Dark Red (#654A4E):** Secondary text, seen 59 times. Token `on-surface-variant`.
- **Red (#916A70):** Muted text and metadata, seen 12 times. Token `on-surface-muted`.
- **White (#FFFFFF):** Raised areas one step from the page, seen 2 times. Token `surface-container-low`.
- **Mist (#F5F1F2):** Borders and dividers, seen 29 times. Token `outline`.
- **Warm Silver (#CFC6C7):** Secondary dividers, seen 2 times. Token `outline-variant`.
- **Light Orange (#F6C48A):** Brand color in logos and imagery. Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.

## Typography

**DomaineDisplayNarrow**, **DomaineText** and **Dia** share the interface. Fallback stack: `DomaineDisplayNarrow, Georgia, serif`.

- **headline-display:** DomaineDisplayNarrow 42px at weight 700, line height 1.2. Page title (h1).
- **headline-lg:** DomaineDisplayNarrow 26px at weight 700, line height 1.2 (18px on mobile). Section headings (h2).
- **body-md:** DomaineText 16px at weight 400, line height 1.5. Body text.
- **body-lg:** DomaineText 18px at weight 400, line height 1.45. Lead paragraphs.
- **body-sm:** DomaineText 14px at weight 400, line height 1.5. Secondary and small text.
- **label-lg:** Dia 15px at weight 900, line height 1.2, tracking -0.03em. Large buttons and tabs.
- **label-md:** Dia 14px at weight 900, line height 1.3. Buttons, navigation and labels.
- **label-sm:** Dia 13px at weight 900, line height 1.3, tracking -0.03em. Small labels and badges.

## Layout

Spacing does not follow a strict grid: 69% of measured values are multiples of 4px, so match the measured steps rather than rounding to a grid.

- **Scale:** xs 4px, sm 8px, md 16px, lg 19px, xl 42px.
- **Container:** content is capped at 1128px.

## Elevation & Depth

Depth comes mostly from hairline rings and inset highlights on tonal surfaces (#FFFFFF):

- `rgb(245, 241, 242) 0px -3px 0px 0px inset`

A few raised panels add a soft drop shadow: `rgba(145, 106, 112, 0.15) 0px 6px 24px 0px`.

## Shapes

Corners are square. Measured radii, most used first:

- **none (0px):** measured.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **input-field (“Enter your email”):** #FFFFFF fill, #443235 text, 16px/400, padding 10.5px, border 1px solid #CFC6C7.
- **link:** transparent fill, #443235 text, padding 0px.

## Do's and Don'ts

- Do use #E6DDDE for the page and lift surfaces in small steps: #FFFFFF.
- Do keep text in 3 levels: #443235, #654A4E, #916A70.
- Do use #F6C48A as the brand accent: header, logo and key highlights.
- Do reuse the measured spacing steps (8px, 16px, 19px).
- Don't use #916A70 for body text; it reaches 3.50:1 on #E6DDDE. Keep it for large text or metadata.
- Don't use heavy drop shadows; keep depth to hairline rings and tonal surfaces.
- Don't introduce new font families beyond DomaineDisplayNarrow, DomaineText and Dia.
- Don't use #F6C48A for large backgrounds or body text.
- Don't make interface transitions slower than 0.5s.

## Motion

Interface transitions are quick: 0.3s, 0.4s, 0.5s, 0.25s.

- **Easing:** `ease-out`, `ease`, `ease-in-out`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/typewolf.com/), the free DESIGN.md generator (engine 2026.10.29+b828a475ee10).
