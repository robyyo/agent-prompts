# Distinctive Frontend Design

**Category:** Design / Frontend UI/UX  
**Purpose:** Generate frontend designs that are visually distinctive, context-specific, and avoid the "AI slop" aesthetic — generic layouts, purple gradients, and overused font families.  
**Works best with:** Claude 3.5+, GPT-4o, Cursor AI

---

## Variables

| Variable | Description | Example |
|---|---|---|
| `{{ client_name }}` | Client or project name | "Apex Fitness Studio" |
| `{{ industry }}` | Client's industry | "health & wellness" |
| `{{ brand_adjectives }}` | 3–5 words describing the brand feeling | "bold, energetic, no-nonsense, industrial" |
| `{{ target_audience }}` | Who will use this UI | "serious athletes aged 25–45" |
| `{{ page_or_component }}` | What you're building | "landing page hero section" |
| `{{ tech_stack }}` | Framework/environment | "React with Tailwind CSS" |
| `{{ color_hint }}` | Any brand colors to anchor from (optional) | "#FF3B00 orange, dark charcoal" |
| `{{ theme_preference }}` | Light, dark, or auto | "dark" |
| `{{ reference_aesthetic }}` | Cultural/design reference to draw from (optional) | "brutalist editorial, like a sports magazine from the 90s" |
| `{{ must_avoid }}` | Specific things to explicitly exclude | "rounded corners, soft pastels, Inter font" |

---

## The Prompt

```
You are building a frontend {{ page_or_component }} for {{ client_name }}, a {{ industry }} brand.

**Client context:**
- Brand feeling: {{ brand_adjectives }}
- Target audience: {{ target_audience }}
- Tech stack: {{ tech_stack }}
- Theme: {{ theme_preference }}
- Anchor colors: {{ color_hint }} (if provided)
- Reference aesthetic: {{ reference_aesthetic }} (if provided)

**Design directive — read this carefully before writing a single line of CSS:**

Your goal is a frontend that feels like a human designer with a strong point of view built it specifically for this client — not a template, not a starter kit, not what most AI would generate.

### Typography
- Choose fonts that are distinctive and earned — ones that communicate the brand's specific personality
- Select from Google Fonts or Adobe Fonts based on the brief
- Avoid: Inter, Roboto, Open Sans, Poppins, DM Sans, Plus Jakarta Sans, or any "safe" neutral sans-serif
- Consider: display serifs, condensed grotesques, slab serifs, humanist faces, historical revivals
- Use typographic scale aggressively — size contrast (e.g., 14px vs 96px) creates visual tension and interest
- Font pairing should feel intentional, not default

### Color & Theme
- Commit to a dominant color story, not a balanced palette
- Use CSS custom properties (`--color-primary`, etc.) for all color values
- Think: 1 dominant color (60%), 1 sharp accent (10–15%), neutrals for the rest
- Avoid: purple/violet gradients, teal + white, coral on white, "startup pastels"
- Draw inspiration from: industrial design, editorial print, retro tech, film posters, regional aesthetics
- For {{ theme_preference }} themes, make darkness or lightness feel intentional, not default

### Motion & Animation
- For CSS/HTML: use `animation-delay` for staggered reveals on page load — one orchestrated entrance is better than scattered micro-animations
- For React: use the Motion library (Framer Motion) for meaningful transitions
- Prioritize: page load sequence, hover states on interactive elements, state change transitions
- Avoid: animations that serve no purpose, generic fade-ins on everything, bounce keyframes

### Backgrounds & Atmosphere
- Never use a plain `background-color: white` or `background-color: #111` as the final answer
- Layer: gradients, noise textures, geometric SVG patterns, or contextual imagery as appropriate
- The background should reinforce the brand feeling — not be an afterthought

### Layout
- Break the grid intentionally at least once — an offset element, a bleed, an asymmetric section
- Negative space is not emptiness — use it as a design element
- Avoid: equal padding on all sides, centered everything, card grids as the default layout

### Anti-generic checklist — verify before submitting:
- [ ] No Inter, Roboto, Arial, or system-ui as primary typeface
- [ ] No purple gradient on white background
- [ ] No generic card grid layout as default hero
- [ ] No "hero image left + text right" cliché without a strong reason
- [ ] Colors feel specific to {{ client_name }}, not a random brand
- [ ] Would a designer look at this and say "that's interesting"?

**Must avoid for this project:** {{ must_avoid }}

Now build the {{ page_or_component }}. Output complete, production-ready code. Use CSS custom properties. If React, use Framer Motion for key transitions. Think like a designer who has a strong aesthetic opinion about {{ industry }} — then execute it.
```

---

## Usage Notes

- **Start with `brand_adjectives`** — these are the creative brief. Spend 30 seconds picking words that actually mean something specific, not "modern, clean, professional."
- **`reference_aesthetic`** is the highest-leverage variable. "Like a Wim Wenders film" gives more creative direction than any color code.
- If the first output is still generic, add: *"Your last output still used [specific thing]. Try again using a completely different typographic approach — something you've never generated before."*
- For React projects, always specify Framer Motion in `{{ tech_stack }}` to unlock animation directives.
- Combine with a branding prompt first to establish the `color_hint` and `brand_adjectives` before running this one.

---

## Example Fills

**Fitness Studio:**
```
client_name: Apex Fitness
industry: strength training gym
brand_adjectives: raw, industrial, uncompromising, no-frills intensity
target_audience: competitive athletes 22–40
page_or_component: gym membership landing page
tech_stack: HTML, CSS, vanilla JS
color_hint: near-black (#0A0A0A), blood orange (#FF3B00)
theme_preference: dark
reference_aesthetic: 1970s Italian motorsport poster meets underground fight gym
must_avoid: rounded cards, gradients, hero stock photos of smiling gym-goers
```

**Law Firm:**
```
client_name: Hargrove & Mays LLP
industry: corporate litigation
brand_adjectives: authoritative, precise, old-money confidence, quiet intimidation
target_audience: C-suite executives and GCs
page_or_component: homepage
tech_stack: React, Tailwind CSS
color_hint: deep navy, warm ivory, gold accent
theme_preference: light
reference_aesthetic: Economist magazine layout crossed with a Goldman Sachs annual report
must_avoid: blue gradients, stock photos of gavels, generic legal iconography
```
