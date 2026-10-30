---
version: alpha
name: Deel
description: "Light interface measured from deel.com: BagossExtendedFont type with BagossCondensedFont, deep violet accents, tonal surfaces and 200px corners."
colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#1B1B1B"
  on-background: "#1B1B1B"
  on-surface-variant: "#212121"
  on-surface-muted: "#5F5F5F"
  on-surface-subtle: "#767676"
  surface-container-low: "#F7F5F2"
  overlay: "#FFFFFF0A"
  outline: "#1B1B1B29"
  outline-variant: "#FFFFFF1A"
  primary: "#201148"
  on-primary: "#FFFFFF"
  secondary: "#B1D8FC"
  tertiary: "#A98DF6"
typography:
  display-hero:
    fontFamily: BagossExtendedFont
    fontSize: 64px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: 0.005em
  headline-display:
    fontFamily: BagossCondensedFont
    fontSize: 60px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.003em
  headline-lg:
    fontFamily: BagossCondensedFont
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.005em
  headline-md:
    fontFamily: BagossCondensedFont
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.15
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.005em
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.7
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.7
  label-lg:
    fontFamily: BagossStandardVF
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.7
    letterSpacing: 0.015em
  label-md:
    fontFamily: BagossStandardVF
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: 0.025em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.43
  headline-display-mobile:
    fontFamily: BagossCondensedFont
    fontSize: 38px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.005em
  headline-lg-mobile:
    fontFamily: BagossCondensedFont
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.05
    letterSpacing: -0.005em
  headline-md-mobile:
    fontFamily: BagossCondensedFont
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.15
rounded:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 200px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 24px
  xl: 64px
  gutter: 12px
  section: 128px
  margin: 64px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.xl}"
    padding: 12px 16px
    height: 51px
  button-outline:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 0px
    height: 32px
  button-outline-hover:
    backgroundColor: "#3F3F3F"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.xl}"
    padding: 8px 16px
    height: 40px
  button-ghost:
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.xl}"
    padding: 14px
  input-field:
    backgroundColor: "{colors.background}"
    textColor: "#000000"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 1px 54px 1px 24px
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-variant}"
    typography: "{typography.body-md}"
    rounded: 24px
    padding: 0px
  link:
    textColor: "#FAF4EE"
---

# Deel Design System

## Overview

