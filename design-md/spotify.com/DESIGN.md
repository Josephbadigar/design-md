---
version: alpha
name: Spotify
description: "Dark interface measured from open.spotify.com: SpotifyMixUITitle type with SpotifyMixUI, green accents, tonal surfaces and pill-shaped controls."
colors:
  background: "#121212"
  surface: "#121212"
  on-surface: "#B3B3B3"
  on-background: "#B3B3B3"
  on-surface-strong: "#FFFFFF"
  surface-container-low: "#1F1F1F"
  surface-container: "#3B3B3B"
  overlay: "#FFFFFF1A"
  primary: "#1ED760"
  on-primary: "#000000"
  secondary: "#CF4C29"
  tertiary: "#A83830"
typography:
  headline-display:
    fontFamily: SpotifyMixUITitle
    fontSize: 24px
    fontWeight: 700
  body-md:
    fontFamily: SpotifyMixUI
    fontSize: 14px
    fontWeight: 400
  body-sm:
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
  headline-display-mobile:
    fontFamily: SpotifyMixUITitle
    fontSize: 20px
    fontWeight: 700
rounded:
  sm: 4px
  md: 6px
  lg: 8px
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
    backgroundColor: "{colors.on-surface-strong}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 0px
    height: 48px
  button-primary-hover:
    backgroundColor: "#F0F0F0"
  button-secondary:
    backgroundColor: "#292929"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    padding: 8px
    height: 40px
  button-outline:
    backgroundColor: "{colors.surface-container-low}"
    textColor: "{colors.on-surface-strong}"
    typography: "{typography.label-md}"
    padding: 12px
    height: 48px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 8px 0px
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

Spotify describes itself as: “Spotify is a digital music service that gives you access to millions of songs, podcasts, and audiobooks. Listen to your favorites online now.” The interface is dark, built on **Charcoal (#121212)** with **Gray (#B3B3B3)** text, and **Green (#1ED760)** as the main accent.

Type is set in **SpotifyMixUITitle** and **SpotifyMixUI**. Headlines run large; body text is 14px. The surface language is flat. Controls are pill-shaped.

Measured from [open.spotify.com](https://open.spotify.com/) on October 29, 2026 at 1440×900 and 390×844 from 343 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 10 roles.

- **Charcoal (#121212):** Page background, seen 2 times. Token `background`, CSS `--background-base`.
- **Gray (#B3B3B3):** Primary text and headings, seen 49 times. Token `on-surface`.
- **White (#FFFFFF):** Headings and emphasis, seen 33 times. Token `on-surface-strong`, CSS `--decorative-base`.
- **Charcoal (#1F1F1F):** Raised areas one step from the page, seen 5 times. Token `surface-container-low`, CSS `--background-elevated-base`.
- **Graphite (#3B3B3B):** Cards and panels, seen 1 time. Token `surface-container`.
- **White 10% (#FFFFFF1A):** Translucent fill for cards and controls, seen 4 times. Token `overlay`.
- **Green (#1ED760):** Brand accent (CSS variable). Token `primary`.
- **Near Black (#000000):** Text and icons on primary. Token `on-primary`.
- **Red (#CF4C29):** Accent on large areas. Token `secondary`.
- **Red (#A83830):** Accent on large areas. Token `tertiary`.

## Typography

**SpotifyMixUITitle** and **SpotifyMixUI** share the interface. Fallback stack: `SpotifyMixUITitle, CircularSp-Arab, CircularSp-Hebr, CircularSp-Cyrl`.

- **headline-display:** SpotifyMixUITitle 24px at weight 700 (20px on mobile). Page title (h1).
- **body-md:** SpotifyMixUI 14px at weight 400. Body text.
- **body-sm:** SpotifyMixUI 12px at weight 400. Secondary and small text.
- **label-md:** SpotifyMixUI 16px at weight 400. Buttons, navigation and labels.
- **label-sm:** SpotifyMixUI 14px at weight 700. Small labels and badges.

## Layout

Spacing follows a 4px grid: 97% of measured gaps and paddings are multiples of 4px.

- **Scale:** xs 4px, sm 8px, md 12px, lg 20px, xl 36px.
- **Gaps:** 8px is the most common gap in flex and grid layouts.
- **Breakpoints:** 320px, 400px, 425px, 426px, 530px, 550px, 599.95px, 600px, 768px, 896px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#1F1F1F → #3B3B3B).

## Shapes

Interactive controls are pill-shaped. Measured radii, most used first:

- **full (9999px):** 108 elements.
- **md (6px):** 76 elements.
- **sm (4px):** 16 elements.
- **lg (8px):** 8 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Log in”):** #FFFFFF fill, #000000 text, 16px/700, 9999px radius, padding 0px.
- **button-primary-hover:** background #F0F0F0, text #000000 on hover.
- **button-secondary (“Instagram”):** #292929 fill, #FFFFFF text, 16px/400, 50% radius, padding 8px.
- **button-outline (“Home”):** #1F1F1F fill, #FFFFFF text, 16px/400, 50% radius, padding 12px.
- **button-ghost (“Premium”):** transparent fill, #B3B3B3 text, 16px/700, 9999px radius, padding 8px 0px.
- **input-field (“What do you want to play?”):** #1F1F1F fill, #FFFFFF text, 16px/400, 500px radius, padding 12px 96px 12px 48px.
- **link:** transparent fill, #B3B3B3 text, padding 0px.

## Do's and Don'ts

- Do use #121212 for the page and lift surfaces in small steps: #1F1F1F, #3B3B3B.
- Do keep text in 2 levels: #B3B3B3, #FFFFFF.
- Do use #1ED760 as the brand accent: header, logo and key highlights.
- Do keep spacing on the 4px grid.
- Do make buttons and chips fully rounded (9999px); most other elements use 6px corners.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond SpotifyMixUITitle and SpotifyMixUI.
- Don't use #1ED760 for large backgrounds or body text.
- Don't make interface transitions slower than 0.22s.

## Motion

Interface transitions are quick: 0.15s, 0.2s, 0.22s, 0.1s.

- **Easing:** `cubic-bezier(0.3, 0, 0, 1)`, `ease`, `ease-in`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/spotify.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
