---
name: Cyber-Minimalist
colors:
  surface: '#0c1609'
  surface-dim: '#0c1609'
  surface-bright: '#323c2d'
  surface-container-lowest: '#071105'
  surface-container-low: '#141e11'
  surface-container: '#182214'
  surface-container-high: '#222d1e'
  surface-container-highest: '#2d3828'
  on-surface: '#dae6d0'
  on-surface-variant: '#baccb0'
  inverse-surface: '#dae6d0'
  inverse-on-surface: '#293324'
  outline: '#85967c'
  outline-variant: '#3c4b35'
  surface-tint: '#2ae500'
  primary: '#efffe3'
  on-primary: '#053900'
  primary-container: '#39ff14'
  on-primary-container: '#107100'
  inverse-primary: '#106e00'
  secondary: '#c8c6c5'
  on-secondary: '#313030'
  secondary-container: '#4a4949'
  on-secondary-container: '#bab8b7'
  tertiary: '#fff8f7'
  on-tertiary: '#442927'
  tertiary-container: '#ffd3ce'
  on-tertiary-container: '#7a5955'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#79ff5b'
  primary-fixed-dim: '#2ae500'
  on-primary-fixed: '#022100'
  on-primary-fixed-variant: '#095300'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1c1b1b'
  on-secondary-fixed-variant: '#474646'
  tertiary-fixed: '#ffdad6'
  tertiary-fixed-dim: '#e7bdb8'
  on-tertiary-fixed: '#2c1513'
  on-tertiary-fixed-variant: '#5d3f3c'
  background: '#0c1609'
  on-background: '#dae6d0'
  surface-variant: '#2d3828'
  background-pure: '#000000'
  surface-glass: rgba(18, 18, 18, 0.7)
  neon-glow: rgba(57, 255, 20, 0.3)
  grid-line: '#1A1A1A'
  text-muted: '#888888'
typography:
  display-xl:
    fontFamily: Poppins
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Poppins
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Poppins
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Poppins
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Poppins
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Poppins
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Poppins
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  container-max: 1200px
  gutter: 24px
  margin-mobile: 20px
  stack-sm: 8px
  stack-md: 24px
  stack-lg: 64px
---

## Brand & Style
The design system embodies a premium, high-tech "Informatics" persona. It balances the raw, structural aesthetics of a code editor with the sophisticated polish of a modern design portfolio. The target audience includes tech recruiters and potential collaborators who value precision and technical mastery.

The style is a hybrid of **Minimalism** and **Glassmorphism**, set against a deep "void" background. It utilizes high-contrast neon accents to draw attention to interactive elements and critical data points. The emotional response is one of authority, innovation, and digital craftsmanship—evoking the feeling of a high-end IDE or a futuristic terminal interface.

## Colors
The palette is strictly nocturnal, centered on deep blacks and dark grays to provide a "true dark mode" experience. 

- **Primary Accent:** Neon Green (#39FF14) is used sparingly but impactfully for interactive states, borders, and status indicators. It should never be used for large blocks of background color.
- **Foundation:** Pure Black (#000000) serves as the canvas, while Dark Gray (#121212) defines the boundaries of elevated containers.
- **Glassmorphism:** Surfaces use a semi-transparent gray to allow background grid patterns or light blurs to filter through, creating depth without losing the dark aesthetic.

## Typography
Poppins is used across all levels to ensure a clean, geometric, and modern feel. 

- **Hierarchy:** High-contrast sizing is used to separate sections. Display text is tightly tracked and bold, mimicking high-end editorial layouts.
- **Labels:** Small, uppercase labels with increased letter spacing are used for categorizing skills and sections, providing a "technical" metadata appearance.
- **Readability:** Body text is kept at a comfortable line height (1.6) to ensure long blocks of CV text are legible against the dark background.

## Layout & Spacing
The layout follows a **Fixed Grid** philosophy inspired by editorial portfolios. On desktop, content is constrained to a 1200px central column with a 12-column underlying structure.

- **Subtle Grids:** Backgrounds should feature a very faint 40px square grid pattern in `#1A1A1A` to reinforce the "informatics" and "structural" theme.
- **Negative Space:** Generous vertical spacing (`stack-lg`) is used between major CV sections (Education, Experience, Skills) to maintain a premium feel.
- **Responsive Behavior:** On mobile, margins reduce to 20px, and grid columns collapse into a single-column stack, prioritizing vertical hierarchy.

## Elevation & Depth
Depth is not conveyed via traditional shadows, but through **Glassmorphism** and **Tonal Layering**.

- **Surfaces:** Elevated cards use `backdrop-filter: blur(12px)` and a 1px border of `rgba(255, 255, 255, 0.1)`.
- **Glow Effects:** Interactive elements like buttons or active progress bars utilize a soft neon outer glow (`box-shadow: 0 0 15px rgba(57, 255, 20, 0.4)`).
- **Z-Index:** Navigation remains fixed at the top with the strongest blur effect, ensuring it clearly floats above the scrolling content.

## Shapes
The design system uses "Soft" roundedness (0.25rem / 4px) to maintain a precise, technical edge. 

- **Standard Elements:** Input fields, buttons, and skill chips use the base 4px radius.
- **Cards:** Larger glassmorphic containers use `rounded-lg` (8px) to soften the transition between sections.
- **Geometric Accents:** Small 4-pointed stars or square bullets are used for list items to reinforce the informatics/tech aesthetic.

## Components

### Glassmorphic Cards
Used for "Selected Work" and "Experience" blocks. Features a 1px top-left highlight border to simulate light hitting the edge of glass. Background is a dark tint with high blur.

### Neon Progress Bars
For technical skills. The track is a dark gray (#1A1A1A), while the fill is vibrant Neon Green (#39FF14) with a localized glow at the leading edge of the bar.

### Modern Timelines
Vertical lines for "Riwayat Pendidikan" should be 1px wide, using the `grid-line` color. Active nodes or current positions are marked with a solid neon green dot and a subtle pulsing glow.

### High-Contrast Buttons
Primary buttons are solid Neon Green with black text. Ghost buttons use a 1px neon green border and green text, shifting to a solid green state on hover.

### Skill Chips
Small, outlined containers with `label-sm` typography. These should look like "tags" in a developer documentation site.

### Input Fields
Dark backgrounds with a simple 1px bottom border. On focus, the border transitions to Neon Green with a subtle horizontal glow.