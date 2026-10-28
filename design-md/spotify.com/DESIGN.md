---
version: alpha
name: Spotify
description: "Dark monochrome interface measured from spotify.com: SpotifyMixUITitle type with SpotifyMixUI, tonal surfaces and pill-shaped controls."
colors:
  background: "#121212"
  surface: "#121212"
  on-surface: "#B3B3B3"
  on-background: "#B3B3B3"
  on-surface-strong: "#FFFFFF"
  surface-container-low: "#1F1F1F"
  surface-container: "#3B3B3B"
  primary: "#292929"
  on-primary: "#FFFFFF"
typography:
  display-hero:
    fontFamily: SpotifyMixUITitle
    fontSize: 24px
    fontWeight: 700
  headline-display:
    fontFamily: SpotifyMixUI
    fontSize: 16px
    fontWeight: 700
  body-md:
    fontFamily: SpotifyMixUI
    fontSize: 14px
    fontWeight: 400
  body-sm:
    fontFamily: SpotifyMixUI
    fontSize: 13.33px
    fontWeight: 400
  caption:
    fontFamily: SpotifyMixUI
    fontSize: 12px
    fontWeight: 400
  label-md:
    fontFamily: SpotifyMixUI
    fontSize: 16px
    fontWeight: 400
  label-sm:
    fontFamily: SpotifyMixUI
    fontSize: 14px
    fontWeight: 700
  display-hero-mobile:
    fontFamily: SpotifyMixUITitle
    fontSize: 20px
    fontWeight: 700
rounded:
  sm: 6px
  md: 8px
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 20px
  xl: 36px
  gutter: 8px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    padding: 8px
    height: 40px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    padding: 12px
    height: 48px
  button-outline-hover:
    backgroundColor: "#2A2A2A"
  button-ghost:
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 4px 16px 4px 36px
    height: 32px
  input-field:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 96px 12px 48px
  link:
    textColor: "{colors.on-surface}"
---

# Spotify Design System

## Overview

Spotify describes itself as: “Spotify is a digital music service that gives you access to millions of songs, podcasts, and audiobooks. Listen to your favorites online now.” The interface is dark, built on **Charcoal (#121212)** with **Gray (#B3B3B3)** text and almost no color: actions are carried by contrast, not hue.

Type is set in **SpotifyMixUITitle** and **SpotifyMixUI**. Headlines run large; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [spotify.com](https://open.spotify.com/) on October 21, 2026 at 1440×900 and 812×1758 from 343 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 7 roles.

- **Charcoal (#121212):** Page background, seen 2 times. Token `background`, CSS `--background-base`.
- **Gray (#B3B3B3):** Primary text and headings, seen 66 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 30 times. Token `on-surface-strong`, CSS `--decorative-base`.
- **Charcoal (#1F1F1F):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`, CSS `--background-elevated-base`.
- **Graphite (#3B3B3B):** Cards and panels, seen 1 time. Token `surface-container`.
- **Graphite (#292929):** Primary buttons and calls to action. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.

## Typography

**SpotifyMixUITitle** and **SpotifyMixUI** share the interface. Fallback stack: `SpotifyMixUITitle, CircularSp-Arab, CircularSp-Hebr, CircularSp-Cyrl`.

- **display-hero:** SpotifyMixUITitle 24px at weight 700 (20px on mobile). Oversized hero statements.
- **headline-display:** SpotifyMixUI 16px at weight 700. Page title (h1).
- **body-md:** SpotifyMixUI 14px at weight 400. Body text.
- **body-sm:** SpotifyMixUI 13.33px at weight 400. Secondary and small text.
- **caption:** SpotifyMixUI 12px at weight 400. Captions and fine print.
- **label-md:** SpotifyMixUI 16px at weight 400. Buttons, navigation and labels.
- **label-sm:** SpotifyMixUI 14px at weight 700. Small labels and badges.

## Layout

Spacing follows a 4px grid: 100% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 36px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 400px, 425px, 426px, 500px, 530px, 550px, 599.95px, 600px, 768px, 769px, 890px, 896px, 897px, 1023px, 1024px, 1280px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#1F1F1F → #3B3B3B).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 104 elements.
- **sm (6px):** 76 elements.
- **md (8px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Instagram”):** #292929 fill, #FFFFFF text, 16px/400, 50% radius, padding 8px.
- **button-outline (“Home”):** #1F1F1F fill, #FFFFFF text, 16px/400, 50% radius, padding 12px.
- **button-outline-hover:** background #2A2A2A, text #FFFFFF on hover.
- **button-ghost (“English”):** transparent fill, #FFFFFF text, 14px/700, 9999px radius, padding 4px 16px 4px 36px, border 1px solid #7C7C7C.
- **input-field (“What do you want to play?”):** #1F1F1F fill, #FFFFFF text, 16px/400, 500px radius, padding 12px 96px 12px 48px.
- **link:** transparent fill, #B3B3B3 text, padding 0px.

## Do's and Don'ts

- Do use #121212 for the page and lift surfaces in small steps: #1F1F1F, #3B3B3B.
- Do keep text in 2 levels: #B3B3B3, #FFFFFF.
- Do let contrast carry emphasis; primary actions use #292929 on #121212.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px).
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond SpotifyMixUITitle and SpotifyMixUI.
- Don't add saturated accent colors; the measured palette is almost entirely neutral.
- Don't make interface transitions slower than 0.22s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.22s.

- **Easing:** `cubic-bezier(0.3, 0, 0, 1)`, `ease-in`, `ease-out`.
