---
name: Bloom
colors:
  surface: '#fcf9f4'
  surface-dim: '#dcdad5'
  surface-bright: '#fcf9f4'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3ee'
  surface-container: '#f0ede9'
  surface-container-high: '#ebe8e3'
  surface-container-highest: '#e5e2dd'
  on-surface: '#1c1c19'
  on-surface-variant: '#54433a'
  inverse-surface: '#31302d'
  inverse-on-surface: '#f3f0eb'
  outline: '#877369'
  outline-variant: '#dac2b6'
  surface-tint: '#944a18'
  primary: '#944a18'
  on-primary: '#ffffff'
  primary-container: '#ff9f66'
  on-primary-container: '#773401'
  inverse-primary: '#ffb68d'
  secondary: '#47664b'
  on-secondary: '#ffffff'
  secondary-container: '#c6e9c7'
  on-secondary-container: '#4b6a4f'
  tertiary: '#695c4b'
  on-tertiary: '#ffffff'
  tertiary-container: '#c5b4a0'
  on-tertiary-container: '#524636'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbc9'
  primary-fixed-dim: '#ffb68d'
  on-primary-fixed: '#331200'
  on-primary-fixed-variant: '#763300'
  secondary-fixed: '#c8ebca'
  secondary-fixed-dim: '#adcfaf'
  on-secondary-fixed: '#03210c'
  on-secondary-fixed-variant: '#304d35'
  tertiary-fixed: '#f2e0ca'
  tertiary-fixed-dim: '#d5c4af'
  on-tertiary-fixed: '#231a0d'
  on-tertiary-fixed-variant: '#514535'
  background: '#fcf9f4'
  on-background: '#1c1c19'
  surface-variant: '#e5e2dd'
typography:
  display:
    fontFamily: Lexend
    fontSize: 40px
    fontWeight: '600'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Lexend
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Lexend
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
  headline-md:
    fontFamily: Lexend
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
  body-lg:
    fontFamily: Quicksand
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 28px
  body-md:
    fontFamily: Quicksand
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  label-md:
    fontFamily: Quicksand
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Quicksand
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  unit: 8px
  container-padding: 24px
  stack-gap: 16px
  section-gap: 40px
  touch-target: 48px
---

## Brand & Style

The design system is centered on the concept of "Nurtured Growth." It targets individuals seeking a low-pressure, supportive environment for personal development. The personality is warm, patient, and encouraging, intentionally avoiding the high-performance, clinical aesthetic of traditional productivity tools.

The visual style is **Soft Minimal with Tactile influences**. It prioritizes heavy whitespace to reduce cognitive load, paired with "squishy" UI elements that feel approachable and physical. The emotional goal is to make habit tracking feel less like a chore and more like tending to a digital garden. High-quality typography and organic shapes replace rigid grids to create a sense of natural harmony.

## Colors

The palette is derived from nature’s transition states—dawn and spring growth. 

- **Primary (Sunset Orange):** Used for primary actions and active growth states. It provides warmth and energy without being aggressive.
- **Secondary (Sage Green):** Used for completed states, success indicators, and "nurturing" actions. It evokes calm and stability.
- **Tertiary (Apricot Cream):** Used for soft containers and highlight backgrounds to provide depth without using harsh grays.
- **Neutral (Warm Parchment):** The foundation of the UI. This off-white base reduces eye strain and provides a softer backdrop than pure white.

Semantic colors should be softened: use the Sage Green for success and a soft terracotta for errors, avoiding high-vibration "traffic light" reds and greens.

## Typography

This design system uses a combination of **Lexend** for structural hierarchy and **Quicksand** for reading and interaction. The choice of rounded terminal fonts ensures the UI feels soft and friendly.

- **Headlines:** Use Lexend with medium weights. Avoid heavy bolds to maintain the "Soft Minimal" aesthetic.
- **Body:** Quicksand is used for all functional text. The "Medium" (500) weight is the default to ensure legibility against warm, tinted backgrounds.
- **Micro-copy:** Use Label-sm for progress indicators and timestamps.

Maintain generous line heights to ensure the interface feels "airy" and unhurried.

## Layout & Spacing

The layout follows a **fluid-to-centered model**. On mobile, it utilizes a single-column flow with 24px side margins. On larger screens, the content is capped at a max-width of 800px to maintain an intimate, journal-like feel.

The spacing rhythm is based on an 8px base unit but favors "generous breathing room." Elements should never feel crowded; if in doubt, increase the `stack-gap`. 

**Breakpoints:**
- **Mobile:** < 600px (Full width, 24px margins)
- **Tablet/Desktop:** > 600px (800px max-width container, centered)

## Elevation & Depth

This design system eschews traditional shadows in favor of **Tonal Layers** and **Soft Ambient Occlusion**.

- **Surface Levels:** The base is the Neutral color. Content cards sit on "Level 1" using the Tertiary color or pure white.
- **Shadows:** Use extremely diffused shadows with a hint of the Primary color (e.g., `rgba(255, 159, 102, 0.08)`). The blur radius should be large (20px+) with a small Y-offset (4px) to create a "floating" look rather than a "lifted" look.
- **Interactive Depth:** When pressed, elements should use a slight inner shadow or scale down to 0.98 to simulate a physical, squishy response.

## Shapes

The shape language is defined by **Pill-shaped (Maximum) roundedness**. This removes all "sharpness" from the experience.

- **Standard Buttons & Inputs:** Use full pill-shaped corners.
- **Cards:** Use `rounded-xl` (24px - 48px) to create a soft, pebble-like appearance.
- **Selection States:** Use organic, slightly irregular "blob" shapes for background highlights to reinforce the growth theme.

## Components

### Buttons
Primary buttons use the Sunset Orange background with white text. They should have a subtle "bounce" animation on hover. Secondary buttons use a thick 2px border in the Primary color with no fill.

### Habit Chips
Small, pill-shaped indicators that represent habit categories. When "Active," they use the Primary color; when "Dormant," they use a low-opacity version of the Neutral color.

### Progress Cards
Cards must have a 24px internal padding. They should use a "Soft Glass" effect (background-blur with high-opacity Tertiary fill) to sit above the main background.

### Checkmarks & Toggle
The "Satisfying State": When a habit is checked, the icon should trigger a subtle haptic-style scale animation and transition from Neutral to Sage Green. Use a custom "Bloom" icon—a growing leaf or flower—instead of a standard tick.

### Input Fields
Inputs should have a thick 2px border in the Tertiary color that shifts to Primary on focus. The background should be a slightly darker tint of the Neutral color to look "recessed" and tactile.