# Day 10 — Build Your Personal Portfolio Website

**Abtalks 60 Days Claude Challenge**
Date: 10 June 2026 · Difficulty: Intermediate · Time: ~60 mins

---

## What I Built

A complete, single-file personal portfolio website generated entirely using Claude — no manual coding required.

**File:** `naman_portfolio.html`
**Live URL:** [namanarora.online](https://namanarora.online)

The portfolio showcases my profile as a Full Stack Developer and AI Engineer, complete with real photo, project cards, experience timeline, achievements, and a contact section — all in one self-contained HTML file.

---

## The Prompt I Used

The task provided a structured portfolio prompt. I replaced every placeholder with my real information:

- Name, title, location, email, phone, LinkedIn, GitHub, portfolio URL
- Profile photo (uploaded directly to Claude)
- Full skills list across languages, frameworks, and tools
- 4 featured projects with tech stacks
- Internship experience at HCL Technologies and The Indian Express
- Achievements including SIH 2024 National Winner

Claude generated the entire HTML file in one shot.

---

## What the Portfolio Includes

| Section | Details |
|---------|---------|
| Hero | Name, animated typing titles (5 rotating), profile photo with gradient ring, stat counters, social links |
| About | Biography, skill badges, quick stat cards |
| Skills | Animated progress bars + colour-coded tech pills |
| Projects | 4 project cards — SIH winner card with special glow treatment |
| Experience | Vertical timeline — HCL Technologies & The Indian Express |
| Achievements | 6 achievement cards with accent borders |
| Contact | Clickable cards for email, phone, LinkedIn, portfolio |
| Footer | Social links + back to top |

**Premium features included:**
- Custom dot cursor with laggy ring (desktop)
- Scroll progress bar at top of page
- Loading screen animation
- Scroll-reveal on every section
- Glassmorphism cards with gradient borders
- Animated background grid
- Typing animation (5 rotating professional titles)
- Dark premium theme — orange (#F47C20) + cyan (#00D4FF) + mint (#00FFB3)

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Structure | HTML5 |
| Styling | Tailwind CSS (CDN) + custom CSS |
| Logic | Vanilla JavaScript |
| Fonts | Space Grotesk + JetBrains Mono (Google Fonts) |
| Hosting | GitHub Pages / Vercel compatible |
| Build step | None — single file, open in browser |

---

## How to Use This File

```bash
# Option 1 — Local
Open naman_portfolio.html in any browser

# Option 2 — Deploy on GitHub Pages
1. Push naman_portfolio.html to your repo
2. Go to Settings → Pages → Source: main branch
3. Your portfolio is live at username.github.io/repo/naman_portfolio.html

# Option 3 — Deploy on Vercel/Netlify
1. Drag and drop the HTML file
2. Get a live URL instantly
```

---

## Key Learnings

**1. Prompt quality = output quality**
The more structured and detailed your prompt, the better the output. Filling in every placeholder with real data (not generic examples) made the difference between a template and an actual personal brand.

**2. Claude handles design decisions**
By specifying color palette, font choices, and design style in the prompt, Claude made intentional design decisions — gradient borders, glassmorphism cards, custom cursor — that would take hours to implement manually.

**3. Personal branding insight**
A portfolio is not a resume. A resume lists what you did. A portfolio shows who you are. The SIH 2024 winner card having a distinct glow, the typing animation cycling through 5 different titles, the photo with a gradient ring — these are brand signals, not just information.

**4. Single file = maximum portability**
One HTML file with embedded photo (base64), embedded CSS, and embedded JS — no dependencies, no build step, no server needed. It opens in any browser, deploys anywhere, and shares as a single attachment.

**5. AI-generated ≠ generic**
When you feed Claude specific information — your actual projects, real tech stack, genuine achievements — the output feels personal. Generic prompts produce generic portfolios. Specific prompts produce specific ones.

---

## What I Would Improve Next

- Add a working contact form backend (Formspree or EmailJS)
- Add a projects filter by tech stack
- Add a blog section pulling from a markdown file
- Connect GitHub API to show real contribution activity
- Add a downloadable PDF resume button

---

## Files in This Folder

```
day10/
├── naman_portfolio.html    ← complete single-file portfolio
├── day10.md                ← this file
└── screenshots/            ← add your screenshots here
    ├── hero.png
    ├── projects.png
    └── mobile.png
```

---

## Prompt Template (reusable)

Use this for anyone wanting to build their own portfolio:

```
You are an expert full-stack web developer and personal branding designer.
Build a complete, modern, single-file personal portfolio website using
HTML, Tailwind CSS (CDN), and vanilla JavaScript.

=== PERSONAL INFO ===
Name: [Your Name]
Title: [Your Title]
Location: [City, Country]
Email: [email]
LinkedIn: [URL]
GitHub: [URL]
About: [2-3 sentences]

=== SKILLS ===
Technical: [list]
Tools: [list]
Soft Skills: [list]

=== PROJECTS ===
1. [Name] — [description] — Tech: [stack]
2. [Name] — [description] — Tech: [stack]

=== EXPERIENCE & ACHIEVEMENTS ===
- [list]

=== DESIGN PREFERENCES ===
Mode: Dark theme
Style: Modern, minimal, premium
Colors: Orange (#F47C20) + Cyan (#00D4FF)
Font: Space Grotesk

Return only the complete HTML code.
```

---

## Part of

**Abtalks 60 Days Claude Challenge**
Day 10 of 60 — building real, shareable things with Claude every day.

*@Anthropic @ABTalksOnAI @AnilBajpai*

---

*Generated using Claude · Abtalks 60 Days Challenge · Day 10*