Deel describes itself as: “Hire, pay, and manage teams in 150+ countries with Deel. Run global payroll, ensure compliance, and streamline HR operations—all on one powerful platform.” The interface is light, built on **White (#FFFFFF)** with **Charcoal (#1B1B1B)** text, and **Deep Violet (#201148)** as the main accent.

Type is set in **BagossExtendedFont** and **BagossCondensedFont**. Headlines run large with tight negative tracking; body text is 16px. The surface language is flat. Corners are mostly 200px.

Measured from [deel.com](https://www.deel.com/) on October 29, 2026 at 1440×900 and 390×844 from 337 rendered elements. Values are computed styles from the live page, not the original source files.

## Colors

The palette has 13 roles.

- **White (#FFFFFF):** Page background, seen 9 times. Token `background`.
- **Charcoal (#1B1B1B):** Primary text and headings, seen 39 times. Token `on-surface`.
- **Charcoal (#212121):** Secondary text, seen 4 times. Token `on-surface-variant`.
- **Slate (#5F5F5F):** Muted text and metadata, seen 18 times. Token `on-surface-muted`.
- **Slate (#767676):** Subtle text and placeholders, seen 3 times. Token `on-surface-subtle`.
- **Snow (#F7F5F2):** Raised areas one step from the page, seen 6 times. Token `surface-container-low`.
- **White 4% (#FFFFFF0A):** Translucent fill for cards and controls, seen 5 times. Token `overlay`.
- **Charcoal 16% (#1B1B1B29):** Borders and dividers, seen 11 times. Token `outline`.
- **White 10% (#FFFFFF1A):** Secondary dividers, seen 5 times. Token `outline-variant`.
- **Deep Violet (#201148):** Primary buttons and calls to action. Token `primary`.
- **White (#FFFFFF):** Text and icons on primary. Token `on-primary`.
- **Light Blue (#B1D8FC):** Accent (CSS variable), seen 1 time. Token `secondary`, CSS `--color-surface-brand-blue-03`.
- **Light Violet (#A98DF6):** Accent (CSS variable), seen 5 times. Token `tertiary`, CSS `--color-surface-brand-purple-03`.

## Typography

**BagossExtendedFont**, **BagossCondensedFont**, **Inter** and **BagossStandardVF** share the interface. Fallback stack: `BagossExtendedFont, BagossExtendedFont Fallback, Arial, Helvetica`.

- **display-hero:** BagossExtendedFont 64px at weight 600, line height 1, tracking 0.005em. Oversized hero statements.
- **headline-display:** BagossCondensedFont 60px at weight 500, line height 1.05, tracking -0.003em (38px on mobile). Page title (h1).
- **headline-lg:** BagossCondensedFont 44px at weight 500, line height 1.05, tracking -0.005em (28px on mobile). Section headings (h2).
- **headline-md:** BagossCondensedFont 24px at weight 500, line height 1.15 (20px on mobile). Sub-section headings.
- **headline-sm:** Inter 20px at weight 400, line height 1.6, tracking -0.01em. Card and feature titles.
- **body-md:** Inter 16px at weight 400, line height 1.5. Body text.
- **body-lg:** Inter 18px at weight 400, line height 1.6, tracking -0.005em. Lead paragraphs.
- **body-sm:** Inter 14px at weight 400, line height 1.7. Secondary and small text.
- **caption:** Inter 12px at weight 400, line height 1.7. Captions and fine print.
- **label-lg:** BagossStandardVF 16px at weight 500, line height 1.7, tracking 0.015em. Large buttons and tabs.
- **label-md:** BagossStandardVF 15px at weight 500, line height 1.6, tracking 0.025em. Buttons, navigation and labels.
- **label-sm:** Inter 14px at weight 600, line height 1.43. Small labels and badges.

## Layout

Spacing is mostly on a 4px grid (83% of measured values), with some off-grid steps. Match the measured scale rather than rounding everything.

- **Scale:** xs 4px, sm 8px, md 12px, lg 24px, xl 64px.
- **Sections:** 128px vertical padding between major sections.
- **Gaps:** 12px is the most common gap in flex and grid layouts.
- **Page margin:** 64px on each side of full-width sections.
- **Breakpoints:** 320px, 391px, 430px, 599px, 600px, 601px, 768px, 959px, 1024px, 1049px, 1279px, 1280px, 1320px, 1440px, 1620px.

## Elevation & Depth

The design is flat: no shadows were measured. Hierarchy comes from tonal surface steps (#F7F5F2) and #1B1B1B29 borders.

## Shapes

Most elements use 200px corners. Measured radii, most used first:

- **xl (200px):** 60 elements.
- **sm (8px):** 32 elements.
- **lg (16px):** 24 elements.
- **xs (4px):** 20 elements.
- **md (12px):** 20 elements.
- **full (9999px):** 12 elements.

## Components

Measured from the rendered page. Token values reference the tokens above.

- **button-primary (“Speak with a trusted expert”):** #201148 fill, #FFFFFF text, 16px/500, 200px radius, padding 12px 16px.
- **button-outline (“Claim offer”):** #FFFFFF fill, #1B1B1B text, 16px/400, 200px radius, padding 0px.
- **button-outline-hover:** background #3F3F3F, text #FFFFFF on hover.
- **button-secondary (“Book a demo”):** #1B1B1B fill, #FFFFFF text, 14px/500, 200px radius, padding 8px 16px.
- **button-ghost (“Manage”):** transparent fill, #1B1B1B text, 14px/600, 200px radius, padding 14px, border 2px solid #1B1B1B29.
- **input-field (“What's your e-mail?”):** #FFFFFF fill, #000000 text, 16px/460, 200px radius, padding 1px 54px 1px 24px, border 2px solid #1B1B1B29.
- **card:** #FFFFFF0D fill, #000000DE text, 16px/400, 24px radius, padding 0px.
- **link:** transparent fill, #FAF4EE text, padding 0px.

## Do's and Don'ts

- Do use #FFFFFF for the page and lift surfaces in small steps: #F7F5F2.
- Do keep text in 4 levels: #1B1B1B, #212121, #5F5F5F, #767676.
- Do reserve #201148 for primary actions and key highlights.
- Do set headlines in BagossExtendedFont with tight tracking (-0.003em).
- Do reuse the measured spacing steps (8px, 12px, 24px).
- Do use 200px corners on most elements; larger surfaces also use 8px, 16px and 4px.
- Don't add drop shadows for depth; use tonal surfaces.
- Don't introduce new font families beyond BagossExtendedFont, BagossCondensedFont, Inter and BagossStandardVF.
- Don't use #201148 for large backgrounds or body text.
- Don't make interface transitions slower than 0.3s.

## Motion

Interface transitions are quick: 0.1s, 0.2s, 0.15s, 0.3s.

- **Easing:** `ease-in-out`, `cubic-bezier(0.4, 0, 0.2, 1)`, `cubic-bezier(0, 0, 0.2, 1)`.
- **Reduced motion:** the page responds to `prefers-reduced-motion`.

Generated by [Sitepeel](https://sitepeel.dev/design-md/deel.com/), the free DESIGN.md tool (engine 2026.10.29+bf9d681d83cf).
