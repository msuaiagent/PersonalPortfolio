# AI Club — Week 4

## Portfolio Design Selection + Modular Prompt Setup

---

## Goal of Week 4

By the end of this week, you will have completely prepared the specifications needed to generate your portfolio website in Week 5.

You are **not** building the website yet.

You are **not** designing the website from scratch.

You are selecting a portfolio design, locking in the important design variables, organizing your content, and preparing a modular prompt that AI can follow reliably when we begin code generation.

This week exists to remove ambiguity before code generation.

In Week 5, the AI should already know:

* which portfolio design you chose
* which sections the design includes
* which components must be built
* which fonts you selected
* which color palette you selected
* what content goes into each section

The goal is to make AI generation as smooth and predictable as possible.

---

## Why This Week Matters

When beginners ask AI to "make me a portfolio website," the model has to guess:

* layout
* sections
* component structure
* colors
* fonts
* content placement
* page hierarchy

That guessing leads to problems:

* inconsistent layouts
* random styling
* missing sections
* poor mobile responsiveness
* messy code structure
* harder debugging

This week fixes that.

Instead of asking AI to guess, we are going to give it a **clear blueprint**.

That is how you get better outputs.

---

## Important Rule for This Week

You are **building from the portfolio designs provided in the reference PDF**.

You are not inventing a design system from scratch.

You are not freely creating your own layout.

You are choosing a design and preparing it for implementation.

This is intentional.

Since this guided project is for students with **little to no coding experience**, we want to reduce as many unknown variables as possible before the AI starts generating code.

More freedom sounds nice, but too much freedom at this stage usually creates more bugs, more confusion, and more troubleshooting.

---

## Can You Choose Your Own Design?

Yes, but it is **not recommended** for most students.

You may choose your own portfolio inspiration instead of one of the provided portfolio designs. However, doing that means you are stepping outside the guided path of the project.

That can make the project harder because:

* you may run into bugs that were **not encountered by one of the project directors**
* your chosen design may be harder to translate into code
* troubleshooting becomes less predictable
* it may be harder for mentors to help you quickly
* the AI may generate code that does not align as cleanly with the guided workflow

Because this project is designed for people with **no experience coding**, the safest path is to use one of the provided portfolio designs from the PDF.

If you choose your own design, you are accepting a higher chance of running into issues that are outside the guided project flow.

---

## What You Are Allowed to Customize

You may customize:

* your chosen portfolio design
* your color palette
* your fonts
* your personal content
* your project information
* your links
* your images

You are **not** customizing:

* the entire layout structure from scratch
* the overall design system from scratch
* the section order without reason
* the framework
* the styling technology
* the component-based architecture

Those constraints are there to help you succeed.

---

## What You Will Complete This Week

By the end of Week 4, you must have completed all of the following:

1. Chosen one portfolio design
2. Identified the sections in that design
3. Identified the components needed to build that design
4. Chosen a color palette
5. Chosen a font pairing
6. Finalized your website content
7. Built your modular prompt for Week 5

If you skip this work, Week 5 becomes much harder.

---

## Step 1 — Choose One Portfolio Design

You must choose **one** portfolio design to use as the basis for your website.

Use the provided portfolio PDF as the default source of truth for your design direction.

Do not combine multiple designs together.

Do not try to merge several layouts into one.

Do not redesign the entire website from scratch.

Pick one design and commit to it.

### Design Selection Rules

You must:

* choose one design only
* keep the core layout structure of that design
* follow the section order shown in that design as closely as possible
* use that design as your blueprint in Week 5

You may:

* swap in your own colors
* swap in your own fonts
* replace placeholder text with your own content
* replace placeholder project cards with your own projects

### Required Deliverable

```text
CHOSEN_PORTFOLIO_DESIGN

Design Name or Number:
Using provided PDF design or custom design:
Why you chose it:
Main sections visible in the design:
Notes about anything important in the layout:
```

---

## Step 2 — Identify the Sections in Your Chosen Design

