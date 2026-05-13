---
name: Cyber-Minimal Safety
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c2c6d8'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8c90a1'
  outline-variant: '#424655'
  surface-tint: '#b0c6ff'
  primary: '#b0c6ff'
  on-primary: '#002d6f'
  primary-container: '#568dff'
  on-primary-container: '#002661'
  inverse-primary: '#0058cb'
  secondary: '#bdf4ff'
  on-secondary: '#00363d'
  secondary-container: '#00e3fd'
  on-secondary-container: '#00616d'
  tertiary: '#ffb3b3'
  on-tertiary: '#680015'
  tertiary-container: '#ff5260'
  on-tertiary-container: '#5b0011'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d9e2ff'
  primary-fixed-dim: '#b0c6ff'
  on-primary-fixed: '#001945'
  on-primary-fixed-variant: '#00429c'
  secondary-fixed: '#9cf0ff'
  secondary-fixed-dim: '#00daf3'
  on-secondary-fixed: '#001f24'
  on-secondary-fixed-variant: '#004f58'
  tertiary-fixed: '#ffdad9'
  tertiary-fixed-dim: '#ffb3b3'
  on-tertiary-fixed: '#400009'
  on-tertiary-fixed-variant: '#920021'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Sora
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Sora
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Sora
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
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
    lineHeight: '1.2'
    letterSpacing: 0.05em
  headline-lg-mobile:
    fontFamily: Sora
    fontSize: 28px
    fontWeight: '600'
    lineHeight: '1.2'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  margin-mobile: 20px
  margin-desktop: 64px
---

## Brand & Style

The design system is anchored in a "Cyber-Minimal" philosophy—a fusion of futuristic high-tech aesthetics and utilitarian clarity. It aims to evoke a sense of absolute security and technical sophistication without falling into the cluttered visual tropes of traditional "cyber" interfaces. 

The core style is **Glassmorphism**, utilized specifically to create depth and hierarchy on deep black canvases. By using translucent layers and high-precision borders, the interface feels lightweight and non-intrusive. The emotional response is one of "calm vigilance": the platform remains unobtrusive until needed, at which point it becomes a high-contrast, authoritative guide for student safety.

## Colors

This design system uses a strictly dark palette to maximize contrast and reduce eye strain in nighttime campus environments. 

- **Primary (Neon Blue):** The heartbeat of the system. Used for critical actions, navigation, and brand presence.
- **Secondary (Cyan):** Reserved for informational states, active trackers, and low-priority successes.
- **Tertiary (Soft Red):** Exclusively for emergencies, panic triggers, and warnings. It is saturated enough to grab attention but "soft" enough to remain legible against black backgrounds.
- **Neutrals:** Three distinct tiers of black are used to create structural depth. Base (#050505) for the background, Surface (#0A0A0A) for standard containers, and Overlay (#111111) for elevated glass cards.

## Typography

The typographic system balances the geometric, technical feel of **Sora** with the highly legible, humanist qualities of **Manrope**.

- **Sora** is used for headings to reinforce the futuristic vibe. Its wide aperture ensures that even at high weights, it remains clear under varying light conditions.
- **Manrope** handles all body copy and UI labels. It provides a grounded, trustworthy feel that is essential for a safety platform.
- **Visual Rhythm:** Use generous line heights for body text to ensure readability during high-stress situations. All labels use slightly increased letter spacing and semi-bold weights for instant recognition.

## Layout & Spacing

This design system utilizes a **Mobile-First Fluid Grid** with a strict 4px baseline rhythm.

- **Mobile:** A 4-column grid with 20px side margins and 16px gutters. Elements should be primarily stacked to allow for easy one-handed thumb interaction.
- **Desktop:** Scales to a 12-column grid. Content containers should be capped at 1200px to maintain readability. 
- **Philosophy:** Negative space is used as a functional tool to separate distinct safety actions. Components never feel "cramped"; padding within glass cards is generous (minimum 24px) to ensure touch targets are accessible and the "glass" effect has enough surface area to be visible.

## Elevation & Depth

Hierarchy is established through **Backdrop Blurs** and **Luminous Borders** rather than traditional shadows.

1. **Base Layer:** The deepest black (#050505), representing the "void" or the furthest background.
2. **Glass Level 1 (Static Cards):** A subtle `20px` blur with a 3% white fill and an 8% white border. This is used for standard content modules.
3. **Glass Level 2 (Floating/Active):** Higher transparency and a subtle Primary (Neon Blue) outer glow (0px 4px 20px rgba(0, 112, 255, 0.15)). This is used for active trackers or buttons.
4. **Emergency Level:** A Soft Red glow is applied to the outermost container when an emergency state is active, creating a "pulsing" peripheral indicator that the app is in alert mode.

## Shapes

The shape language is consistently **Rounded** (0.5rem base) to counteract the coldness often associated with "cyber" aesthetics.

- **Cards & Modals:** Use `rounded-xl` (1.5rem) to create a friendly, modern container feel.
- **Buttons:** Use `rounded-lg` (1rem) for a distinct interactive shape.
- **Status Indicators:** Small chips use a pill-shape (full radius) to distinguish them from actionable buttons.
- **Borders:** All glass elements must feature a `1px` solid border to define their edges against the deep black background.

## Components

- **Glass Cards:** The primary container. Must feature `backdrop-filter: blur(20px)`, a thin subtle border, and internal padding of at least `24px`.
- **Primary Action Button:** Solid Neon Blue fill with white or deep black text. For "Cyber-Minimal" flair, add a secondary 1px border 4px outside the button on hover/active states.
- **Emergency Button:** A large, circular, Soft Red component. It should occupy a fixed position in mobile layouts for instant access.
- **Input Fields:** Darker than the surface (#050505), featuring a simple bottom border that glows Primary Blue when focused.
- **Safety Chips:** Small, pill-shaped indicators using Cyan for "Safe" or "Active" statuses.
- **Interactive Map:** A custom dark-themed map (using #050505 base) with Neon Blue paths and Soft Red incident markers.
- **Status Bar:** A persistent, semi-transparent blur at the top or bottom of the screen to provide continuous feedback of the student's safety status.