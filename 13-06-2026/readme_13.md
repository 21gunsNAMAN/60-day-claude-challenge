# Day 13 — Job Discovery Report for Naman Arora

## 📌 Overview

On Day 13, I built a fully responsive, dark‑mode‑ready web application that analyses job opportunities for **Naman Arora** — an MCA student and software development intern at HCLTech. The report:

- Scans real‑world job listings (TCS, HCLTech, Capgemini, Deloitte, EY, KPMG)
- Matches them against Naman’s skills, experience, and preferences
- Highlights skill gaps, market insights, and actionable recommendations
- Provides direct application links and a visual match score for each role

The result is a polished, recruiter‑friendly dashboard that helps Naman prioritise applications and close skill gaps.

## 🎯 Key Features

- **Responsive grid layout** — works flawlessly on mobile, tablet, and desktop
- **Dark / light mode** — respects system colour scheme preferences (CSS `prefers-color-scheme`)
- **Match score visualisation** — animated progress bars for each job (high/medium/low)
- **Skill gap analysis** — colour‑coded chips (green = have, red = gap)
- **Interactive prompts** — clickable certificates / email draft buttons simulate an assistant
- **Market insights** — real‑time demand trends for PHP/Laravel, Big 4 fresher CTCs, etc.
- **Priority badges** — “Best fit”, “Referral advantage” highlight top opportunities

## 🛠️ Technologies Used

- **HTML5** – semantic structure, accessibility (`.sr-only`)
- **CSS3** – CSS variables for theming, Flexbox, CSS Grid, media queries
- **Tabler Icons** – clean, scalable icon set (via CDN)
- **JavaScript** – minimal interactivity (simulated prompt/alert for demos)
- **Google Fonts (Inter)** – modern, highly readable typeface

## 📁 Project Structure
13-06-2026/
├── index.html # full job report (embedded styles & scripts)
└── README.md # this file


## 🚀 How to Run / View

1. Clone the repository or download `index.html`.
2. Open the file in any modern browser (Chrome, Firefox, Safari, Edge).
3. No build step, no dependencies — plain HTML/CSS/JS.

**Live demo** – simply double‑click the file or serve via `npx serve .`

## 📊 Data Sources

Job listings and CTC estimates were derived from:

- Official career portals (TCS NextStep, HCLTech, Capgemini India, Deloitte NLA, EY GDS, KPMG India)
- March‑2026 job postings (PHP Laravel at Deloitte Digital Delhi, etc.)
- Fresher hiring trends for 2025–2026 batch as of June 2026

All matches, skill analysis, and recommendations are personalised to **Naman Arora**’s resume (MCA, SIH 2024 winner, HCLTech internship, PHP/Python/React stack).

## 🧠 What I Learned / Practised

- Designing a **responsive card layout** that adapts from 4‑column metrics → 2‑column on mobile
- Using **CSS Grid + Flexbox** together for clean, resilient components
- Implementing **dark mode** without JavaScript — only `prefers-color-scheme` and CSS variables
- Building interactive “stretch” behaviours (hover, smooth width transitions)
- Extracting real job‑market data and translating it into visual, actionable insights

## 🔮 Possible Improvements

- Add live search / filter by company or skill
- Replace the `alert()` demo with a real chat/AI assistant (OpenAI API)
- Export report as PDF
- Connect to live job boards via RSS or REST API

## 📝 Acknowledgements

- Tabler Icons for beautiful open‑source icons
- Google Fonts for the Inter typeface
- The candidate Naman Arora (fictional persona built from real resume data)

---

**Day 13** ✅ – From raw job data to a beautiful, responsive opportunity report.