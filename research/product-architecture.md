# GHP Math Interview Project - Product Architecture
**For: High School Senior, GHP Math Semifinalist**
**Context: Interview conversation piece (NOT presentation centerpiece)**
**Date: February 2026**

---

## EXECUTIVE SUMMARY

**Project:** Interactive Math Exploration Portfolio
**Format:** Single-page web app with 4 focused visualizations
**Time Investment:** 8-12 hours total build time
**Interview Use:** 30-second mention → 2-minute demo if asked
**Core Message:** "I built this to explore math concepts I was curious about beyond the classroom"

---

## THE STRATEGIC FRAME

### What GHP Judges Actually Care About
- **Genuine curiosity:** Did you explore this because YOU wanted to, or because it sounds impressive?
- **Independent learning:** Can you explain what you learned and how you figured it out?
- **Mathematical breadth:** Do you appreciate different areas of math, not just calc/competition?
- **Creative problem-solving:** Did you make connections or ask interesting questions?

### What They Don't Care About (for this interview)
- Advanced tech stack complexity
- Research paper-level rigor
- Whether you could publish this
- Comparison to college-level work

### The Interview Reality
- You have 15-20 minutes total
- They'll ask about your math interests, problem-solving approach, favorite topics
- This project is ONE data point among: your application, your responses, your problem-solving on the spot
- If you spend 2 minutes on this, that's 10% of your interview

**Conclusion:** Build something authentic, explainable, and genuinely interesting to YOU. Don't overbuild.

---

## ARCHITECTURE DECISION: 4 FOCUSED DEMOS

**Not 2-3:** Too narrow, doesn't show breadth
**Not 5-7:** Spread too thin, looks like a checklist

**4 demos = 4 corners of math:**
1. **Visual/Geometric** - something you can see and manipulate
2. **Probabilistic/Random** - something with uncertainty and patterns
3. **Algebraic/Number Theory** - something with structure and properties
4. **Applied/Modeling** - something connected to real phenomena

This shows: "I appreciate different flavors of math, not just the calc track"

---

## THE 4 RECOMMENDED DEMOS

### Demo 1: Chaos and Sensitivity (Logistic Map)
**Math Concept:** The logistic map: x(n+1) = r * x(n) * (1 - x(n))
**Why This Works:**
- Taught in AP Calc (difference equations, iteration)
- Visually stunning (bifurcation diagram, period-doubling route to chaos)
- Accessible explanation: "Small changes in r create wildly different long-term behavior"
- Connection point: "I wanted to understand how simple rules create complex patterns"

**Can a 17-year-old explain it?** YES.
- "It's a population model where growth is limited by resources"
- "The r parameter controls reproduction rate"
- "Watch what happens when I slowly increase r - the pattern goes from stable to chaotic"
- "This is why weather is hard to predict - tiny changes compound"

**Visual:** Bifurcation diagram (r on x-axis, long-term behavior on y-axis) + live iteration plot
**Interaction:** Slider for r value (2.4 to 4.0), shows both fixed points and chaos

**What Makes It Interview-Gold:**
- Bridges calc (sequences, limits) and dynamical systems
- Clear "wow" moment when chaos appears
- Easy to explain why you cared: "I wanted to see order become disorder"

---

### Demo 2: Prime Spirals (Ulam Spiral)
**Math Concept:** Plot integers in a spiral, highlight primes - diagonal patterns emerge
**Why This Works:**
- Number theory (primes) is HS-accessible
- Visually unexpected - "why would primes make diagonal lines?"
- Ties to unsolved problems (prime gaps, distribution) WITHOUT requiring you to solve them
- Shows genuine curiosity: "I heard primes were random, but this shows structure"

**Can a 17-year-old explain it?** YES.
- "Start at center, spiral outward: 1, 2, 3, 4, 5..."
- "Color the primes differently"
- "These diagonal lines appear - they're related to quadratic polynomials that generate primes"
- "We don't fully understand why, which is cool"

**Visual:** Spiral grid (50x50 or 100x100), primes in one color, composites in another
**Interaction:** Zoom in/out, highlight specific diagonals, show the polynomial (x² + x + 41)

**What Makes It Interview-Gold:**
- Connects to competition math (primes, sieves, patterns)
- Honest about the math: "This is an open area of research"
- Shows you're comfortable with "I don't know why, but here's what I observed"

---

