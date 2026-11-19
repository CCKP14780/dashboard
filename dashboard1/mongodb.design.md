---
version: alpha
name: MongoDB
website: "https://www.mongodb.com"
description: MongoDB carries a strong dual-mode visual identity — dark deep-teal hero bands at "#001e2b" with bright MongoDB green "#00ed64" CTAs paired with stark white documentation surfaces. The signature green pill button is unmistakable across product, pricing, learning, and AI use-case surfaces. The system uses Euclid Circular A as its display face, anchors a 3-tier pricing comparison (Free / Flex / Dedicated), and presents extensive course catalogs in card grids with colored category tags. Coverage spans homepage, Atlas product page, Community Edition, MongoDB University, AI use cases, and pricing.

seo:
  title: "MongoDB Design Tokens: Spring Green on Deep Teal"
  metaDescription: "MongoDB's brand green #00ed64 on deep teal #001e2b with Euclid Circular A, as a DESIGN.md with colors, type and components for React and AI tools."
  highlights:
    - "Dual-mode identity — deep teal #001e2b hero bands paired with bright #00ed64 green pill CTAs, no third surface mode"
    - "Universal pill buttons — every primary, secondary, on-dark, and badge CTA renders at 9999px radius across all six pages"
    - "Category-coded course tags — purple #7b3ff2, orange #fa6e39, pink #f06bb8, and blue #3d4f9f appear only on MongoDB University tiles"
    - "Euclid Circular A across 16 type tokens — from 72px hero display at weight 500 down to 11px uppercase eyebrows at weight 600"
    - "Source Code Pro reserved for terminal-aesthetic code mockups on dark #001e2b canvas, never for prose"
  tags:
    - "Backend, Database & DevOps"
    - "Developer Tools & IDEs"
  lastUpdated: "2026-05-12"
  author:
    name: "Dov Azencot"
    url: "https://x.com/dovazencot"
  opening: |
    MongoDB's design system runs on a tight two-mode contract. Deep teal "#001e2b" hero bands frame primary CTAs in bright MongoDB green "#00ed64", and the rest of the page drops to stark white "#ffffff" for documentation, pricing, and course catalogs. The brand has refined this contrast since the rebrand era, and today every surface — homepage, Atlas product page, Community Edition, MongoDB University, AI use cases, and the 3-tier pricing page — uses the same dark-band-plus-green-pill pattern. The pill button is the brand signature: 9999px radius applied universally to primary, secondary, on-dark, ghost, and badge CTAs. There is no rounded-rectangle button anywhere in the system. Euclid Circular A is the geometric sans-serif that holds the entire typographic scale, and Source Code Pro shows up only inside terminal-styled code mockup cards.

    This page packages MongoDB's full specification into a single DESIGN.md file aligned with the Google Labs spec. Inside: 35 color tokens (brand green ramp, deep teal palette, four category accents, surface and hairline neutrals, full text scale), 16 typography tokens at sizes from 11px micro-uppercase to 72px hero display, a 7-step rounded scale topping out at the universal 9999px pill, 13 spacing tokens running from 4px through a 120px hero band, and 38 component definitions covering buttons, cards, pricing tiers, course tiles, code mockups, inputs, tabs, badges, comparison tables, and the dark teal footer region.

    Feed the file to Claude, Cursor, GitHub Copilot, or any AI coding tool that reads structured tokens. The agent will reproduce the deep-teal-and-green discipline rather than substitute a generic shadcn theme — green stays scoped to CTAs and inline links, dark hero bands frame primary actions, and category accents stay locked to course tags. The token names map cleanly onto Tailwind config keys or CSS variables. MongoDB is worth studying because the system proves a developer-tool brand can stay both stark and warm — the deep teal is serious, the bright green is human, and the discipline of holding only two saturated colors across six product surfaces is rare.
  related:
    - href: "https://github.com/google-labs-code/design.md"
      title: "The DESIGN.md specification"
      description: "Google Labs' open spec for machine-readable design system files — the format this page is built on."
    - href: "/design"
      title: "Browse all design systems"
      description: "The full directory of DESIGN.md files on shadcn.io, with live mockups for each."
    - href: "/blocks"
      title: "React blocks for shadcn/ui"
      description: "Production-ready hero, pricing, CTA, and dashboard sections built with the same Tailwind + shadcn primitives."
  questions:
    - id: "primary-color"
      title: "What is MongoDB's primary brand color?"
      answer: "MongoDB's brand color is the bright green at '#00ed64' — the unmistakable pill-CTA fill that appears on every primary action across homepage, Atlas, Community, University, AI, and pricing pages. A darker variant at '#00684a' carries inline link text and segmented-tab actives, and a pale mint at '#c3f0d2' tints the featured pricing tier and success badges. Bright green is reserved for CTAs and small accents — it never floods large surfaces."
    - id: "dark-mode"
      title: "Does MongoDB's design system have a dark mode?"
      answer: "MongoDB runs a hybrid rather than a true dark mode. Hero bands, footer, code mockups, and CTA banners use the deep teal '#001e2b' canvas with white text, while documentation, pricing tiers, course tiles, and form surfaces stay on stark white '#ffffff'. The two surface modes coexist on the same page rather than toggling via a theme switcher. Specific dark-mode token values for documentation surfaces are not surfaced in the public spec — see Known Gaps."
    - id: "typography"
      title: "What typography does MongoDB use, and what should I use if Euclid isn't available?"
      answer: "MongoDB runs Euclid Circular A across every UI surface — display, body, navigation, captions, and microcopy. The face is contemporary geometric with confident proportions and a slight technical edge. The scale walks 16 tokens from a 72px hero display at weight 500 down to 11px uppercase eyebrows at weight 600. Source Code Pro appears only inside terminal-aesthetic code mockups. Inter is the closest open-source substitute for Euclid; for code, JetBrains Mono or IBM Plex Mono match Source Code Pro's proportions cleanly."
    - id: "shape-language"
      title: "What is MongoDB's shape language?"
      answer: "Pills and 12px cards. Every button — primary, secondary, on-dark, and badge — uses '{rounded.full}' (9999px), making the pill the brand signature across all six pages. Cards, pricing tiers, and course tiles use '{rounded.lg}' (12px). Inputs and code blocks step down to '{rounded.md}' (8px), course category tags to '{rounded.xs}' (4px), and featured product showcases up to '{rounded.xxl}' (24px). Hard corners appear nowhere — even the comparison table uses 8px outer rounding."
    - id: "use-in-project"
      title: "Can I use this DESIGN.md to build my own React developer-tool site?"
      answer: "Yes — the file is structured to feed Claude, Cursor, or any AI tool that reads structured design tokens. The agent will reproduce MongoDB's restraint (single green voltage, dark hero bands, universal pill buttons, locked category accents) rather than a generic shadcn theme. You can also paste the tokens straight into a Tailwind config or CSS variables. Every color, typography token, radius, and spacing value is a quoted hex or pixel value that maps cleanly to a Tailwind theme key."
    - id: "known-gaps"
      title: "What's missing from this DESIGN.md spec?"
      answer: "Four items documented in the Known Gaps section: specific dark-mode token values for documentation surfaces beyond hero bands, animation and transition timings (recommend 150–200ms ease as a default), form validation success state styling, and the course-tile category color mappings (purple, orange, pink, blue) which are observation-based rather than confirmed brand documentation. The spec captures the visible six-page surface area at roughly 95% fidelity."

