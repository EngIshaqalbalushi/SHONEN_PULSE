---
name: Shonen Hyperdrive
colors:
  surface: '#131316'
  surface-dim: '#131316'
  surface-bright: '#39393c'
  surface-container-lowest: '#0e0e11'
  surface-container-low: '#1b1b1e'
  surface-container: '#1f1f22'
  surface-container-high: '#2a2a2d'
  surface-container-highest: '#353438'
  on-surface: '#e4e1e6'
  on-surface-variant: '#e7bdb3'
  inverse-surface: '#e4e1e6'
  inverse-on-surface: '#303033'
  outline: '#ae887f'
  outline-variant: '#5d3f38'
  surface-tint: '#ffb4a2'
  primary: '#ffb4a2'
  on-primary: '#611200'
  primary-container: '#ff562b'
  on-primary-container: '#550e00'
  inverse-primary: '#b42900'
  secondary: '#d3fbff'
  on-secondary: '#00363a'
  secondary-container: '#00eefc'
  on-secondary-container: '#00686f'
  tertiary: '#e5b4ff'
  on-tertiary: '#4f0077'
  tertiary-container: '#c464ff'
  on-tertiary-container: '#450069'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdad2'
  primary-fixed-dim: '#ffb4a2'
  on-primary-fixed: '#3c0700'
  on-primary-fixed-variant: '#891d00'
  secondary-fixed: '#7df4ff'
  secondary-fixed-dim: '#00dbe9'
  on-secondary-fixed: '#002022'
  on-secondary-fixed-variant: '#004f54'
  tertiary-fixed: '#f5d9ff'
  tertiary-fixed-dim: '#e5b4ff'
  on-tertiary-fixed: '#30004b'
  on-tertiary-fixed-variant: '#7000a7'
  background: '#131316'
  on-background: '#e4e1e6'
  surface-variant: '#353438'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Be Vietnam Pro
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Be Vietnam Pro
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-bold:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '700'
    lineHeight: '1.0'
spacing:
  unit: 4px
  gutter: 24px
  margin: 32px
  container-max: 1440px
  offset-depth: 6px
---

## Brand & Style

This design system captures the kinetic energy and high-stakes drama of modern action anime. The brand personality is explosive, youthful, and uncompromisingly bold, targeting a Gen-Z and Alpha audience that thrives on visual stimulation and rapid information processing.

The design style is a fusion of **Neo-Brutalism** and **Vaporwave**, characterized by thick "ink" borders, saturated accent colors, and aggressive typography. To accommodate background video, the system utilizes high-opacity surfaces with glassmorphism-inspired edges, ensuring content "pops" against moving imagery. Movement is baked into the DNA through the use of skewed containers, speed-line patterns, and offset shadows that suggest a constant forward velocity.

## Colors

The palette is built on extreme contrast to maintain legibility over dynamic video backgrounds. 

- **Primary (Signal Orange):** Used for critical actions, calls to action, and "active" states. It represents heat and energy.
- **Secondary (Electric Cyan):** Used for highlights, data visualization, and interactive borders. It provides a digital, "cyber" feel.
- **Tertiary (Impact Purple):** Used for rare items, special states, or accents that require a sense of mystery or power.
- **Neutral (Deep Slate):** A near-black base used for heavy overlays and container backgrounds to anchor the vibrant accents.

All colors must meet a minimum 4.5:1 contrast ratio against the neutral background. When used over video, containers should use a 90% opacity fill of the Neutral color to prevent visual noise bleed.

## Typography

The typography strategy pairs the technical, geometric aggression of **Space Grotesk** for headings with the contemporary warmth of **Be Vietnam Pro** for body text. 

Headlines should be treated as graphic elements. Use "Display" sizes for impact, often utilizing italicization or 3-degree skews to imply motion. For high-energy sections, use uppercase transformations and tight letter spacing. Body text remains clean and highly legible, optimized for reading long-form content over dark, slightly transparent surfaces.

## Layout & Spacing

This design system employs a **12-column Fluid Grid** with generous gutters to allow the background video to "breathe" through the gaps. 

A signature "Offset Rhythm" is used: interactive elements are often physically offset from their decorative "shadow" containers by the `offset-depth` unit. Alignment should favor a strong vertical axis, but individual cards or modules can be slightly rotated (1-2 degrees) to break the "corporate" grid and add a sense of hand-drawn manga energy.

## Elevation & Depth

Depth is conveyed through **Bold Borders** and **Hard Shadows** rather than soft blurs. 

1.  **Level 0 (Base):** The video background.
2.  **Level 1 (Surface):** Neutral color at 85-90% opacity with a 1px solid border in a dimmed version of the Primary or Secondary color.
3.  **Level 2 (Active):** Solid fills with a thick (3px+) hard-drop shadow in the Primary color.
4.  **Level 3 (Overlay/Modal):** Full opacity Neutral backgrounds with a high-glow "inner stroke" (Electric Cyan) to simulate a holographic screen effect.

Avoid ambient shadows; if a shadow is needed, it must be a solid-color block offset to the bottom-right.

## Shapes

The shape language is strictly **Sharp**. 0px border radii are used to maintain a technical, aggressive, and "cut" aesthetic reminiscent of cel-shaded animation. 

To add visual interest, use "clipped corners" (diagonal cuts) on large containers or buttons to mimic mecha UI. Structural elements should feel architectural and rigid, providing a stable frame for the fluid motion of the background video.

## Components

- **Buttons:** Large, blocky, and rectangular. Primary buttons use a solid Signal Orange fill with black text and a 4px hard shadow. On hover, the button should "compress" (shift 4px down and right) to meet its shadow.
- **Chips/Badges:** Use a "Warning Tape" motif—black and yellow/orange stripes or solid Primary color with `label-bold` typography.
- **Input Fields:** Thick bottom-borders only (2px), using Electric Cyan for focus states. Include a "scanning" animation line that intermittently pulses across the field.
- **Cards:** Semi-transparent Neutral backgrounds with a "cut" top-right corner. Borders should be 1px wide, but increase to 4px on the bottom and right sides to create a faux-3D effect.
- **Progress Bars:** Use segmented blocks rather than a continuous line to evoke a "charging up" or "battery" UI feel.
- **Information Overlays:** Use "Speed Lines" (thin diagonal strokes) as subtle background patterns within cards to draw the eye toward the center.