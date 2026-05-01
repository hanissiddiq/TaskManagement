---
name: Neumorphic Task System
colors:
  surface: '#f6faf9'
  surface-dim: '#d6dbda'
  surface-bright: '#f6faf9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f4f4'
  surface-container: '#eaefee'
  surface-container-high: '#e5e9e8'
  surface-container-highest: '#dfe3e3'
  on-surface: '#181c1c'
  on-surface-variant: '#3e4949'
  inverse-surface: '#2c3131'
  inverse-on-surface: '#edf2f1'
  outline: '#6e7979'
  outline-variant: '#bdc9c8'
  surface-tint: '#006a6a'
  primary: '#006a6a'
  on-primary: '#ffffff'
  primary-container: '#4fb3b3'
  on-primary-container: '#004242'
  inverse-primary: '#74d6d6'
  secondary: '#505f76'
  on-secondary: '#ffffff'
  secondary-container: '#d0e1fb'
  on-secondary-container: '#54647a'
  tertiary: '#914c27'
  on-tertiary: '#ffffff'
  tertiary-container: '#e48f65'
  on-tertiary-container: '#632906'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#91f3f2'
  primary-fixed-dim: '#74d6d6'
  on-primary-fixed: '#002020'
  on-primary-fixed-variant: '#004f50'
  secondary-fixed: '#d3e4fe'
  secondary-fixed-dim: '#b7c8e1'
  on-secondary-fixed: '#0b1c30'
  on-secondary-fixed-variant: '#38485d'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb693'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#733512'
  background: '#f6faf9'
  on-background: '#181c1c'
  surface-variant: '#dfe3e3'
typography:
  headline-xl:
    fontFamily: Manrope
    fontSize: 40px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.6'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 64px
  gutter: 24px
  margin: 32px
---

## Brand & Style

The design system is centered on tactile serenity and cognitive ease. Designed for a high-focus task management environment, it moves away from flat, digital-first aesthetics toward a physical, "clay-like" interface that feels soft to the touch. The brand personality is calm, organized, and approachable, aiming to reduce the anxiety often associated with productivity and deadlines.

The visual style is a hybrid of **Neomorphism** and **Claymorphism**. It utilizes dual-source lighting to create extruded surfaces and soft, inner-shadowed cavities. This creates a UI that feels molded rather than painted, using depth as the primary signifier of hierarchy and interactivity.

## Colors

The palette is intentionally monochromatic with a single, calming teal accent to guide the eye toward primary actions. The background is a soft, cool-toned off-white that serves as the canvas for the shadow-based depth effects.

*   **Primary:** A desaturated teal used for progress indicators, active states, and primary call-to-actions.
*   **Neutral/Background:** A specific cool gray-white that provides enough contrast for white highlights to pop while remaining soft enough for dark shadows to appear natural.
*   **Functional Shadows:** Colors are derived from the background tint. The light shadow is pure white, while the dark shadow is a deeper, semi-transparent version of the background hue to ensure the "clay" effect looks organic.

## Typography

This design system utilizes **Manrope** for its balanced, modern, and slightly rounded geometric qualities, which perfectly complement the soft edges of the UI elements. 

The typographic scale is highly structured to maintain clarity amidst the soft visual effects of the containers. Headings use heavier weights and tighter tracking to feel grounded, while body text maintains generous line heights for readability. Labels are often treated with increased letter spacing and uppercase styling to distinguish them from interactive button text.

## Layout & Spacing

The layout philosophy relies on a **Fluid Grid** with generous margins to allow the neumorphic shadows enough room to bleed without overlapping or creating visual clutter. 

A strict 8px spatial rhythm is used to define padding and margins. Because depth is the primary differentiator, elements are spaced further apart than in traditional flat design to prevent the "extrusion" effects from feeling cramped. Each card or container should have a minimum of 24px (md) spacing between its edge and the next element to ensure the shadow gradients are fully visible and contribute to the sense of height.

## Elevation & Depth

Hierarchy is established through "Surface Extrusion." All elements exist on a common plane and are either pushed out (convex) or pressed in (concave).

*   **Extruded (Convex):** Standard state for cards and buttons. Created using two shadows: a light shadow (top-left) and a dark shadow (bottom-right). The light shadow should be `#FFFFFF` at 100% opacity, and the dark shadow should be `#D1D9E6` at 70% opacity.
*   **Inset (Concave):** Used for input fields, checkboxes, and "pressed" button states. This uses internal shadows with the same light/dark directional logic, creating a "carved" look.
*   **Claymorphism Volume:** For primary buttons and progress bars, a subtle inner glow (white, 40% opacity) is applied to the top-left edge to simulate a 3D rounded volume, giving the component a "squishy" or "clay" appearance.

## Shapes

The design system uses a **Rounded** shape language to reinforce the tactile, organic feel of clay. Hard corners are strictly avoided as they break the illusion of a continuous, molded surface.

Standard cards and task containers use a 1rem (16px) corner radius. Interactive elements like buttons and chips utilize even softer radii (up to 2rem or pill-shaped) to invite interaction. The soft corners allow the light and dark shadows to wrap smoothly around the object, enhancing the 3D effect.

## Components

### Buttons
Buttons are styled as "soft-embossed" surfaces. In their default state, they are extruded from the background. Upon hover, the extrusion height increases slightly (larger shadow spread). On click, the button transitions to an "inset" state, appearing to be physically pressed into the surface.

### Task Containers (Cards)
Task containers are low-profile extruded cards. They feature a soft outer shadow to separate them from the background. Content inside the card should be flat, though progress bars within the card should be inset (carved into the card surface).

### Progress Indicators
The track of the progress indicator is inset into the container, while the active fill is a vibrant Teal "clay" bar that appears to sit inside the carved track. The fill should have a subtle inner highlight on the top edge to give it a cylindrical volume.

### Input Fields & Checkboxes
Input fields are styled as concave "wells." The text sits inside this carved area. Checkboxes follow this logic: the empty state is a small inset square; when checked, it fills with a small teal extruded "pill" or "tick" that looks like it has been dropped into the well.

### Chips & Tags
Chips are small, pill-shaped extruded elements. When selected, they change color to the primary teal but maintain their soft, molded appearance with a slightly darker teal shadow to maintain depth consistency.