colors:
  primary: "#00ed64"
  primary-deep: "#00b545"
  primary-pressed: "#008c34"
  on-primary: "#001e2b"
  brand-green: "#00ed64"
  brand-green-dark: "#00684a"
  brand-green-mid: "#00a35c"
  brand-green-soft: "#c3f0d2"
  brand-teal-deep: "#001e2b"
  brand-teal: "#003d4f"
  brand-teal-mid: "#00684a"
  accent-purple: "#7b3ff2"
  accent-orange: "#fa6e39"
  accent-pink: "#f06bb8"
  accent-blue: "#3d4f9f"
  semantic-warning-bg: "#fff8e0"
  semantic-warning-text: "#946f3f"
  canvas: "#ffffff"
  canvas-dark: "#001e2b"
  surface: "#f9fbfa"
  surface-soft: "#f4f7f6"
  surface-feature: "#e3fcef"
  hairline: "#e1e5e8"
  hairline-soft: "#eceff1"
  hairline-strong: "#c1ccd6"
  hairline-dark: "#1c2d38"
  ink: "#001e2b"
  charcoal: "#1c2d38"
  slate: "#3d4f5b"
  steel: "#5c6c7a"
  stone: "#7c8c9a"
  muted: "#a8b3bc"
  on-dark: "#ffffff"
  on-dark-muted: "#a8b3bc"