### Demo 3: Random Walks and Probability (2D Random Walk)
**Math Concept:** Start at origin, take random steps N/S/E/W - how far do you get?
**Why This Works:**
- AP Stats connection (random processes, expected value)
- Intuitive to explain, surprising in behavior
- Ties to diffusion, Brownian motion, stock prices (real applications)
- Shows you think about randomness mathematically

**Can a 17-year-old explain it?** YES.
- "Flip a coin 4 times: heads = north, tails = south, etc."
- "Run this 1000 times - where do most walks end up?"
- "The average distance grows with √n steps, not n"
- "This is how particles diffuse, how rumors spread, how stock prices move"

**Visual:**
- Single walk animated path (colorful trail)
- Heatmap of 1000+ walk endpoints
- Distance-from-origin histogram

**Interaction:**
- Slider for number of steps (10, 50, 100, 500)
- Button to run new batch of walks
- Toggle between single walk and aggregate view

**What Makes It Interview-Gold:**
- Bridges pure math (probability) and applied (physics, finance)
- You can DO it physically: "I could flip coins and walk around my room"
- Shows computational thinking: "I used simulation to explore the math"

---

### Demo 4: Fourier Series Approximation (Draw Any Wave)
**Math Concept:** Any periodic function = sum of sine waves (Fourier series)
**Why This Works:**
- Taught in AP Calc BC (series, convergence)
- Mind-blowing visual: sine waves → square wave
- Ties to music (harmonics), signal processing, image compression
- Shows you understand calculus beyond derivatives

**Can a 17-year-old explain it?** YES.
- "Any repeating wave can be built from sine waves"
- "A square wave looks nothing like a sine wave, but watch what happens when I add sines with the right frequencies and amplitudes"
- "More terms = closer approximation (show 1, 5, 20, 100 terms)"
- "This is how MP3s compress music - they store the sine wave recipe, not the full waveform"

**Visual:**
- Target wave (square, triangle, sawtooth - user selects)
- Individual sine terms stacked
- Running sum approaching target
- Residual error plot

**Interaction:**
- Slider for number of terms (1 to 50)
- Dropdown for wave type
- Play button to animate the series building up

**What Makes It Interview-Gold:**
- Connects pure math (infinite series) to engineering (signal processing)
- Explains why you cared: "I wanted to understand how Spotify works"
- Shows you appreciate the power of calculus in the real world

---

## WHAT TO EXCLUDE (THE "DON'T OVERBUILD" LIST)

