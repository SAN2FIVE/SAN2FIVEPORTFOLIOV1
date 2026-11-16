# Santosh Bhikale – Software Developer Portfolio

A high-performance, single-page personal portfolio website for **Santosh Bhikale**, Software Developer based in Mumbai with 5+ years of experience in enterprise web applications, REST APIs, and database engineering.

**Live Site:** [https://san2five.github.io](https://san2five.github.io)  
**Repository:** [SAN2FIVE/SAN2FIVE.github.io](https://github.com/SAN2FIVE/SAN2FIVE.github.io)

---

## Overview

- **Owner:** Santosh Bhikale, Software Developer (Mumbai, India)
- **Specializations:** C#, ASP.NET Core, Web API, ASP.NET MVC, Angular, Entity Framework, SQL Server, JWT, OAuth 2.0
- **Tagline:** Open to senior .NET and full-stack roles
- **Contact:** [santoshbhikale@gmail.com](mailto:santoshbhikale@gmail.com) · [+91 70387 36407](tel:+917038736407)
- **Profiles:** [GitHub](https://github.com/SAN2FIVE) · [LinkedIn](https://www.linkedin.com/in/santosh-vishnu-bhikale/)

---

## Design System & Architecture

The site is built with a bespoke editorial aesthetic that combines brutalist precision with refined micro-interactions and liquid-glass elements.

### Color Palette (CSS Custom Properties)
- **Black:** `#000000` (`--color-black` / `--black`)
- **Electric Lime:** `#C6FF34` (`--color-lime` / `--lime`)
- **Off-white Text:** `#EEF3DC` (`--color-offwhite` / `--ink`)
- **Muted Olive:** `#B3BF8C` (`--color-muted-olive` / `--mute`)
- **Dim Olive:** `#4B5532` (`--color-dim-olive` / `--dim`)
- **Section Inversions:** Experience and Contact sections feature inverted color styling with a vibrant lime background (`#C6FF34`) and deep black typography (`#000000`).

### Typography (Google Fonts)
- **Headings & Monumental Text:** [Bricolage Grotesque](https://fonts.google.com/specimen/Bricolage+Grotesque) (weights 600, 700, 800)
- **Body & Paragraphs:** [Inter](https://fonts.google.com/specimen/Inter) (weights 400, 500, 600, 700)
- **Dates, Labels, Typing Line & Code Details:** [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (weights 400, 500, 700)

### Key Interactive Features
1. **Floating Liquid-Glass Pill Header:**
   - Centered floating glass navigation pill with `backdrop-filter` blur, specular cursor-tracking highlight, and bright inner rim.
   - Dynamic tone switching: changes to light glass with black text when scrolling over lime sections (`.exp` and `.contact`).
   - Active section spy powered by `IntersectionObserver`.
   - Mobile responsive burger button with a frosted glass navigation drawer card (closes on link click, outside tap, or `Esc`).
2. **Hero Section:**
   - Giant two-line name ("Santosh Bhikale") with a randomized character scramble on initial load that resolves letter-by-letter.
   - Magnetic cursor tracking on desktop where letters near the pointer lift and scale.
   - Animated typing line cycling through 5 role titles (*C# developer*, *.NET engineer*, *Angular builder*, *API designer*, *SQL Server specialist*).
   - Pulsing live availability indicator with quick contact action links.
3. **Skills Marquee Bands:**
   - Horizontal text strip linked to scroll speed via `requestAnimationFrame`.
   - Triple opposite-direction text tracks with alternating outlined and solid typography in the dedicated Skills section.
4. **Scroll-Driven Word Illumination:**
   - Statement paragraph in About lights up word-by-word from dim olive to electric lime based on viewport scroll progress.
   - Animated statistic counters (5+ years, 4 companies, 6 projects) running cubic ease-out transitions on view.
   - Giant faint outlined "DEVELOPER" and ".NET" background words drifting horizontally on scroll.
5. **Masked Headings & Outline Filling:**
   - Section titles rise smoothly out of overflow masks when entering the viewport.
   - Outline titles for "Experience" and "Projects" fill horizontally with color as you scroll past them.
6. **Experience Highlighter Sweeps:**
   - Monospace dates and metadata for each role.
   - Key technology terms in bullet points feature a highlighter sweep effect on hover and keyboard focus.
7. **Interactive Project Rows:**
   - Featured projects: **KolabX**, **Fine Food e-commerce**, **TMS**, **DMS**, **SARATHI**, **SMERA Lines**.
   - Hovering inverts the project row to lime while the project title scrambles and resolves.
8. **Accessibility & Motion Preferences:**
   - Full static fallback support under `prefers-reduced-motion: reduce`.
   - High-contrast `:focus-visible` outlines for keyboard navigability.
   - Accessible heading hierarchy, ARIA labels, and screen reader announcements.

---

## Technical Specifications

- **Zero Build Step:** 100% plain HTML5, CSS3, and vanilla ES6 JavaScript in a single, self-contained `index.html`.
- **Zero External JS/CSS Dependencies:** No frameworks (React, Vue, Tailwind, Bootstrap, jQuery, etc.). The only external network resource is Google Fonts.
- **Ultra-lightweight:** 60fps smooth scrolling with passive event listeners and `requestAnimationFrame`.
- **Mobile Responsive:** Fluid layout with `clamp()` typography and CSS Grid/Flexbox tested from 360px up to 1920px viewports.

---

## Running Locally

Since the portfolio has no build step and requires no package installations, you can run it immediately with any browser or local web server.

### Option 1: Direct File Open
Double-click `index.html` or open it directly from your terminal:

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Windows
start index.html
```

### Option 2: Python Static HTTP Server (Recommended)
From the repository root directory:

```bash
python3 -m http.server 8000
```
Open [http://localhost:8000](http://localhost:8000) in your browser.

### Option 3: Node.js `npx serve`
```bash
npx serve .
```

---

## Deploying to GitHub Pages

The repository `SAN2FIVE.github.io` is pre-configured to host GitHub Pages from the `main` branch.

### 1. Push Changes to GitHub
```bash
git add index.html README.md
git commit -m "feat: complete modern portfolio redesign"
git push origin main
```

### 2. Verify GitHub Pages Settings
1. On GitHub, navigate to your repository: [https://github.com/SAN2FIVE/SAN2FIVE.github.io](https://github.com/SAN2FIVE/SAN2FIVE.github.io).
2. Go to **Settings** > **Pages** (in the left sidebar).
3. Under **Build and deployment**:
   - **Source:** Deploy from a branch
   - **Branch:** `main` / `/ (root)`
   - Click **Save** (if not already enabled).
4. GitHub Pages will build and deploy automatically via the GitHub Actions static workflow (`.github/workflows/static.yml`).
5. Your portfolio will be live at:
   **[https://san2five.github.io/](https://san2five.github.io/)**

---

## File Structure

```text
SAN2FIVE.github.io/
├── .github/
│   └── workflows/
│       └── static.yml      # GitHub Actions Pages deployment workflow
├── index.html              # Complete self-contained portfolio (HTML, CSS, JS)
└── README.md               # Documentation, design system, and deployment guide
```

---

## License

© 2026 Santosh Bhikale. All rights reserved.