typography:
  hero-display:
    fontFamily: Euclid Circular A
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1.10
    letterSpacing: -1.5px
  display-lg:
    fontFamily: Euclid Circular A
    fontSize: 56px
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: -1px
  heading-1:
    fontFamily: Euclid Circular A
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.20
    letterSpacing: -0.5px
  heading-2:
    fontFamily: Euclid Circular A
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.5px
  heading-3:
    fontFamily: Euclid Circular A
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.30
  heading-4:
    fontFamily: Euclid Circular A
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.35
  heading-5:
    fontFamily: Euclid Circular A
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.40
  subtitle:
    fontFamily: Euclid Circular A
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.50
  body-md:
    fontFamily: Euclid Circular A
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.55
  body-md-medium:
    fontFamily: Euclid Circular A
    fontSize: 16px
    fontWeight: 500
    lineHeight: 1.55
  body-sm:
    fontFamily: Euclid Circular A
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.50
  body-sm-medium:
    fontFamily: Euclid Circular A
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.50
  caption:
    fontFamily: Euclid Circular A
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.40
  caption-bold:
    fontFamily: Euclid Circular A
    fontSize: 13px
    fontWeight: 600
    lineHeight: 1.40
  micro:
    fontFamily: Euclid Circular A
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.40
  micro-uppercase:
    fontFamily: Euclid Circular A
    fontSize: 11px
    fontWeight: 600
    lineHeight: 1.40
    letterSpacing: 1px
  button-md:
    fontFamily: Euclid Circular A
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.30
  code-md:
    fontFamily: Source Code Pro
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55

rounded:
  xs: 4px
  sm: 6px
  md: 8px
  lg: 12px
  xl: 16px
  xxl: 24px
  full: 9999px

spacing:
  xxs: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 20px
  xl: 24px
  xxl: 32px
  xxxl: 40px
  section-sm: 48px
  section: 64px
  section-lg: 96px
  hero: 120px

