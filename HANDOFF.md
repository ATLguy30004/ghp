# HANDOFF — hayaandangra.com

## Status: Built, needs polish + deploy

**10 Astro pages built and building clean (1.84s, zero errors).**

Run `npm run dev` to see the site locally.

---

## What Exists

### Pages
| Page | Path | Status |
|---|---|---|
| Home | / | Built — hero, timeline, 3 project cards |
| Elote King | /elote-king | Built — full case study (Problem → Process → Results → Learnings) |
| Math Hub | /math-explorations | Built — 4 demo cards with colored accents |
| Chaos Demo | /math-explorations/chaos | Built — bifurcation diagram + time series, r slider, animate button |
| Primes Demo | /math-explorations/primes | Built — Ulam spiral, grid size slider, highlight diagonals toggle |
| Walks Demo | /math-explorations/walks | Built — animated single walk + endpoint distribution scatter |
| Fourier Demo | /math-explorations/fourier | Built — square/triangle/sawtooth approximation, terms slider |
| Creative Labs | /creative-labs | Built — teaching story + what I do grid |
| About | /about | Built — bio, interests grid, tech stack, what's next |
| Contact | /contact | Built — Formspree form (PLACEHOLDER URL needs replacing) |

### Tech Stack
- Astro 5.x (static)
- Vanilla CSS (no Tailwind)
- Google Fonts (DM Sans + Bebas Neue)
- Canvas API for math demos
- Formspree for contact form
- Target: Vercel free hosting

### Design System (in src/styles/global.css)
- White (#FFFFFF) background
- Charcoal (#2C3E50) text
- Blue (#3498DB) accent
- Orange (#E67E22) accent (Elote King)
- DM Sans body, Bebas Neue display

---

## What Needs to Happen

### 1. Visual QA
- Open `npm run dev` in browser
- Check every page at 375px (mobile) and 1200px (desktop)
- Fix any layout breaks, text overflow, touch targets too small
- Verify Header hamburger menu works on mobile
- Verify all nav links work

### 2. Math Demo Testing
- Test ALL 4 demos in browser — sliders, buttons, canvas rendering
- Chaos: does bifurcation diagram render? Does r slider update time series?
- Primes: does Ulam spiral draw? Does grid size slider work?
- Walks: does single walk animate? Does distribution run and show scatter?
- Fourier: do all 3 wave types render? Does terms slider update approximation?
- Fix any JS bugs (Canvas issues, NaN values, animation glitches)

### 3. Missing Files
- Add favicon.svg to public/ (simple "HD" monogram or "H" lettermark)
- Add .gitignore (node_modules/, dist/, .astro/)
- Add robots.txt to public/
- Add og-image.jpg to public/ (can be a simple branded card — name + tagline)

### 4. Formspree
- Contact page has PLACEHOLDER in form action URL
- Either: create a Formspree form and replace the URL
- Or: leave it with a TODO comment for Fahim to set up

### 5. Footer Social Links
- Footer and contact page have # placeholder hrefs for X, LinkedIn, GitHub
- Replace when Hayaan's profiles are created, or leave as # with TODO

### 6. Git + Deploy
- git init in ghp/
- .gitignore first
- Initial commit
- Create GitHub repo (hayaandangra or ghp)
- Push to GitHub
- Connect to Vercel
- Set custom domain when hayaandangra.com is purchased

---

## Research Files (in ghp/research/)

| File | What it contains |
|---|---|
| strategy-validation.md | GHP risk analysis — should he build this at all? |
| product-architecture.md | Math demo specs, scope, authenticity test |
| interview-narrative.md | Word-for-word GHP interview prep with tone guide |
| brand-strategy.md | 12-month roadmap, college angle, positioning |
| personal-brand.md | Voice guide, X/LinkedIn content calendar |
| site-architecture.md | Original detailed page specs |
| portfolio-research.md | 20+ analyzed teen builder portfolio sites |
| site-design-patterns.md | Full design system research with anti-patterns |

## Full Plan
~/.claude/plans/shimmying-churning-teacup.md

---

## Owner Context
- **Fahim** (dad) is the project owner
- **Hayaan Dangra** is the high school senior whose site this is
- GHP math semifinal interview is late Feb / mid-March 2026
- hayaandangra.com domain needs to be purchased
- X and LinkedIn profiles for Hayaan need to be created
- Elote King is the family food business
- Creative Labs Learning Center is mom's business
