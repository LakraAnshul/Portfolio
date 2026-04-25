---
name: Architectural Logic
colors:
  surface: '#0d1515'
  surface-dim: '#0d1515'
  surface-bright: '#323b3b'
  surface-container-lowest: '#081010'
  surface-container-low: '#151d1d'
  surface-container: '#192121'
  surface-container-high: '#232b2c'
  surface-container-highest: '#2e3637'
  on-surface: '#dce4e4'
  on-surface-variant: '#b9caca'
  inverse-surface: '#dce4e4'
  inverse-on-surface: '#2a3232'
  outline: '#849495'
  outline-variant: '#3a494a'
  surface-tint: '#00dce5'
  primary: '#e9feff'
  on-primary: '#003739'
  primary-container: '#00f5ff'
  on-primary-container: '#006c71'
  inverse-primary: '#00696e'
  secondary: '#b9cacb'
  on-secondary: '#243334'
  secondary-container: '#3d4c4d'
  on-secondary-container: '#abbbbc'
  tertiary: '#fcf9f9'
  on-tertiary: '#303030'
  tertiary-container: '#dfdddc'
  on-tertiary-container: '#626161'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#63f7ff'
  primary-fixed-dim: '#00dce5'
  on-primary-fixed: '#002021'
  on-primary-fixed-variant: '#004f53'
  secondary-fixed: '#d5e6e7'
  secondary-fixed-dim: '#b9cacb'
  on-secondary-fixed: '#0f1e1f'
  on-secondary-fixed-variant: '#3a494a'
  tertiary-fixed: '#e4e2e1'
  tertiary-fixed-dim: '#c8c6c6'
  on-tertiary-fixed: '#1b1c1c'
  on-tertiary-fixed-variant: '#474747'
  background: '#0d1515'
  on-background: '#dce4e4'
  surface-variant: '#2e3637'
typography:
  display-hero:
    fontFamily: Space Grotesk
    fontSize: 120px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: -0.04em
  h1:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '600'
    lineHeight: '1.1'
    letterSpacing: -0.03em
  h2:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: -0.03em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  code:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.05em
spacing:
  base: 4px
  xs: 8px
  sm: 16px
  gutter: 24px
  md: 32px
  margin: 40px
  lg: 64px
  xl: 128px
  max-width: 1440px
---

## Brand & Style
The brand identity is rooted in high-performance engineering and technical precision. It follows a **Cyber-Brutalist** aesthetic—characterized by a raw, unrefined structural layout, heavy use of borders instead of shadows, and monospaced typography that evokes a command-line interface (CLI) or system terminal.

The UI targets a highly technical audience (developers, AI engineers, architects) and aims to evoke a sense of "cold efficiency," logic, and uncompromising architectural integrity. It rejects soft gradients and organic shapes in favor of sharp angles, high-contrast neon accents, and a strict grid system.

## Colors
The palette is built on a "Deep Space" foundation with high-visibility functional accents. 

- **Primary (#00F5FF):** A vibrant electric cyan used for "active" states, primary actions, and high-impact semantic highlights.
- **Backgrounds:** The interface uses `#0D0D0D` as the base canvas, providing a true-black backdrop that makes the cyan accents pop.
- **Grayscale/Utility:** Various shades of zinc and slate-gray are used for structural borders and secondary text to maintain a hierarchy of information without overwhelming the user with color.
- **Interaction:** Selection states use the primary cyan as a background with inverted black text to mimic terminal highlighting.

## Typography
The typography system uses a tri-font approach to balance personality with readability:
- **Space Grotesk (Headlines):** A geometric sans-serif with eccentricities that feel futuristic and engineered. Used for massive display text and section headers.
- **Inter (Body):** Used for long-form content and descriptions where legibility is paramount.
- **JetBrains Mono (Labels/System):** Reinforces the "code" aesthetic. Used for navigation, tags, numbers, and technical metadata. All monospaced labels should be set in uppercase.

## Layout & Spacing
The layout adheres to a rigid **12-column grid system** with a fixed maximum width of 1440px. 

- **Structure:** Content is organized in horizontal bands separated by explicit borders rather than whitespace alone.
- **Grid Alignment:** Items like project lists use a 12-column split (e.g., 2-col index, 4-col title, 4-col description, 2-col metadata).
- **Rhythm:** Spacing follows a base-4 system, but prioritizes large, dramatic gaps (64px and 128px) between major sections to emphasize the Brutalist scale.

## Elevation & Depth
This system uses **Zero-Elevation Logic**. 

- **Flat Hierarchy:** No shadows or blurs are used to indicate depth.
- **Depth via Outlines:** Hierarchy is established through the use of 1px solid borders (`#3A494A`). 
- **Active State Elevation:** Instead of lifting an element, "elevation" is signaled by color inversion (e.g., a border changing from gray to cyan) or background fills.
- **Marquee Layers:** Occasional low-opacity overlays or scrolling text are used to create "visual noise" and layers of information without breaking the flat plane.

## Shapes
The shape language is strictly **rectangular and sharp**. 
- **Corners:** 0px border radius is the default for all buttons, inputs, and containers.
- **Borders:** All containers are defined by 1px solid strokes.
- **Exceptions:** No exceptions. Even "pills" or tags should maintain square corners to uphold the architectural brutalist aesthetic.

## Components

### Buttons
- **Primary:** Solid `#00F5FF` background with `#0D0D0D` text. Sharp corners.
- **Ghost/Outline:** 1px `#00F5FF` border, no background, uppercase monospaced text. Transitions to solid on hover.
- **Navigation:** Borderless, uppercase monospaced text with an underline on active/hover state.

### Cards & Rows
- **List Rows:** Instead of traditional cards, use full-width rows separated by borders. On hover, the border color shifts to the primary cyan.
- **Metadata Tags:** Small, square-cornered boxes with 1px borders containing uppercase monospaced text.

### Inputs
- **Text Fields:** 1px borders on all sides, JetBrains Mono font. Active state features a glowing cyan border.

### Decorative Elements
- **Marquee:** Scrolling text containers with `-webkit-text-stroke` styling to create "hollow" typography.
- **Morphing Text:** Use CSS animations to cycle through keywords within hero headlines, maintaining a dynamic but technical feel.