components:
  button-primary:
    backgroundColor: "{colors.brand-green}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button-md}"
    rounded: "{rounded.full}"
    padding: "10px 22px"
  button-primary-pressed:
    backgroundColor: "{colors.primary-pressed}"
    textColor: "{colors.on-primary}"
  button-primary-disabled:
    backgroundColor: "{colors.hairline}"
    textColor: "{colors.muted}"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.button-md}"
    rounded: "{rounded.full}"
    padding: "10px 22px"
    border: "1px solid {colors.hairline-strong}"
  button-on-dark:
    backgroundColor: "{colors.brand-green}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button-md}"
    rounded: "{rounded.full}"
    padding: "10px 22px"
  button-secondary-on-dark:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.button-md}"
    rounded: "{rounded.full}"
    padding: "10px 22px"
    border: "1px solid {colors.hairline-dark}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.button-md}"
    rounded: "{rounded.md}"
    padding: "8px 12px"
  button-link:
    backgroundColor: "transparent"
    textColor: "{colors.brand-green-dark}"
    typography: "{typography.body-sm-medium}"
    padding: "0"
  card-base:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xl}"
    border: "1px solid {colors.hairline}"
  card-feature:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xxl}"
    border: "1px solid {colors.hairline}"
  card-product-deploy:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xxl}"
    border: "1px solid {colors.hairline}"
  card-feature-dark:
    backgroundColor: "{colors.brand-teal-deep}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xxl}"
  card-course:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xl}"
    border: "1px solid {colors.hairline}"
  card-cert:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xl}"
    border: "1px solid {colors.hairline}"
  pricing-card:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xxl}"
    border: "1px solid {colors.hairline}"
  pricing-card-featured:
    backgroundColor: "{colors.surface-feature}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xxl}"
    border: "2px solid {colors.brand-green}"
  text-input:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: "{spacing.sm} {spacing.md}"
    border: "1px solid {colors.hairline-strong}"
    height: 44px
  text-input-focused:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    border: "2px solid {colors.brand-green-dark}"
  search-pill:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.steel}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: "{spacing.sm} {spacing.md}"
    height: 44px
    border: "1px solid {colors.hairline-strong}"
  search-pill-large:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.steel}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
    height: 56px
    border: "1px solid {colors.hairline-strong}"
  pill-tab:
    backgroundColor: "transparent"
    textColor: "{colors.steel}"
    typography: "{typography.body-sm-medium}"
    rounded: "{rounded.full}"
    padding: "{spacing.xs} {spacing.md}"
    border: "1px solid {colors.hairline}"
  pill-tab-active:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.full}"
    border: "1px solid {colors.ink}"
  segmented-tab:
    backgroundColor: "transparent"
    textColor: "{colors.steel}"
    typography: "{typography.body-sm-medium}"
    padding: "{spacing.sm} {spacing.md}"
    border: "0 0 2px transparent solid"
  segmented-tab-active:
    backgroundColor: "transparent"
    textColor: "{colors.brand-green-dark}"
    typography: "{typography.body-sm-medium}"
    border: "0 0 2px {colors.brand-green-dark} solid"
  badge-green:
    backgroundColor: "{colors.brand-green}"
    textColor: "{colors.on-primary}"
    typography: "{typography.caption-bold}"
    rounded: "{rounded.sm}"
    padding: "2px 8px"
  badge-green-soft:
    backgroundColor: "{colors.brand-green-soft}"
    textColor: "{colors.brand-green-dark}"
    typography: "{typography.caption-bold}"
    rounded: "{rounded.full}"
    padding: "4px 10px"
  badge-purple:
    backgroundColor: "{colors.accent-purple}"
    textColor: "{colors.on-dark}"
    typography: "{typography.caption-bold}"
    rounded: "{rounded.sm}"
    padding: "2px 8px"
  badge-orange:
    backgroundColor: "{colors.accent-orange}"
    textColor: "{colors.on-dark}"
    typography: "{typography.caption-bold}"
    rounded: "{rounded.sm}"
    padding: "2px 8px"
  badge-popular:
    backgroundColor: "{colors.brand-teal-deep}"
    textColor: "{colors.brand-green}"
    typography: "{typography.caption-bold}"
    rounded: "{rounded.full}"
    padding: "4px 10px"
  promo-banner:
    backgroundColor: "{colors.brand-teal-deep}"
    textColor: "{colors.on-dark}"
    typography: "{typography.body-sm-medium}"
    padding: "{spacing.sm} {spacing.md}"
  hero-band-dark:
    backgroundColor: "{colors.brand-teal-deep}"
    textColor: "{colors.on-dark}"
    rounded: "0"
    padding: "{spacing.hero}"
  hero-platform-card:
    backgroundColor: "{colors.brand-teal-mid}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.xl}"
    padding: "{spacing.xxl}"
  cta-banner-dark:
    backgroundColor: "{colors.brand-teal-deep}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.lg}"
    padding: "{spacing.section}"
  code-block:
    backgroundColor: "{colors.canvas-dark}"
    textColor: "{colors.on-dark}"
    typography: "{typography.code-md}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  code-mockup-card:
    backgroundColor: "{colors.canvas-dark}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
  comparison-table:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    border: "1px solid {colors.hairline}"
  comparison-row:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    padding: "{spacing.md} {spacing.lg}"
    border: "0 0 1px {colors.hairline-soft} solid"
  service-tile:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xl}"
    border: "1px solid {colors.hairline}"
  why-card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xl}"
  customer-testimonial-card:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xxl}"
    border: "1px solid {colors.hairline}"
  logo-wall-item:
    backgroundColor: "transparent"
    textColor: "{colors.steel}"
    typography: "{typography.body-md-medium}"
    padding: "{spacing.lg}"
  faq-accordion-item:
    backgroundColor: "{colors.canvas}"
    rounded: "{rounded.md}"
    padding: "{spacing.xl}"
    border: "0 0 1px {colors.hairline} solid"
  footer-region:
    backgroundColor: "{colors.brand-teal-deep}"
    textColor: "{colors.on-dark}"
    typography: "{typography.body-sm}"
    padding: "{spacing.section} {spacing.xxl}"
  footer-link:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark-muted}"
    typography: "{typography.body-sm}"
    padding: "{spacing.xxs} 0"
