# hayaandangra.com — Site Architecture
**Target audience:** College admissions, GHP judges, internship recruiters, peers
**Tech stack:** Astro (static), Vanilla CSS, Google Fonts (DM Sans + Bebas Neue), Vercel, GitHub
**Core principle:** Living portfolio that grows with Hayaan's projects

---

## STRATEGIC POSITIONING

### Who Lands Here and What They See

**College Admissions Officer (30 seconds)**
- Hero: High school senior who builds real things
- First scroll: Elote King case study (business impact, real revenue)
- Second scroll: GHP math explorations (intellectual curiosity)
- Third scroll: Creative Labs (community/teaching)
- CTA: Contact for portfolio review or questions

**GHP Interview Judge (2 minutes, on phone)**
- Clean, fast load on mobile
- Math explorations section: pull up, demo on phone during interview
- Shows: independent learning, technical execution, genuine curiosity
- No resume bloat, just "here's what I made"

**Internship Recruiter (tech/startup focus) (5 minutes)**
- Sees: web development skills, SEO/marketing understanding, business thinking
- Elote King = product/marketing skills
- Math visualizations = technical depth
- Cyber Security pathway = future specialization signal
- Contact form for opportunities

**Peer/Classmate (browsing)**
- "This guy actually does stuff"
- Clear project showcase
- Social proof (real results, not fake testimonials)
- Inspiration for their own work

### Core Message Hierarchy
1. **I build things that work** (Elote King, real business impact)
2. **I explore ideas I'm curious about** (GHP math, independent learning)
3. **I teach and help others** (Creative Labs, tutoring, mentoring)
4. **I'm growing into tech + healthcare** (pathways, future projects)

---

## SITE STRUCTURE

### Pages and Routing

```
/                          Home (landing + project showcase)
/elote-king                Full case study
/math-explorations         GHP math visualizations (embedded)
/creative-labs             Teaching/mentoring story
/about                     Full background, resume-style
/journal                   Optional: build-in-public posts
/contact                   Contact form + social links
```

### Why This Structure?
- **Single-page home** with project previews = fast first impression
- **Deep-dive pages** for each major project = space to tell the full story
- **Math explorations on its own page** = can pull up on phone during GHP interview
- **/about separate** = keeps home page focused on work, not biography
- **/journal optional** = can add later without redesigning

---

## PAGE-BY-LEVEL ARCHITECTURE

### Home Page (/)

**Purpose:** First impression + project showcase

**Sections:**
1. **Hero**
   - Name: "Hayaan Dangra"
   - Tagline: "High school senior. I build websites, explore math, and teach kids to code."
   - CTA: "See my work" (scrolls to projects) + "Contact me" (goes to contact page)
   - Visual: Clean headshot or abstract visual (NOT stock photo)
   - Mobile: Sticky CTA bar appears on scroll

2. **Featured Projects** (3 cards)
   - **Elote King** (primary feature)
     - Preview: "Built website, did SEO, business grew to food trailer. 2 sold-out events."
     - Visual: Screenshot of elotekingcatering.com or event photo
     - CTA: "Read case study" → /elote-king
   - **GHP Math Explorations**
     - Preview: "Interactive math visualizations. Chaos theory, prime spirals, random walks, Fourier series."
     - Visual: Screenshot of one visualization (logistic map bifurcation diagram)
     - CTA: "Explore the math" → /math-explorations
   - **Creative Labs Learning Center**
     - Preview: "Teaching kids to code and think critically. Tutoring, summer camps, mentoring."
     - Visual: Photo from class/camp OR icon-based illustration
     - CTA: "Learn more" → /creative-labs

3. **Pathways + Future Projects**
   - Brief: "I'm in the Cyber Security and Healthcare pathways at Alliance Academy. Future projects will go here."
   - Visual: Simple icon grid (cyber icon, healthcare icon, question mark for future)
   - Purpose: Signals growth trajectory, keeps site future-proof

4. **Connect**
   - Social links: X, LinkedIn, GitHub, email
   - CTA: "Want to work together?" → /contact
   - Optional: Newsletter signup for journal posts (if journal exists)

**Conversion flow:**
- Hero CTA → Projects section
- Project cards → Deep-dive pages
- Bottom CTA → Contact page
- Social links → External profiles