Now that you have selected a design, you need to identify exactly which sections appear in it.

Do not guess.

Look at the design and list the visible sections in order.

Examples of sections you may see in the portfolio references include:

* Navbar
* Hero
* About
* Services
* Skills
* Projects
* Testimonials
* Resume
* Work
* Contact
* Footer
* Blog

Your section list should come from the chosen design, not from imagination.

### Example

A selected design might contain:

```text
Navbar
Hero
About
Services
Projects
Testimonials
Contact
Footer
```

Another might contain:

```text
Navbar
Hero
About
Projects
Resume
Contact
Footer
```

### Required Deliverable

```text
SECTION_LIST

1.
2.
3.
4.
5.
6.
7.
```

Write the sections in the exact order they appear in your design.

---

## Step 3 — Identify the Components Needed to Build the Design

Now convert the design into components.

This is one of the most important steps of Week 4.

The AI should not have to guess what components to build.

If the design includes a hero, project grid, contact form, and footer, then your prompt should explicitly require those components.

### Base Component Rule

Every student should identify:

* section-level components
* reusable child components

### Example

If your design has:

* navbar
* hero
* projects
* testimonials
* contact form
* footer

Then your components might be:

```text
Navbar
HeroSection
ProjectsSection
ProjectCard
TestimonialsSection
TestimonialCard
ContactSection
ContactForm
Footer
```

### Required Deliverable

```text
COMPONENT_LIST

Section Components:
-
-
-
-

Reusable Child Components:
-
-
-
-
```

---

## Step 4 — Choose Your Color Palette

You are allowed to customize colors, but only within the structure of the chosen design.

Use:

[https://coolors.co/](https://coolors.co/)

Export your chosen palette as code or Tailwind values if possible.

### Required Color Roles

```text
Primary:
Secondary:
Accent:
Background:
Text:
```

Optional:

```text
Muted:
Card Background:
Border:
```

### Rules

* do not choose too many colors
* do not make the design visually chaotic
* keep the selected design recognizable even after swapping colors
* prioritize readability and contrast

### Required Deliverable

```text
COLOR_PALETTE

Primary:
Secondary:
Accent:
Background:
Text:
Muted:
Card Background:
Border:
```

---

## Step 5 — Choose Your Fonts

You are also allowed to customize typography.

Use:

[https://coolors.co/fonts](https://coolors.co/fonts)

Choose fonts that fit the portfolio design you selected.

### Required Font Roles

```text
Heading Font:
Body Font:
```

Optional:

```text
Accent Font:
```

### Rules

* keep it to 1 or 2 fonts
* choose web-friendly fonts
* do not choose extremely decorative body fonts
* prioritize readability

### Required Deliverable

```text
FONT_SYSTEM

Heading Font:
Body Font:
Accent Font:
```

---

## Step 6 — Finalize Your Website Content

Before code generation, your content must be ready.

Do not let AI invent your biography, projects, or links.

You need to prepare the content that will go into the chosen layout.

### Required Fields

```text
Full Name:
Professional Title:
Short Intro:
About Paragraph:
Skills:
Projects:
Contact Email:
GitHub URL:
LinkedIn URL:
Resume Link or File:
```

### Project Format

For each project, write:

```text
Project Name:
Description:
Tech Stack:
Link:
GitHub:
Image:
```

### Required Deliverable

```text
CONTENT_SPEC

Full Name:
Professional Title:
Short Intro:
About Paragraph:

Skills:
-
-
-

Projects:
1.
2.
3.

Contact Email:
GitHub:
LinkedIn:
Resume:
```

---

## Step 7 — Build the Design Mapping File

This is the file that connects your chosen design to your implementation plan.

Create a file called:

```text
design_mapping.md
```

This file should explain exactly how your chosen design will be translated into code.

### `design_mapping.md` Template

```md
# Design Mapping

## Chosen Portfolio Design
Design Name or Number:
Reference Source: Provided Portfolio PDF or Custom Design

## Section List
1.
2.
3.
4.
5.
6.
7.

## Component List
### Section Components
-
-
-

### Reusable Child Components
-
-
-

## Color Palette
Primary:
Secondary:
Accent:
Background:
Text:
Muted:
Card Background:
Border:

## Font System
Heading Font:
Body Font:
Accent Font:

## Content Notes
What content goes in each section:
```

---

## Step 8 — Build the Modular Prompt for Week 5

Now that your design choice is frozen, you can prepare the AI prompt.

This is the main output of Week 4.

The prompt must clearly tell AI:

* which portfolio design to follow
* which components to build
* which sections to include
* which colors to use
* which fonts to use
* which content to insert

### Base Prompt

```md
You are an expert frontend engineer.

Generate a portfolio website in Next.js using Tailwind CSS.

The website must follow the selected portfolio design chosen for this project.

Do not invent a new layout.
Do not add extra sections that are not in the chosen design.
Do not use placeholder lorem ipsum unless content is missing.
Build the website using reusable React components.
Make the site responsive and cleanly organized.

Project requirements:
- Framework: Next.js
- Styling: Tailwind CSS
- Component-based architecture
- Mobile responsive
- Beginner-readable code
```

### Inserted Variables

```md
## Chosen Portfolio Design
[Insert design name or number]

## Required Sections
1. [Insert]
2. [Insert]
3. [Insert]
4. [Insert]
5. [Insert]
6. [Insert]
7. [Insert]

## Required Components
Section Components:
- [Insert]
- [Insert]
- [Insert]

Reusable Child Components:
- [Insert]
- [Insert]
- [Insert]

## Color Palette
Primary: [Insert]
Secondary: [Insert]
Accent: [Insert]
Background: [Insert]
Text: [Insert]
Muted: [Insert]
Card Background: [Insert]
Border: [Insert]

## Fonts
Heading Font: [Insert]
Body Font: [Insert]
Accent Font: [Insert]

## Content
Full Name: [Insert]
Professional Title: [Insert]
Short Intro: [Insert]
About Paragraph: [Insert]

Projects:
1. [Insert]
2. [Insert]
3. [Insert]

Contact Email: [Insert]
GitHub: [Insert]
LinkedIn: [Insert]
Resume: [Insert]
```

### Output Constraints

```md
## Output Requirements

Generate:
1. The main page structure
2. Reusable React components
3. Tailwind styling
4. Responsive behavior
5. Clean file organization

Do not:
- create a different layout from the chosen design
- invent extra sections
- ignore the chosen fonts
- ignore the chosen colors
- collapse everything into one giant file unless asked
```

---

## Step 9 — Recommended Folder Structure

Create the following inside your project:

```text
week_4/
  design_mapping.md
  content.md
  prompt.md
  inspiration_notes.md
```

### File Purposes

#### `design_mapping.md`

Maps the selected portfolio design into sections and components.

#### `content.md`

Contains the actual personal content for the website.

#### `prompt.md`

Contains the final modular AI prompt for Week 5.

#### `inspiration_notes.md`

Contains notes about the chosen design and anything important about the layout.

---

## Step 10 — What You Should Not Do

Do not do any of the following:

* do not combine multiple portfolio designs
* do not redesign the site from scratch
* do not keep changing sections after Week 4
* do not leave colors undefined
* do not leave fonts undefined
* do not leave your content undefined
* do not ask AI to decide the layout for you

Week 4 exists so that Week 5 is controlled.

---

## Submission Checklist

```md
## Week 4 Checklist

- [ ] I chose one portfolio design
- [ ] I decided whether I am using a provided design or a custom design
- [ ] I listed the sections in my chosen design
- [ ] I listed the components required to build it
- [ ] I selected my color palette
- [ ] I selected my fonts
- [ ] I finalized my content
- [ ] I completed `design_mapping.md`
- [ ] I completed `prompt.md`
```

---

## Final Reminder

You are not designing a portfolio from scratch. You are selecting a design and preparing it for reliable AI implementation.
The more disciplined you are in Week 4, the smoother Week 5 will be.