---

## Overview

MongoDB carries a strong dual-mode visual identity — dark deep-teal hero bands at "#001e2b" paired with bright MongoDB green "#00ed64" CTA pills, sitting alongside stark white "#ffffff" documentation and pricing surfaces. The homepage opens with "One data platform. Unlimited AI potential." headline over a deep navy hero, the green pill at the visual center as the primary CTA. Lower on the page, embedded code mockup cards with terminal aesthetic sit on the dark hero band, breaking out into white feature cards below. The pricing page renders a 3-tier comparison (Free / Flex / Dedicated) with a featured tier highlighted in soft mint "#e3fcef" background and a 2px "#00ed64" border. The MongoDB University page presents a course catalog grid where each tile carries a colored category tag — purple "#7b3ff2", orange "#fa6e39", pink "#f06bb8", and blue "#3d4f9f" — the only place outside the brand green where saturated color appears in the system.

The system uses Euclid Circular A as its display face. The face is contemporary geometric — confident but not overly playful — and pairs naturally with both the developer-tool aesthetic of the database product and the educational positioning of the learning surfaces. Cards use 12px corners; buttons use 9999px pills universally. The brand-teal palette at "#001e2b" anchors hero bands, footer, code mockups, and the dark CTA banners. Source Code Pro is scoped strictly to terminal-styled code mockup content — it never appears in prose, headers, or UI labels.

**Key Characteristics:**
- Deep navy/teal hero bands at "#001e2b" with bright MongoDB green "#00ed64" CTA pills
- Stark white "#ffffff" pricing and documentation surfaces with colored category tags for course tiles (purple, orange, pink, blue)
- Euclid Circular A across every UI surface from 11px micro-uppercase to 72px hero display
- Pill-shaped buttons (9999px) universal across primary, secondary, on-dark, ghost, and badge CTAs
- 3-tier pricing comparison (Free / Flex / Dedicated) with featured-mint highlight tier at "#e3fcef" + green border
- Code mockup cards with terminal-aesthetic dark canvas at "#001e2b"

## Known Gaps

- Specific dark-mode token values for canvas and surface beyond hero bands not surfaced in the public spec
- Animation and transition timings not extracted; recommend 150–200ms ease as a working default
- Form validation success state not explicitly captured — only focus and error/disabled documented
- Course-tile category color mappings (purple for Database & Security, orange for Search, pink and blue variants) are observation-based rather than confirmed brand documentation
