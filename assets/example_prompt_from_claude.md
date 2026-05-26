# Kden Model Website - Claude Code Prompt

You are building a **landing & product showcase website** for **Kden**, a state-of-the-art 64M MoE (Mixture of Experts) language model powered by Retrieval Transformers (RT) that operates purely on text—no multimodal distractions, pure performance.

---

## Core Brand Identity

**What is Kden?**
- 64 Million parameters, MoE architecture (sparse, efficient)
- Retrieval Transformer backbone (RT) for grounded, accurate responses
- Non-multimodal: Text-only focus = laser-sharp performance
- Positioning: High-performance, specialized, no bloat

**Brand Personality:** Technical precision, confidence, innovation, efficiency
**Emotional Goals:** Users should feel: "This is built for serious work"

---

## Build Instructions

### Phase 1: Design Intelligence (activate `ui-ux-pro-max`)
Use design research to inform every decision:

1. **Product Positioning:** Search for SaaS AI model APIs, LLM landing pages, developer tools
2. **Style Direction:** Modern, minimal, technical but not cold. Consider glassmorphism for the techy vibe
3. **Typography:** Professional + modern (pair elegant serif with clean sans)
4. **Color Palette:** Dark mode with electric accents (cyan, violet, or electric blue to suggest power/speed)
5. **Layout Strategy:** Hero-centric with performance metrics, feature comparison, live API demo area
6. **UX Best Practices:** Smooth interactions, hover states, accessibility compliance

### Phase 2: Design Context (activate `teach-impeccable`)
After design research, document all decisions:

1. **Create `.impeccable.md`** in project root capturing:
   - **Users:** ML engineers, product builders, researchers evaluating models
   - **Brand Personality:** Precision, efficiency, innovation
   - **Aesthetic Direction:** Dark, technical, modern minimal with electric accents
   - **Design Principles:**
     - Performance-first (visuals + content load fast)
     - Trust through transparency (model specs, benchmarks visible)
     - Clarity over decoration (every element serves a purpose)
     - Accessibility built-in (WCAG AA minimum)

2. **Document key design tokens:** Colors, spacing, typography rules

### Phase 3: Implementation (React + Tailwind recommended)

**Key Sections to Build:**

#### Hero Section
- Headline: Something like "Kden: 64M Parameters. Pure Text. Maximum Performance."
- Subheadline: Emphasize the MoE + RT advantage
- CTA buttons: "View Benchmarks" | "Try API" | "Read Docs"
- Background: Subtle animated gradient or particle effect (performance-conscious)

#### Key Features / Why Kden
- **MoE Architecture:** Sparse, efficient inference
- **Retrieval Transformer:** Grounded responses, reduces hallucinations
- **Text-Only Focus:** No bloat, pure language capability
- **Production-Ready:** Optimized, tested, battle-hardened
- **Developer-Friendly:** Simple API, excellent documentation

#### Model Specifications Dashboard
- Show specs in a clean table or cards:
  - Parameter count
  - MoE expert count & routing
  - Context window size
  - Inference speed benchmarks
  - Accuracy metrics vs competitors

#### Benchmarks Section
- Visualize performance: charts comparing Kden vs similar models
- Metrics: MMLU, HellaSwag, TruthfulQA, HumanEval (text-only tasks)
- Interactive: Allow users to toggle benchmarks to focus on

#### Live API Demo (Optional but impressive)
- Text input box → Send query to Kden → Display response
- Shows real-world capability in <500ms (or gracefully explain delay)
- Or simulated with stunning pre-recorded examples

#### API Documentation Preview
- Quick start code snippet (Python, cURL, Node.js)
- Link to full docs
- Pricing/rate limit clarity

#### Call-to-Action Footer
- Sign up for beta / waitlist
- Join Discord/community
- Download research paper / model card

---

## Design System Details (from `ui-ux-pro-max`)

### Color Palette (Dark Mode Recommended)
- **Primary:** Electric blue or cyan (#06B6D4 or #0891B2 for Tailwind)
- **Accent:** Violet or electric purple (#A78BFA or #C084FC)
- **Background:** Deep slate (#0F172A or #1E293B)
- **Text:** Off-white (#F1F5F9)
- **Muted:** Slate-600 (#475569)

### Typography
- **Headlines:** Modern sans (Inter, Sora, Geist) + weight 700-800
- **Body:** Clean sans (Inter, Poppins, Geist) + weight 400-500
- **Code/Specs:** Monospace (JetBrains Mono, Fira Code, Courier Prime)

### Component Standards
- Buttons: Solid CTA, minimal secondary, code-style tertiary
- Cards: Use `backdrop-blur` + semi-transparent bg for glassmorphism feel
- Icons: Lucide React (24px, consistent stroke width)
- Spacing: 8px grid (Tailwind's default)
- Transitions: 200-300ms, ease-in-out

### Accessibility Checklist
- [ ] WCAG AA contrast minimum (4.5:1 for body text)
- [ ] Keyboard navigation fully functional
- [ ] Focus states visible
- [ ] `alt` text on all images
- [ ] Reduced motion respected (`prefers-reduced-motion`)

---

## Technical Stack Recommendation

**React + Tailwind CSS + Lucide Icons**

- Fast, responsive
- Tailwind's utility-first = pixel-perfect consistency
- Lucide icons = professional SVG library
- ESLint + Prettier for code quality

**Optional Enhancements:**
- Framer Motion for subtle micro-interactions (hero animations, scroll reveals)
- Chart.js or Recharts for benchmark visualization
- Markdown renderer (MDX) if embedding research/docs

---

## Deliverables

1. **`/.impeccable.md`** – Design context document
2. **`/src`** – React components
   - `Hero.jsx` – Landing hero
   - `Features.jsx` – Why Kden section
   - `Specs.jsx` – Model specifications
   - `Benchmarks.jsx` – Performance comparisons
   - `Demo.jsx` – Live or example API interaction
   - `CTA.jsx` – Call-to-action sections
3. **`/public`** – Assets (logos, favicons, og-images)
4. **`/styles`** – Global Tailwind config + design tokens
5. **README.md** – Setup & deployment instructions

---

## Success Criteria

✅ Design is **cohesive**: Every pixel reflects "efficient, powerful, trustworthy"
✅ Content **loads fast**: No unnecessary animations or bloated assets
✅ **Mobile-first** responsive: Works beautifully on 320px → 2560px
✅ **Accessibility**: WCAG AA compliant, keyboard navigable
✅ **Clear hierarchy**: User immediately understands what Kden is
✅ **Credibility signals**: Specs, benchmarks, and social proof visible above fold
✅ **Conversion-ready**: CTAs are prominent and clear (demo, API, docs, sign up)

---

## Pro Tips

1. **Performance is your hero:** Use Next.js Image optimization, code splitting, lazy loading
2. **Specs as proof:** Let the model specs speak—64M MoE is impressive on its own
3. **Trust with data:** Real benchmarks > marketing fluff. Be honest about trade-offs
4. **Mobile-first design:** Start mobile, then enhance for desktop
5. **One-page wonder:** Keep it focused—a long-scrolling page is perfect for showcasing depth
6. **Social proof:** If Kden is being used anywhere, feature it
7. **Call-to-action clarity:** "Try Kden," "View Benchmarks," "Get API Keys"—no ambiguity

---

Good luck cooking! 🔥