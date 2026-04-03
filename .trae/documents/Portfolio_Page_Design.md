# Page Design Document — Web Developer Portfolio (Desktop-first)

## Global Styles (All Pages)
- Layout approach: Bootstrap container/grid for primary layout + Tailwind utilities for fine-tuning spacing/typography.
- Spacing: 8px baseline; section vertical padding ~64–96px desktop, ~40–64px mobile.
- Typography: system font stack (or one Google Font). Scale example: H1 48–56px, H2 32–36px, body 16–18px.
- Color tokens (example placeholders):
  - Background: #0B1220 (dark) or #FFFFFF (light)
  - Surface/card: #111A2E / #F8FAFC
  - Primary/accent: #3B82F6
  - Text: #E5E7EB / #0F172A
- Buttons/links:
  - Primary button: solid accent, hover darken + subtle shadow
  - Secondary button: outline, hover filled
  - Links: underlined on hover; external link icon optional
- Imagery: project thumbnails use consistent aspect ratio (e.g., 16:9). Use placeholders: “/assets/project-1.png”.
- Responsiveness (desktop-first):
  - Desktop (≥992px): multi-column grids, sticky top nav
  - Tablet (≥768px): reduce columns (e.g., 2)
  - Mobile: stacked layout, larger tap targets

---

## Page: Home (index.html)

### Meta Information
- Title: “{Your Name} | Web Developer Portfolio”
- Description: “Portfolio of {Your Name}: projects, skills, experience, and contact.”
- Open Graph:
  - og:title: same as title
  - og:description: same as description
  - og:image: “/assets/og-cover.png” (placeholder)

### Page Structure
- Overall pattern: stacked sections with anchored navigation.
- Main container: `container` + section blocks; max width ~1140–1320px.

### Sections & Components
1. Header / Navigation (sticky)
   - Left: logo/name text (“{Your Name}”) linking to top.
   - Right: anchor links: About, Skills, Projects, Experience, Contact.
   - Mobile: collapse menu (Bootstrap navbar) or simple stacked links.

2. Hero Section
   - Left column: 
     - H1: “Hi, I’m {Your Name}.”
     - Subtitle: “{Role: Frontend/Full‑Stack Developer}”
     - 2–3 line summary placeholder.
     - CTAs:
       - Primary: “View Projects” (scroll to projects)
       - Secondary: “Download Resume” (link to “/assets/resume.pdf” placeholder)
       - Tertiary: “Email Me” (mailto)
   - Right column:
     - Profile photo placeholder (circle) or illustration.

3. About Section
   - Two-column layout:
     - Bio paragraph placeholders
     - Quick facts list: “Location”, “Availability”, “Focus areas”

4. Skills Section
   - Grid of skill groups (cards):
     - Frontend: “HTML, CSS, JavaScript, …”
     - Styling: “Bootstrap, Tailwind, …”
     - Tools: “Git, Figma, …”
   - Use badges/chips for individual skills.

5. Featured Projects Section
   - Card grid (3 columns desktop, 2 tablet, 1 mobile).
   - Each card includes:
     - Thumbnail placeholder
     - Title (“Project Name”)
     - 1–2 sentence description placeholder
     - Stack tags (badges)
     - Links: “Details” (to project page), “GitHub”, “Live Demo” (placeholders)

6. Experience / Education Section
   - Timeline-style list:
     - Item: “{Role} — {Company}”, dates, 2–4 impact bullets placeholders.

7. Contact Section
   - Left: contact card
     - Email: “you@example.com”
     - LinkedIn/GitHub links placeholders
   - Right: message form UI (static placeholder)
     - Fields: Name, Email, Message
     - Submit button shows helper text: “This form is a UI placeholder (no backend).”

8. Footer
   - Copyright
   - Small links: GitHub, LinkedIn

---

## Page: Project Details (/project-<slug>.html)

### Meta Information
- Title: “{Project Name} | {Your Name}”
- Description: “Case study for {Project Name}: goals, build, and outcomes.”
- Open Graph: title/description/image per project

### Page Structure
- Top: compact header with “Back to Home/Projects”.
- Body: hero + gallery + case study + links.

### Sections & Components
1. Project Hero
   - Title: “{Project Name}”
   - Short pitch: 1–2 lines placeholder
   - Link buttons: “Live Demo”, “GitHub Repo” (placeholders)
   - Quick facts row: role, timeline, stack.

2. Media Gallery
   - Large main image + 2 smaller thumbnails (or simple carousel using Bootstrap).
   - All images are placeholders with captions.

3. Case Study Content
   - Headings with placeholder copy:
     - “Problem”
     - “Solution”
     - “Key Features” (bullets)
     - “Challenges & Learnings”

4. Tech Stack
   - Badge list + short notes on what you used and why.

5. Navigation
   - Buttons: “Previous Project”, “Next Project”, “Back to Projects”.
