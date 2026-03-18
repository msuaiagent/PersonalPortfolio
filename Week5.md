````md
# AI Club — Week 5

## One-Shot Portfolio Implementation (v0.dev)

---

## Goal of Week 5

By the end of this week, you will generate and assemble a **fully working personal portfolio website** using:

- a selected approved portfolio design (from Week 4)
- your structured resume JSON
- your design specifications (colors, fonts, layout notes)
- AI-assisted code generation using v0.dev

You are now moving from **planning → implementation**.

If Week 4 was done correctly, Week 5 should feel structured, predictable, and smooth.

---

## Core Philosophy

You are **not designing a website**.

You are **implementing an existing design** using:

- a fixed layout (from the approved design)
- real content (from your resume JSON)
- controlled styling (from your design spec)

This is not a creativity exercise.

This is an **accuracy + implementation exercise**.

---

## Tools You Will Use

### Primary Tool

- **v0.dev (Vercel AI UI Generator)**

You will use v0 to generate React components using your structured prompt.

---

## Required Inputs

Before starting Week 5, you must have:

- your **chosen portfolio design (from Week 4)**
- your **resume JSON**
- your **color palette**
- your **font system**
- your **design_mapping.md**
- your **prompt.md**

If any of these are incomplete, stop and fix Week 4.

---

## Week 5 Workflow

You will follow this exact process:

1. Open v0.dev
2. Upload your selected portfolio design image or PDF
3. Paste your **Week 5 master prompt**
4. Insert:
   - your resume JSON
   - your color palette
   - your fonts
   - your section order
5. Generate your portfolio website
6. Copy the generated code into your Next.js project
7. Run and test locally
8. Fix any small issues (spacing, responsiveness, imports)

---

## Critical Rule

You must use **one of the 5 approved portfolio designs**.

Do not:
- mix multiple designs
- redesign the layout
- improvise new sections
- invent your own structure

The goal is **consistency across all students**.

---

## Implementation Strategy

### Do NOT do this

```text
Generate my entire portfolio website from scratch.
````

This will produce:

* messy layouts
* inconsistent spacing
* extra sections
* hard-to-debug code

---

### DO THIS

You will use a **controlled one-shot prompt** that:

* locks the layout
* locks the sections
* locks the styling
* locks the content mapping

---

## Master Prompt (Use This)

Paste the following into v0.dev and fill in all placeholders.

---

### One-Shot Personal Portfolio — Generation Prompt

````md
You are an expert frontend engineer and UI implementation specialist.

Your job is to generate a complete, working personal portfolio website in Next.js and Tailwind CSS.

---

## PRIMARY IMPLEMENTATION OBJECTIVE

Use the uploaded approved portfolio design as the structural and visual blueprint.
Use the resume JSON as the content source.
Use the design specification as the styling constraint layer.

This is not a creative generation task.
This is a faithful implementation task.

---

## APPROVED DESIGN RULE

The reference image/PDF will be one of the 5 approved portfolio designs.

You must implement it exactly.

Do not:
- mix designs
- redesign layout
- introduce new patterns

---

## SELECTED DESIGN

Approved Design Number: [1–5]  
Design Name: [INSERT]

---

## SOURCE OF TRUTH PRIORITY

1. Reference design image/PDF  
2. Design specifications  
3. Resume JSON  
4. Minimal implementation judgment  

---

## REQUIRED SECTION ORDER

1. [INSERT]
2. [INSERT]
3. [INSERT]
4. [INSERT]
5. [INSERT]
6. [INSERT]
7. [INSERT]

Do not add, remove, or reorder sections.

---

## LAYOUT EXTRACTION STEP

Before writing code:

- determine layout for each section
- identify columns, grids, cards, and alignment
- determine spacing patterns
- detect repeated UI patterns

Use this as your blueprint.

---

## GLOBAL LAYOUT RULES

- Container: `max-w-6xl mx-auto px-6`
- Section spacing: `py-16` (desktop), `py-12` (mobile)
- Section gap: `space-y-8`
- Card padding: `p-6`
- Grid gap: `gap-6`

---

## VISUAL STRICTNESS RULES

Do not add:
- gradients (unless present)
- animations
- shadows (unless present)
- glassmorphism
- decorative effects

---

## COMPONENT STRICTNESS

Only use:

- Navbar
- HeroSection
- AboutSection
- SkillsSection
- ProjectsSection
- ExperienceSection
- ContactSection
- Footer

UI components:
- SectionHeading
- ProjectCard
- SkillBadge
- ExperienceCard
- SocialLink
- Button

Do not create extra components.

---

## RESUME JSON

```json
[PASTE RESUME JSON HERE]
````

Use JSON for ALL content. Do not invent content.

---

## MISSING DATA RULE

If data is missing:

* do not fabricate
* omit or use minimal placeholder

---

## DESIGN SPECIFICATIONS

### Colors

Primary:
Secondary:
Accent:
Background:
Text:
Muted:
Card Background:
Border:

### Fonts

Heading:
Body:
Accent:

---

## TECH STACK

* Next.js (App Router)
* Tailwind CSS

---

## IMPLEMENTATION RULES

* semantic HTML
* responsive layout
* clean component structure
* no inline styles
* no placeholder comments

---

## OUTPUT FORMAT

Generate:

1. lib/resume.ts
2. app/page.tsx
3. all section components
4. UI components

Each file must be complete.

---

## FINAL CHECK

* layout matches reference
* sections match exactly
* content comes from JSON
* colors/fonts applied
* no extra features added

Generate the full implementation now.

````

---

## Folder Structure (Final)

Your project should look like:

```text
app/
  page.tsx

components/
  Navbar.tsx
  HeroSection.tsx
  AboutSection.tsx
  SkillsSection.tsx
  ProjectsSection.tsx
  ExperienceSection.tsx
  ContactSection.tsx
  Footer.tsx
  ui/
    SectionHeading.tsx
    ProjectCard.tsx
    SkillBadge.tsx
    ExperienceCard.tsx
    SocialLink.tsx
    Button.tsx

lib/
  resume.ts
````

---

## Common Mistakes to Avoid

* ❌ generating everything without constraints
* ❌ adding extra sections
* ❌ ignoring the chosen design
* ❌ inventing fake content
* ❌ inconsistent spacing
* ❌ using too many styles
* ❌ not following component structure

---

## Submission Checklist

```md
## Week 5 Checklist

- [ ] Used one approved design
- [ ] Uploaded design to v0
- [ ] Used master prompt
- [ ] Inserted resume JSON
- [ ] Inserted colors and fonts
- [ ] Generated full site
- [ ] Copied code into project
- [ ] Site runs locally
- [ ] Layout matches design
```

---

## Final Reminder

If Week 4 was done correctly, Week 5 should feel:

* structured
* predictable
* controlled

Your goal is not creativity.

Your goal is:

> **accurate implementation of a real design using real data**

That is how real engineers build.

```
```
