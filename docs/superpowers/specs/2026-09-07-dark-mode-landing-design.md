# Design Spec: Ignova Global Modern Dark Mode Landing Page

## 1. Overview
A modern, ultra-sleek, dark mode landing page for **Ignova Global** designed to host and serve `app-ads.txt` for AdMob / Ad networks verification while presenting a premium brand image.

## 2. Visual Aesthetic & Theme
- **Color Palette**:
  - Background: Deep Dark Canvas (`#0a0b14` / `#0f1123`)
  - Accent / Glow: Neon Indigo (`#6366f1`) to Vivid Violet (`#a855f7`) and Cyan highlight (`#06b6d4`)
  - Glass Card: `rgba(255, 255, 255, 0.04)` with `backdrop-filter: blur(24px)` and `border: 1px solid rgba(255, 255, 255, 0.08)`
  - Text: Primary `#ffffff`, Secondary `#94a3b8`, Highlight `#c084fc`
- **Dynamic Effects**:
  - Animated ambient gradient mesh in background (smooth, GPU-accelerated CSS animations)
  - Multi-layer glassmorphism with subtle gradient border
  - Tactile interactive CTA button with luminous glow and smooth micro-interactions

## 3. Page Structure & Components (`index.html`)
1. **Background Canvas**:
   - Multiple ambient floating gradient orbs (pure CSS).
   - Subtle grid/dot overlay for depth.
2. **Central Glass Card**:
   - **Logo / Brand Icon**: Custom modern geometric SVG icon with linear gradient fill and subtle drop-shadow pulse.
   - **Greeting / Title**: `<h1>Welcome!</h1>` with clean modern typography (Plus Jakarta Sans / Inter).
   - **Description**: "This is the official website for **Ignova Global**.<br>We create useful apps and fun games."
   - **Primary Action Button**: `<a href="/app-ads.txt" class="btn-ads">View app-ads.txt</a>`
   - **Security / Verified Badge / Micro-footer**: Minimal clean footer note `© 2026 Ignova Global. All rights reserved.`

## 4. File Architecture
```
f:\Ads Txt\
├── index.html        # Main semantic HTML5 landing page
├── style.css         # Modern Vanilla CSS design system with CSS variables & animations
├── app-ads.txt       # Standard IAB compliant app-ads.txt file with AdMob template
└── docs\
    └── superpowers\
        └── specs\
            └── 2026-09-07-dark-mode-landing-design.md
```

## 5. Key Features & Quality Standards
- **Pure Vanilla HTML/CSS**: Zero external heavy JS frameworks, ultra-fast TTFB and 100/100 Lighthouse performance.
- **IAB Compliance**: `app-ads.txt` placed at root URL `/app-ads.txt` with UTF-8 encoding and standard format for Google AdMob crawlers.
- **Responsive & Accessible**: Seamlessly adapts to all screen sizes (mobile phones, tablets, large monitors) with `prefers-reduced-motion` support.
- **Easy Maintenance**: All colors, brand names, and URLs parameterized via CSS variables and clean HTML tags.

## 6. Verification
- Open in browser to inspect UI layout, animations, hover effects, and responsive breakpoints.
- Verify clicking "View app-ads.txt" routes correctly to `/app-ads.txt`.
- Validate standard `app-ads.txt` formatting.