**Mobile optimizations:**
- Hero text: 24px min on mobile
- Project cards: stack vertically
- Sticky CTA bar: "View projects" + "Contact" buttons
- Fast load: lazy-load images below fold

---

### Elote King Case Study (/elote-king)

**Purpose:** Full business case study. This is Hayaan's strongest story.

**Sections:**
1. **Hero**
   - Title: "Elote King: From Local Business to Food Trailer"
   - Subtitle: "How a website and SEO strategy helped a family business scale"
   - Visual: Hero image of food trailer or event crowd

2. **The Context**
   - Brief: Started as local catering, needed online presence
   - Challenge: No website, no visibility, no online orders
   - Opportunity: High demand for authentic Mexican food in [location]

3. **What I Built**
   - Website: [elotekingcatering.com](https://elotekingcatering.com)
   - SEO work: Keyword research, local SEO, on-page optimization
   - Result: Catering calls started coming in
   - Visual: Before/after screenshots, analytics graph (if available)

4. **The Impact**
   - Business grew from home kitchen to food trailer
   - 2 events sold out (specific events if you have them)
   - Real revenue impact (quantify if possible: "X% increase in bookings")
   - Visual: Event photos, customer testimonials (real ones only)

5. **What I Learned**
   - Technical: Web development, SEO fundamentals, conversion optimization
   - Business: Market research, pricing strategy, customer acquisition
   - Real-world: "I saw how a good website isn't just code — it's a business tool"

6. **Links + Proof**
   - Live site link: [elotekingcatering.com](https://elotekingcatering.com)
   - GitHub repo (if public)
   - Optional: Press mentions, customer testimonials

7. **CTA**
   - "See another project" → /math-explorations or /creative-labs
   - "Work with me" → /contact

**Conversion focus:**
- This page proves Hayaan delivers real business results
- Targets: recruiters, potential clients, business-minded readers
- Tone: Professional but not corporate. "Here's what I did and why it worked."

---

### Math Explorations (/math-explorations)

**Purpose:** Interactive math visualizations. GHP interview showpiece. Embedded demos.

**Sections:**
1. **Hero**
   - Title: "Math Explorations"
   - Subtitle: "Interactive visualizations of concepts I was curious about. Built to understand, not to impress."
   - CTA: "Jump to demos" (scrolls down)

2. **Why I Built This**
   - 1 paragraph (max 150 words)
   - "I wanted to SEE how math concepts behave, not just work through equations. Building these visualizations forced me to understand chaos theory, prime patterns, randomness, and signal processing at a deeper level. I used AI tools to help with the code, but the math design and insights are mine."
   - Tone: Honest, curious, not overselling

3. **The Demos** (4 embedded visualizations)
   - Each demo lives on this page, no navigation away
   - **Demo 1: Logistic Map (Chaos Theory)**
     - Heading: "How Simple Rules Create Chaos"
     - Interactive: Slider for r parameter (2.4 to 4.0)
     - Visual: Bifurcation diagram + live iteration plot
     - Explanation (1 paragraph): What it is, why it's interesting, what you learned
   - **Demo 2: Ulam Spiral (Prime Patterns)**
     - Heading: "Why Do Primes Make Diagonal Lines?"
     - Interactive: Zoom in/out, highlight diagonals
     - Visual: Spiral grid (50x50 or 100x100), primes highlighted
     - Explanation: Unexpected structure in "random" primes
   - **Demo 3: Random Walks (Probability)**
     - Heading: "How Far Can You Get by Random Chance?"
     - Interactive: Slider for steps, button to run new batch
     - Visual: Single walk trail + heatmap of endpoints
     - Explanation: Connection to diffusion, stock prices, real-world randomness
   - **Demo 4: Fourier Series (Signal Processing)**
     - Heading: "Building Any Wave from Sine Waves"
     - Interactive: Slider for number of terms, dropdown for wave type
     - Visual: Target wave + individual sine terms + running sum
     - Explanation: How MP3s work, why calculus matters in engineering

4. **Technical Notes**
   - Brief: "Built with HTML5 Canvas and vanilla JavaScript. I used AI tools (Claude, ChatGPT) to help structure the code, but I wrote the math functions myself and can explain every part."
   - Link to GitHub repo (if public)
   - Purpose: Transparency + shows you own the work

5. **What's Next**
   - "I want to add visualizations for [X, Y, Z]. This is a living project — I keep adding as I learn."
   - Shows: Ongoing curiosity, not a "done and dusted" portfolio filler

6. **CTA**
   - "See another project" → /elote-king or /creative-labs
   - "Ask me about this" → /contact

**Mobile optimization:**
- Demos must work on mobile (GHP interview use case!)
- Touch-friendly sliders
- Responsive canvas sizing
- Fast load, no lag on interactions

**GHP Interview Use:**
- Judge asks "What have you explored outside class?"
- Pull up hayaandangra.com/math-explorations on phone
- Scroll to logistic map demo
- "Watch what happens when I change this parameter — simple rule, chaotic behavior"
- 30 seconds to 2 minutes max

---

### Creative Labs Learning Center (/creative-labs)

**Purpose:** Teaching and mentoring story. Shows community impact and communication skills.

**Sections:**
1. **Hero**
   - Title: "Creative Labs Learning Center"
   - Subtitle: "Teaching kids to code, think critically, and love learning"
   - Visual: Photo from class or camp (if available)

2. **What Creative Labs Is**
   - Brief: Mom's business, Hayaan teaches coding and tutoring
   - Programs: After-school coding classes, summer camps, 1-on-1 tutoring
   - Age range: [specific ages if you have them]

3. **What I Teach**
   - Coding: Scratch, Python basics, web development fundamentals
   - Math tutoring: [grade levels/topics]
   - Critical thinking: Problem-solving, debugging mindset
   - Visual: Curriculum overview or class photos

4. **Why I Do This**
   - "I love the moment when a concept clicks for a student. Teaching forces me to understand things deeply enough to explain them simply. It's also shown me how much I enjoy mentoring — helping someone else grow is as rewarding as learning myself."
   - Tone: Genuine, not resume-paddy

5. **Student Outcomes** (if you have data)
   - "X students taught over Y years"
   - Testimonials from parents/students (real ones only)
   - Success stories: "One student built their first website after 8 weeks"

6. **CTA**
   - "Interested in classes?" → Link to Creative Labs website or contact
   - "See another project" → /elote-king or /math-explorations

**Conversion focus:**
- This page shows: communication skills, patience, leadership
- Targets: College admissions (community impact), potential collaborators
- Tone: Humble, focused on students' growth, not self-promotion

---

### About (/about)

**Purpose:** Full background, resume-style info, personal context.

**Sections:**
1. **Who I Am**
   - Name, school (Alliance Academy), location (Georgia)
   - Grade (high school senior)
   - Interests: "I build websites, explore math, teach coding, and I'm figuring out where tech and healthcare intersect."

2. **Education + Pathways**
   - Alliance Academy (Cyber Security pathway, Healthcare pathway)
   - GHP Math Semifinalist (if you advance, update to finalist/participant)
   - Relevant coursework: AP Calc, AP Stats, etc.

3. **Skills**
   - **Web Development:** HTML, CSS, JavaScript, Astro, SEO
   - **Tools:** GitHub, Vercel, VS Code, AI-assisted coding (Claude, ChatGPT)
   - **Math:** Calculus, statistics, dynamical systems, number theory
   - **Teaching:** Coding instruction, tutoring, curriculum design

4. **Projects** (brief list with links)
   - Elote King → /elote-king
   - Math Explorations → /math-explorations
   - Creative Labs → /creative-labs

5. **What I'm Learning**
   - Current focus: [e.g., "Cyber security fundamentals, web security best practices"]
   - Future interests: [e.g., "Healthcare tech, patient data systems, bioinformatics"]
   - Shows: Growth mindset, future trajectory

6. **Outside of Projects**
   - Hobbies, interests, personality (optional, keeps it human)
   - Example: "I love [X], play [sport/instrument], and I'm always looking for the next thing to build."

7. **CTA**
   - "Want to collaborate?" → /contact
   - "Check out my work" → / (back to home)

**Tone:**
- Professional but not corporate
- Honest about using AI tools
- Focused on growth and learning, not achievements

---

### Journal (/journal) — OPTIONAL

**Purpose:** Build-in-public posts. Blog for project updates, learning reflections, insights.

**When to add this:**
- **Add later** (after core site is live)
- **Add if Hayaan actually wants to write** (don't force it)
- **Add if there's content to share** (project updates, math insights, business learnings)

**If you build it:**

**Structure:**
- Blog roll (most recent first)
- Post format:
  - Title
  - Date
  - Short excerpt
  - "Read more" link to full post
- Categories: "Projects", "Math", "Business", "Learning"

**Sample posts:**
- "How I Built the Logistic Map Visualization"
- "What I Learned Doing SEO for a Real Business"
- "Teaching Kids to Code: What Works, What Doesn't"
- "How I Use AI Tools for Coding (Honestly)"

**SEO benefits:**
- Fresh content signals to Google
- Long-tail keyword opportunities
- Backlink magnet (if posts get shared)

**Social integration:**
- Auto-post excerpts to X and LinkedIn
- Cross-link: Journal post → X thread → LinkedIn article
- Builds online presence beyond static portfolio

**If you skip it:**
- No problem. Static portfolio is enough.
- Can always add later without redesigning.

---

### Contact (/contact)

**Purpose:** Contact form + social links. Conversion endpoint for all CTAs.

**Sections:**
1. **Hero**
   - Title: "Let's Connect"
   - Subtitle: "Interested in working together, have a question, or just want to chat? Reach out."

2. **Contact Form**
   - Fields:
     - Name (required)
     - Email (required)
     - Subject (dropdown: "Project inquiry", "Job opportunity", "Collaboration", "General question")
     - Message (required)
   - Submit button: "Send message" (action verb, not "Submit")
   - Backend: Formspree (free tier, no setup)
   - Success state: "Thanks! I'll get back to you within 48 hours."

3. **Social Links**
   - X: [link]
   - LinkedIn: [link]
   - GitHub: [link]
   - Email: [email]
   - Visual: Icon buttons, clean layout

4. **Response Time**
   - "I typically respond within 1-2 business days. If it's urgent, DM me on X."

**Conversion focus:**
- Low friction: 4 fields max, no captcha (Formspree handles spam)
- Clear CTA: "Send message" not "Submit"
- Multiple contact options: Form, social, email (user chooses)

---

## SITE-WIDE DESIGN SYSTEM

### Visual Identity

**Typography:**
- **Headers:** Bebas Neue (bold, high-impact)
- **Body:** DM Sans (clean, readable, modern)
- **Code:** Monospace (for technical sections)

**Font Sizes:**
- Hero title: 48px desktop, 32px mobile
- Section headers: 36px desktop, 24px mobile
- Body text: 18px desktop, 16px mobile (NEVER below 16px)
- Min absolute: 13px (only for captions/metadata)

**Colors:**
- **Primary:** TBD (Hayaan's preference — suggest: deep blue or teal for tech feel)
- **Accent:** TBD (suggest: bright orange or yellow for CTAs)
- **Background:** White (default, clean, professional)
- **Text:** Dark gray (#333 or #222), not pure black (easier on eyes)
- **Links:** Blue (standard web convention) or primary color

**Spacing:**
- Generous whitespace (mobile: 20px padding, desktop: 40px)
- Section padding: 80px vertical desktop, 40px mobile
- Component spacing: 24px between elements

**Imagery:**
- Real photos (no stock photos)
- Optimized for web (WebP format, lazy-load)
- Alt text for accessibility
- Aspect ratios: 16:9 for hero images, 4:3 for project cards

### Layout Patterns

**Hero sections:**
- Full-width background (image or solid color)
- Centered text
- CTA buttons: Primary (filled) + Secondary (outline)

**Project cards:**
- Image top, text bottom
- Hover effect: slight lift + shadow
- CTA button: "Learn more", "Read case study", "Explore"

**Content sections:**
- Max width: 1200px (desktop)
- Two-column on desktop, single-column on mobile
- Left: Text, Right: Visual (alternates per section)

### Navigation

**Desktop:**
- Horizontal nav bar (sticky on scroll)
- Logo/Name left
- Links right: "Projects", "About", "Journal" (if exists), "Contact"
- CTA button: "Contact me" (accent color)

**Mobile:**
- Hamburger menu (top right)
- Overlay menu on click
- Logo/Name top left
- Menu links: Same as desktop

**Behavior:**
- Smooth scroll for anchor links
- Active state for current page
- Hover effects on links

### Footer

**Content:**
- Name + tagline
- Navigation links (same as header)
- Social icons
- Copyright: "© 2026 Hayaan Dangra. Built with Astro."

**Layout:**
- Three columns desktop, stacked mobile
- Background: Light gray (#f5f5f5)
- Text: Dark gray

---

## ASTRO PROJECT FILE STRUCTURE

```
hayaandangra.com/
├── src/
│   ├── layouts/
│   │   └── BaseLayout.astro          # Main layout (header, footer, meta tags)
│   ├── pages/
│   │   ├── index.astro               # Home page
│   │   ├── elote-king.astro          # Elote King case study
│   │   ├── math-explorations.astro   # Math demos (with embedded JS)
│   │   ├── creative-labs.astro       # Teaching story
│   │   ├── about.astro               # Full background
│   │   ├── journal/                  # Optional blog
│   │   │   ├── index.astro           # Blog roll
│   │   │   └── [slug].astro          # Individual posts
│   │   └── contact.astro             # Contact form
│   ├── components/
│   │   ├── Header.astro              # Site header/nav
│   │   ├── Footer.astro              # Site footer
│   │   ├── ProjectCard.astro         # Reusable project card
│   │   ├── Hero.astro                # Reusable hero section
│   │   ├── CTA.astro                 # Reusable CTA button
│   │   └── MathDemo.astro            # Wrapper for math visualizations
│   ├── scripts/
│   │   ├── logistic-map.js           # Logistic map viz
│   │   ├── ulam-spiral.js            # Ulam spiral viz
│   │   ├── random-walk.js            # Random walk viz
│   │   └── fourier-series.js         # Fourier series viz
│   ├── styles/
│   │   ├── global.css                # Global styles, typography, reset
│   │   ├── variables.css             # CSS custom properties (colors, spacing)
│   │   └── components.css            # Component-specific styles
│   └── content/
│       └── journal/                  # Optional: Markdown blog posts
│           ├── post-1.md
│           └── post-2.md
├── public/
│   ├── images/
│   │   ├── elote-king/               # Elote King assets
│   │   ├── math-explorations/        # Math demo screenshots
│   │   ├── creative-labs/            # Teaching photos
│   │   └── headshot.jpg              # Hayaan's photo
│   ├── favicon.ico
│   ├── og-image.jpg                  # OpenGraph image for social sharing
│   └── robots.txt
├── astro.config.mjs
├── package.json
├── README.md
└── .gitignore
```

### Key Files Explained

**BaseLayout.astro**
- Wraps all pages
- Includes: `<head>` (meta tags, fonts, SEO), Header, Footer
- Injects global CSS
- Sets up: title, description, og:image per page

**index.astro (Home)**
- Hero section
- Featured projects (3 cards)
- Pathways + future projects
- Connect section (social links)

**math-explorations.astro**
- Hero + "Why I built this"
- 4 embedded demos (canvas elements)
- Each demo: heading + interactive controls + explanation
- Technical notes + GitHub link
- Imports: All 4 JS visualization scripts

**elote-king.astro**
- Full case study structure
- Sections: Context, What I Built, Impact, Learnings, Links
- Images: Before/after, event photos, analytics

**contact.astro**
- Contact form (Formspree backend)
- Social links
- Success state (client-side JS)

**components/ProjectCard.astro**
- Props: title, description, image, link
- Reused on home page for all 3 featured projects

---

## RESPONSIVE BREAKPOINTS

```css
/* Mobile first (default) */
/* 0-767px: Base styles */

/* Tablet */
@media (min-width: 768px) {
  /* Two-column layouts, larger text */
}

/* Desktop */
@media (min-width: 1024px) {
  /* Three-column layouts, full nav, larger hero */
}

/* Large desktop */
@media (min-width: 1440px) {
  /* Max content width, larger padding */
}
```

### Mobile-First Rules
1. Start with mobile layout (single column, stacked)
2. Use min-width media queries to enhance for larger screens
3. Touch targets: 44px minimum (buttons, links)
4. No hover effects on mobile (use :active instead)
5. Hamburger menu below 768px

---

## SEO STRATEGY

### Per-Page Meta Tags

**Home (/):**
- Title: "Hayaan Dangra — High School Senior, Web Developer, Math Explorer"
- Description: "I build websites, explore math, and teach coding. Check out my projects: Elote King (business case study), GHP Math Explorations (interactive visualizations), and Creative Labs (teaching)."
- og:image: Headshot or abstract visual
- Keywords: "high school developer", "portfolio", "web development", "math visualizations", "Georgia student"

**Elote King (/elote-king):**
- Title: "Elote King Case Study — From Website to Food Trailer | Hayaan Dangra"
- Description: "How I built a website and SEO strategy that helped a local catering business grow to a food trailer with 2 sold-out events. Full case study."
- og:image: Screenshot of elotekingcatering.com or event photo
- Keywords: "case study", "SEO", "small business website", "web development portfolio"

**Math Explorations (/math-explorations):**
- Title: "Interactive Math Visualizations — Chaos, Primes, Random Walks | Hayaan Dangra"
- Description: "Explore chaos theory, prime patterns, random walks, and Fourier series through interactive visualizations. Built to understand, not to impress."
- og:image: Screenshot of logistic map or bifurcation diagram
- Keywords: "math visualizations", "chaos theory", "Fourier series", "interactive math", "GHP"

**Creative Labs (/creative-labs):**
- Title: "Teaching Kids to Code — Creative Labs Learning Center | Hayaan Dangra"
- Description: "Teaching coding, tutoring math, and running summer camps at Creative Labs Learning Center. How I help kids love learning."
- og:image: Photo from class or camp
- Keywords: "coding teacher", "tutoring", "STEM education", "youth mentorship"

**About (/about):**
- Title: "About Hayaan Dangra — High School Senior, Developer, Math Explorer"
- Description: "High school senior at Alliance Academy (Georgia). Cyber Security and Healthcare pathways. I build websites, explore math, and teach coding."
- og:image: Headshot
- Keywords: "about", "resume", "portfolio", "student developer"

**Contact (/contact):**
- Title: "Contact Hayaan Dangra — Let's Connect"
- Description: "Interested in working together? Have a question? Reach out via contact form, email, or social media."
- og:image: Abstract visual or headshot
- Keywords: "contact", "hire", "collaborate"

### Global SEO Setup
- **Sitemap:** Auto-generated by Astro
- **Robots.txt:** Allow all
- **Structured data:** JSON-LD for Person schema (on About page)
- **Image optimization:** WebP format, descriptive alt text
- **Performance:** Lighthouse score 90+ (mobile and desktop)

---

## INTEGRATION WITH SOCIAL MEDIA

### X (Twitter) Strategy
- Bio: "High school senior. I build websites, explore math, and teach coding. Check out my work: hayaandangra.com"
- Pin tweet: "Just launched my portfolio site. Check out how I helped Elote King grow to a food trailer, my GHP math explorations, and my teaching work. [link]"
- Content strategy:
  - Share project updates ("Just added [X] to my math explorations")
  - Cross-post journal articles (if journal exists)
  - Engage with math/tech/education communities
  - Use hashtags: #buildinpublic, #GHP, #mathviz, #webdev

### LinkedIn Strategy
- Headline: "High School Senior | Web Developer | Math Explorer | Teaching @ Creative Labs"
- Featured section: Link to hayaandangra.com + 3 project pages
- Experience:
  - "Web Developer — Elote King Catering" (with link to case study)
  - "Coding Instructor — Creative Labs Learning Center" (with link to teaching page)
- Projects section: All 3 projects with links
- Content strategy:
  - Share professional updates (project launches, achievements)
  - Long-form posts (journal articles expanded)
  - Engage with education/tech professionals

### GitHub Strategy
- Profile README: Link to hayaandangra.com + brief intro
- Pin repositories:
  - hayaandangra.com (portfolio site source code)
  - elote-king (if public)
  - math-explorations (if public)
- README files: Clear documentation, screenshots, setup instructions

### Cross-Posting Workflow
1. Publish journal post on hayaandangra.com/journal
2. Auto-generate excerpt + link
3. Post to X (thread format if long)
4. Post to LinkedIn (professional tone, expanded)
5. Update GitHub README if technical project

---

## FUTURE-PROOFING

### How New Projects Get Added

**Scenario 1: Cyber Security Project**
- Add new project card to home page (Featured Projects section)
- Create new page: /cyber-security-project.astro
- Update About page (add to Skills or Projects section)
- Add to navigation (if major project)

**Scenario 2: Healthcare Pathway Project**
- Same process as Cyber Security
- Update "Pathways + Future Projects" section on home
- Write journal post about the project (build-in-public)

**Scenario 3: New Math Visualization**
- Add to /math-explorations page (no new page needed)
- Update "What's Next" section
- Write script file in /scripts/
- Cross-post to X and LinkedIn

**Scenario 4: New Teaching Project**
- Add to /creative-labs page or create separate page
- Update home page if significant

### Design Scalability
- **Component-based:** Reusable components (ProjectCard, Hero, CTA) mean adding projects is copy-paste
- **Content-driven:** Astro supports Markdown content collections (journal scales easily)
- **CSS variables:** Change colors/fonts site-wide by editing variables.css
- **No hardcoded content:** All project data can move to JSON/Markdown (future upgrade)

### When to Redesign
- **Don't redesign when:** Adding 1-3 new projects (just add pages)
- **Consider redesign when:** 10+ projects (need better filtering/categorization)
- **Definitely redesign when:** Graduating, career shift, or site doesn't reflect current skills

---

## TECHNICAL IMPLEMENTATION NOTES

### Astro-Specific Setup

**astro.config.mjs**
```javascript
import { defineConfig } from 'astro/config';

export default defineConfig({
  site: 'https://hayaandangra.com',
  output: 'static', // Static site generation
  build: {
    format: 'directory', // Clean URLs (/about instead of /about.html)
  },
});
```

**package.json dependencies**
```json
{
  "dependencies": {
    "astro": "^4.0.0"
  },
  "devDependencies": {
    "@astrojs/sitemap": "^3.0.0"
  }
}
```

### Math Visualizations Tech Stack
- **Canvas API:** Native browser, no libraries (keeps it simple)
- **Vanilla JS:** No React, no Vue (you can explain every line)
- **Interaction:** HTML range inputs (sliders) + buttons
- **Responsive:** Canvas resizes based on viewport
- **Performance:** RequestAnimationFrame for smooth animations

### Form Backend (Formspree)
- Free tier: 50 submissions/month
- Setup: Add Formspree endpoint to form action
- No backend code needed
- Anti-spam built-in
- Email notifications on new submission

### Hosting (Vercel)
- Free tier: Unlimited bandwidth, custom domain
- Deploy: Connect GitHub repo, auto-deploy on push
- Custom domain: hayaandangra.com (point DNS to Vercel)
- SSL: Automatic (HTTPS)
- Performance: Edge network, fast global load times

### Analytics (Optional)
- **Google Analytics 4:** Free, standard web analytics
- **Plausible:** Privacy-friendly alternative (paid)
- **Decision:** Add after launch, not before (focus on content first)

---

## LAUNCH CHECKLIST

### Pre-Launch
- [ ] All pages built and tested (desktop + mobile)
- [ ] Math demos work on phone (GHP interview test)
- [ ] Forms submit successfully (test Formspree)
- [ ] All images optimized (WebP, lazy-load)
- [ ] No console errors (check browser dev tools)
- [ ] SEO tags set on all pages
- [ ] Favicon and og:image present
- [ ] Social links correct (X, LinkedIn, GitHub, email)
- [ ] Text readable at 375px mobile width
- [ ] Load time under 3 seconds (Lighthouse test)

### Launch Day
- [ ] Push to GitHub
- [ ] Deploy to Vercel
- [ ] Connect custom domain (hayaandangra.com)
- [ ] Test all pages on live site
- [ ] Submit sitemap to Google Search Console
- [ ] Share on X and LinkedIn
- [ ] Pin tweet on X
- [ ] Update LinkedIn featured section

### Post-Launch
- [ ] Monitor Formspree for spam
- [ ] Check analytics (if installed)
- [ ] Fix any bugs reported
- [ ] Add journal posts (if relevant)
- [ ] Update with new projects as they happen

---

## ANSWERS TO YOUR SPECIFIC QUESTIONS

### 1. Architect the site structure
**Answer:** 6 pages (Home, Elote King, Math Explorations, Creative Labs, About, Contact) + optional Journal. Single-page home with project previews, deep-dive pages for major projects. See full structure above.

### 2. How does the math visualization integrate?
**Answer:** Lives on its own page (/math-explorations) with all 4 demos embedded directly. No external links, no navigation away. Pull up on phone during GHP interview. Also previewed on home page as one of 3 featured projects.

### 3. How does Elote King get presented?
**Answer:** Full case study page (/elote-king) with sections: Context, What I Built, Impact, Learnings, Links. Featured prominently on home page as primary project. Proves business impact and real-world results.

### 4. How do future projects get added without redesigning?
**Answer:** Component-based architecture. Add new page (e.g., /cyber-security-project.astro), create new ProjectCard on home page, update About. No redesign needed until 10+ projects.

### 5. Should there be a blog/journal?
**Answer:** OPTIONAL. Add later if Hayaan wants to write. Benefits: Fresh content for SEO, build-in-public narrative, cross-posting to X/LinkedIn. Skip if no time or interest. Static portfolio is enough.

### 6. Can he pull up the site on his phone for GHP?
**Answer:** YES. /math-explorations page is fully mobile-responsive. Touch-friendly sliders, canvas elements resize, fast load. Test on phone before interview. Pull up, scroll to logistic map demo, show chaos bifurcation in 30 seconds.

### 7. Information architecture: what does each audience see?
**Answer:**
- **College admissions:** Home page hero → Elote King (business impact) → Math explorations (intellectual curiosity) → Creative Labs (community) → About (full background)
- **GHP judge:** /math-explorations on phone, demo during interview, shows independent learning and technical execution
- **Internship recruiter:** Home page → Elote King (marketing/SEO skills) → Math explorations (technical depth) → Contact (CTA)

### 8. How does this connect to X and LinkedIn?
**Answer:** Social links in footer and contact page. Cross-post journal articles (if journal exists) to X (thread format) and LinkedIn (expanded professional post). Profile bios link to hayaandangra.com. Pin tweet on X featuring portfolio.

### 9. Site map with file structure
**Answer:** See "ASTRO PROJECT FILE STRUCTURE" section above. Full directory layout with all pages, components, scripts, and assets.

---

## NEXT STEPS

1. **Review this architecture with Hayaan**
   - Does he agree with the project hierarchy? (Elote King first, math second, Creative Labs third)
   - Does he want a journal/blog? (Optional, can add later)
   - Any projects missing? (Other work he's done that should be featured)

2. **Gather assets**
   - Headshot photo
   - Elote King: Website screenshots, event photos, analytics data (if available)
   - Math explorations: Demo screenshots (for preview cards)
   - Creative Labs: Class photos or camp photos (if available)
   - Social media: Confirm X handle, LinkedIn URL, GitHub username, email

3. **Build in phases**
   - **Phase 1:** Home page + About + Contact (core structure)
   - **Phase 2:** Elote King case study (strongest project, full story)
   - **Phase 3:** Math explorations (GHP demos embedded)
   - **Phase 4:** Creative Labs (teaching story)
   - **Phase 5:** Journal (optional, add later)

4. **Deploy and test**
   - Push to GitHub
   - Deploy to Vercel
   - Test on desktop, tablet, mobile
   - Test math demos on phone (GHP interview scenario)
   - Fix bugs, optimize load times

5. **Launch and promote**
   - Share on X and LinkedIn
   - Update all social media bios to link to hayaandangra.com
   - Submit to Google Search Console
   - Optional: Share in relevant communities (GHP alumni groups, student dev communities)

---

## FINAL NOTES

**This is a LIVING portfolio.**
- Start with core pages (Home, Elote King, Math, Creative Labs, About, Contact)
- Add journal later if Hayaan wants to write
- New projects get added as cards + pages, no redesign needed
- Site grows with Hayaan's work throughout high school and beyond

**Design philosophy:**
- Clean, professional, not flashy
- Content-first (work speaks for itself)
- Mobile-friendly (GHP interview use case)
- Fast, accessible, semantic HTML

**Tone:**
- Honest about using AI tools
- Focused on learning and growth, not achievements
- Real results (Elote King revenue, sold-out events, teaching impact)
- No fake social proof, no resume bloat

**Key differentiator:**
- This isn't a static resume. It's a showcase of real work with real impact.
- Elote King = business results
- Math explorations = intellectual curiosity
- Creative Labs = community impact
- Future projects = growth trajectory

Build this, ship it, iterate as needed.
