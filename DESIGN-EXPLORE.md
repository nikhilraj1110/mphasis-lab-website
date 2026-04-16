# Design Exploration Protocol

## Trigger
When the user points to this file and names a section on any webpage, execute the following workflow.

## Inspiration References
- **Global Research Footprint** (contact.html) — data arranged spatially with visual impact
- **Student Trajectories** (impact.html) — narrative data showcase with compelling flow
- The principle: data itself becomes the design. Arrangement, hierarchy, motion, and whitespace do the heavy lifting — not decoration.

## Design Philosophy
Think like Steve Jobs: obsess over every detail, strip away the unnecessary, make the complex feel simple, and create moments of delight. Every layout choice should feel inevitable — like there was no other way it could have been done.

**Critical directive from user:** "I want you to think of something a master designer and artist would take pride in. Someone like Steve Jobs would take pride in — now don't go ahead and copy any of his Apple ideas, I rather want you to take inspiration on what kind of impact and design inspiration I am looking for." This means: no generic grids, no safe layouts, no "arrange data neatly" thinking. Every concept must create an *experience* — a moment that makes the viewer feel something. Lead with emotion and story, not information architecture. If a concept could appear on any other website, it's not good enough.

## Workflow

### Step 1 — Study
- Read the section the user pointed to (HTML + CSS + JS + data)
- Understand the data structure, content type, and current presentation
- Identify what makes this data interesting and what story it tells

### Step 2 — Ideate
- Propose **5-6 radically different design concepts** for showcasing that section
- Each concept should have:
  - **Name** — a short, evocative title (e.g., "The Observatory", "Living Grid")
  - **Core Idea** — one sentence on the design philosophy
  - **Visual Description** — how it looks, feels, and moves
  - **Why It Works** — what makes this arrangement maximise viewer impact
  - **Inspired By** — real-world design reference (website, product, installation, etc.)
- Concepts should range from refined-minimal to bold-experimental
- No two concepts should feel similar — each must be a genuinely different approach

### Step 3 — User Selects
- Present all concepts to the user
- User picks which concepts they want built as mockups (could be 1, could be all)

### Step 4 — Build Mockups
- For each selected concept, build a **standalone HTML file** (e.g., `prototype-{concept-name}.html`)
- Place in the Website root: `/Users/raj/Desktop/projects/Work/Workspace/Website/`
- Each mockup must:
  - Be fully self-contained (inline CSS + JS, or reference existing site assets)
  - Use **real data** from the actual section (not placeholder/lorem ipsum)
  - Look **exactly** as it would appear on the final website (same fonts, colors, design tokens)
  - Be responsive (test at desktop + mobile widths)
  - Include all interactions, animations, and hover states described in the concept
  - Run independently on localhost for side-by-side comparison

### Step 5 — User Compares & Decides
- User tests all mockups on localhost
- User picks the final design (or requests a hybrid)
- Winning design gets integrated into the actual page

## Rules
- Never auto-start building without user selection (Step 3 approval required)
- Use real data only — no fabrication
- Each mockup is a complete, polished experience — not a wireframe or sketch
- Maintain the site's existing design system (tokens, fonts, pillar colors) as the foundation
- Push creative boundaries on layout, motion, and data arrangement — not on branding