### Too Advanced (Judges Will Be Skeptical)
- Differential equations (unless you've taken them - even then, risky)
- Topology (manifolds, homeomorphisms - too abstract)
- Abstract algebra (group theory, rings - no visual hook)
- Advanced chaos theory (Lorenz attractor - you can't explain the ODEs)
- Machine learning (you didn't train the model, you used a library)

### Too Simple (Doesn't Show Exploration)
- Basic graphing calculator functions (y = mx + b sliders)
- Pythagorean theorem visualizations (too elementary)
- Memorization tools (multiplication tables, unit circle)

### Wrong Signal
- Anything you clearly copied from a tutorial without understanding
- Anything that looks like "I Googled 'cool math visualizations' and picked 5"
- Anything with incorrect math (judges WILL notice)

### Red Flags in Explanation
If you can't answer these for each demo, DON'T INCLUDE IT:
- "Why did you choose to explore this?"
- "What did you learn that surprised you?"
- "How would you explain this to someone who's taken pre-calc?"
- "What would you explore next if you had more time?"

---

## TECH STACK RECOMMENDATION

### The Right Stack for a High School Senior
**Frontend:** Plain HTML + vanilla JavaScript (NO frameworks)
**Visualization:** Canvas API (native browser, no libraries) OR p5.js (if you want easier drawing)
**Math:** Write your own functions (don't import numpy.js or math.js unless absolutely needed)
**Styling:** Simple CSS, clean and readable
**Hosting:** GitHub Pages (free, easy, shows you can use git)

### Why This Stack?
- **You can explain every line:** No "magic" framework code you don't understand
- **No build process:** No webpack, no npm, no mysterious errors
- **Fast development:** 2-3 hours per demo, not 2-3 days
- **Honest ownership:** "I wrote the simulation loop myself" is way better than "I used react-three-fiber"

### What You Can Say in the Interview
"I used JavaScript and Canvas because I wanted to understand the math directly, not just use a library. I wrote the logistic map iteration myself, the prime-checking sieve, the random walk simulation. The code is simple enough that I can explain any part of it."

### What You Should NOT Say
"I used React with TypeScript and WebGL shaders because I wanted to learn modern web development." (Wrong goal - this isn't a hackathon)

---

## SCOPE AND TIMELINE

### Build Time Per Demo
- **Demo setup (HTML structure, canvas, UI):** 30 minutes
- **Math implementation:** 1 hour
- **Visualization and interactivity:** 1 hour
- **Testing and polish:** 30 minutes
- **Total per demo:** ~3 hours

### Total Project Time
- **4 demos:** 12 hours
- **Landing page + navigation:** 1 hour
- **Testing and bug fixes:** 1 hour
- **Deployment:** 30 minutes
- **Total:** 14-15 hours over a weekend

### If You're Short on Time
**Minimum Viable Version:** 3 demos (chaos, primes, random walk) in 9 hours
**Skip:** Fourier series (most complex to code)
**Keep:** The other three cover geometric, number theory, and probabilistic thinking

---

## INTERVIEW STRATEGY

### How to Reference This Project
**If they ask "What math have you explored outside of class?"**
> "I built a web app to visualize math concepts I was curious about - things like how simple rules create chaos, why primes show up in spiral patterns, and how random walks behave. I wanted to see the math, not just work through problem sets."

**If they ask "Can you show us?"**
> (Pull up laptop or phone) "Here's the logistic map - watch what happens as I increase this parameter. It goes from stable to chaotic. I was fascinated by how such a simple equation could be so unpredictable."

**If they DON'T ask:**
> (Mention it in response to "What math topics interest you?") "I've been exploring dynamical systems and number theory - I even built some interactive visualizations to understand them better."

### What NOT to Do
- Don't lead with the project (it's a supporting detail, not your main pitch)
- Don't spend more than 2 minutes on it unless they're genuinely interested
- Don't say "I built this for GHP" (say "I was curious" even if GHP motivated you)
- Don't oversell: "This is just something I made to explore, not research"

### If They Dig Deeper
**"How did you learn to code this?"**
> "I used AI tools to help with the syntax, but I made sure I understood every concept. I can walk through any part of the code."

**"What did you learn?"**
> "I learned that simple mathematical rules can have incredibly complex behavior. And I realized I love the process of exploring math through experiments and visualization, not just proofs."

**"What would you add next?"**
> (Pick ONE genuine extension) "I'd love to explore the Collatz conjecture visually - it's another case where simple rules lead to mysterious patterns."

---

## THE AUTHENTICITY TEST

Before you call this done, answer these honestly:

1. **Can you explain each demo to your math teacher without notes?** (If no, simplify it)
2. **Did you pick these topics because YOU find them interesting?** (If no, pick different ones)
3. **Could you code a 5th demo in the same style without help?** (If no, you don't own the code)
4. **If the judges ask "why this topic?" do you have a real answer?** (If no, you don't own the story)

If you can't answer YES to all four, you've overbuilt or picked the wrong topics.

---

## FINAL RECOMMENDATION

**Build this project:**
- 4 demos (chaos, primes, random walk, Fourier)
- Plain HTML/JS, no frameworks
- 12-15 hours total time
- Host on GitHub Pages
- Write a 1-paragraph "why I built this" at the top of the page

**Use it in the interview as:**
- A 30-second mention when relevant
- A 2-minute demo if they're interested
- Evidence that you explore math independently

**Don't:**
- Make it the center of your interview
- Overbuild with advanced tech
- Pick topics you can't fully explain
- Pretend you didn't use AI assistance (be honest: "I used AI for syntax, but I own the concepts")

**The goal:** Show genuine curiosity, independent learning, and mathematical breadth. That's what gets you to GHP finals, not the complexity of your code.

---

## NEXT STEPS

1. **Validate with student:** Do these topics genuinely interest you? Swap any that don't.
2. **Start with ONE demo:** Build the logistic map first (2-3 hours). If you can explain it confidently, proceed.
3. **Build the other 3 demos:** One per day over a long weekend.
4. **Practice explaining:** Spend as much time practicing your explanation as you did coding.
5. **Deploy and test:** Make sure it works on mobile (judges might ask to see it on your phone).

**Remember:** This is a conversation piece, not a thesis defense. Keep it authentic, explainable, and genuinely interesting to you.
