# Day 11 — ATS Resume Optimizer & Resume Generator

**Course:** Career Applications with Claude  
**Date:** June 11, 2026  
**Difficulty:** Beginner  
**Deliverable:** ATS analysis + optimized resume + key learnings

---

## What I Built

An AI-powered ATS Resume Optimizer using Claude. The tool takes an existing resume and a target job description, then produces:

- An **ATS Match Score** across four dimensions
- A **Gap Analysis** identifying missing keywords, skills, and improvement areas
- A fully **rewritten ATS-optimized resume** using only factual information from the original
- **Recruiter Feedback** with an interview readiness score

I also built an interactive artifact (Claude-in-Claude) with a two-panel input UI, score cards, and tabbed output sections for gap analysis, optimized resume, and recruiter feedback.

---

## ATS Match Score

> Resume analyzed: **Naman Arora** — Full Stack / Backend Web Developer profile

| Metric | Score |
|---|---|
| **Overall ATS Score** | 78% |
| **Keyword Match Score** | 82% |
| **Technical Skills Match** | 85% |
| **Experience Relevance** | 72% |

---

## Gap Analysis

### Missing Keywords (common in target JDs)
- REST API, Agile, Version Control, CI/CD
- Unit Testing, MVC Architecture, Docker
- Linux/Ubuntu, OOP, Debugging

### Missing Skills
- Docker / containerization
- Cloud platforms (AWS, GCP, or Azure)
- Automated testing frameworks
- TypeScript

### Improvement Opportunities

| Area | Issue | Fix Applied |
|---|---|---|
| Bullet points | No measurable metrics anywhere | Rewrote with context and scope |
| Project descriptions | Too vague in original | Added tech stack, architecture, business value |
| Soft skills section | Listed AI tool names as soft skills | Removed; replaced with relevant tech context |
| Contact info | No GitHub link on original resume | Added GitHub to header |
| Typo | "Currently persuing" | Corrected to "Currently Pursuing" |
| Summary | Generic, not role-targeted | Rewritten with specific tech and achievements |

---

## Updated ATS-Optimized Resume

> Full resume generated as a `.docx` file ready for Word, Google Docs, FlowCV, Overleaf, and Canva.  
> File: `Naman_Arora_ATS_Resume.docx`

### NAMAN ARORA
+91 9560758246 | namanaurora01@gmail.com | [LinkedIn](https://www.linkedin.com/in/naman-arora-6921a7229/) | [GitHub](https://github.com/21gunsNAMAN) | [namanarora.online](https://namanarora.online)

---

### Professional Summary

Full Stack Web Developer with hands-on industry experience at HCLTech and Indian Express, specializing in PHP (Laravel, CodeIgniter), Python, MySQL, REST API integration, and backend system architecture. Built a scalable multi-tenant WhatsApp communication platform at HCLTech and a news publishing CMS at Indian Express. SIH 2024 National Hackathon Winner with demonstrated experience in AI/ML (YOLOv9s, CNN, LSTM, Django). Pursuing MCA at IMS Noida with a strong portfolio of freelance and personal projects spanning e-commerce, content management, and real-time systems.

---

### Technical Skills

| Category | Technologies |
|---|---|
| Programming Languages | PHP, Python, JavaScript, C/C++, HTML5, CSS3 |
| Frameworks & Libraries | Laravel, CodeIgniter 3, React.js, Node.js, Bootstrap, jQuery, Ajax |
| Databases | MySQL, MongoDB |
| Cloud & DevOps | cPanel Hosting, Netlify, Git, GitHub |
| AI/ML & Data | YOLOv9s, CNN, RNN, LSTM, Django (AI pipelines), Python AI scripting |
| APIs & Integrations | WhatsApp Cloud API (Meta), REST APIs, Third-party API integration |
| CMS & Platforms | WordPress, Custom PHP CMS |
| Tools | VS Code, ChatGPT, Deepseek, Perplexity, Lovable |

---

### Experience

**Software Development Intern** | HCLTech Pvt. Ltd. | Jan 2026 – Mar 2026
- Architected and deployed a scalable multi-tenant communication system using PHP (Laravel) integrated with the WhatsApp Cloud API (Meta Developers).
- Engineered custom message template management, bulk messaging workflows, and automated client communication pipelines serving multiple tenants from a single platform.
- Designed tenant-isolated data structures ensuring secure, independent communication channels per client.
- Collaborated with the engineering team on backend API design and system testing across edge-case scenarios.

**PHP Development Intern** | Indian Express Pvt. Ltd. | Jul 2023 – Sep 2023
- Developed a full-featured News Publishing CMS using PHP, MySQL, Bootstrap, Ajax, and WordPress for the digital editorial team.
- Implemented dynamic content management features including article creation, editing, category management, and user role controls.
- Integrated Ajax-driven interactions for seamless real-time content updates without page reload.

**Web Development Intern** | Webdesys | Jul 2023 – Sep 2023
- Designed and delivered multiple client websites from scratch and customized existing templates to match brand requirements.
- Collaborated directly with clients to gather requirements, iterate on designs, and deliver production-ready websites.

---

### Projects

**WhatsApp Multi-Tenant Communication System** — HCLTech  
`PHP` `Laravel` `WhatsApp Cloud API` `MySQL` `REST API`
- Built at HCLTech; supports custom message templates, bulk messaging, and fully automated client communication workflows across isolated tenants.
- Architected multi-tenant data isolation ensuring zero cross-tenant data leakage with role-based access.

**AI-Powered Fridge Detection System** — SIH 2024 National Winner  
`Python` `Django` `YOLOv9s` `CNN` `RNN` `LSTM` `Voice Assistant`
- National SIH 2024 winning project; integrated YOLOv9s object detection, deep learning models, a voice assistant, and a Django backend for high-accuracy, secure fridge inventory detection.

**News Publishing CMS** — Indian Express  
`PHP` `MySQL` `Bootstrap` `Ajax` `WordPress`
- Full editorial CMS with role-based access, content workflow management, and AJAX-driven real-time updates.

**United Nutritions** — E-Commerce Platform  
`PHP` `MySQL` `HTML/CSS` `JavaScript`
- Online retail platform for supplements with product catalogue, cart, and order management.

**News Page App**  
`React.js` `REST API`
- React.js news aggregator consuming a third-party API with dynamic filtering and responsive UI.

**Other Projects:** Law Hiring Website, Robust Solutions Wire Testing Platform, Cafe Management System, Car Details CMS, AI Assistant (Python), Encryption/Decryption Tool, To-Do List (React.js), JIMS Cynet 2024 Event Website

---

### Education

| Degree | Institution | Year |
|---|---|---|
| MCA (Currently Pursuing) | Institute of Management Studies, Noida Sec 62 | 2024 – 2026 |
| BCA | Jagannath Institute of Management Science, Vasant Kunj | Jan 2024 |
| Class 12th — IT (92% GPA) | St. Columba's School, New Delhi | Dec 2021 |
| Class 10th | St. Columba's School, New Delhi | May 2018 |

---

### Certifications

- Arena Animations — GWDD (Graphic Web Design & Development)
- SIH 2024 Winner Certificate — Smart India Hackathon, National Level
- JIMS Cynet 2023 — Winner, Website Development Competition
- JIMS Cynet 2024 — President, Event Coordination

---

### Achievements

- **SIH 2024 National Winner** — Led IMS Noida team to victory in Smart India Hackathon 2024 with an AI-powered fridge detection system using YOLOv9s, CNN, LSTM, RNN, and Django.
- **JIMS Cynet 2023 Website Winner** — Recognized for best website project at the intercollegiate tech fest.
- **JIMS Cynet 2024 Event President** — Appointed to lead and coordinate the flagship technology event.
- **Class 12 IT — 92% GPA** — Strong academic foundation in technology at St. Columba's School.

---

## Recruiter Feedback

### What recruiters will like
- SIH 2024 national hackathon win is a **strong differentiator** — most freshers don't have this
- Real internships at recognized companies (HCLTech, Indian Express) add immediate credibility
- The WhatsApp multi-tenant system demonstrates production-level backend architecture thinking
- Diverse project portfolio covering AI/ML, CMS, e-commerce, and real-time systems shows range

### What may still hurt interview chances
- **No quantified metrics** anywhere — no user counts, request volumes, or performance numbers
- **MCA still in progress** — no degree in hand yet for roles requiring a completed degree
- **No GitHub activity** mentioned — recruiters often check repos directly
- **Cloud gap** — most backend/full-stack JDs now expect at least basic AWS or GCP exposure

### Recommended improvements outside the resume
1. Pin the WhatsApp system and AI fridge project to GitHub with a good README and screenshots
2. Add a Projects section to namanarora.online with live demos and tech stack badges
3. Earn one free cloud certification (AWS Cloud Practitioner or GCP Associate) — fills the biggest gap
4. Contribute to one open-source PHP or Python project for GitHub activity signal
5. Add rough metrics wherever possible (even estimates: "system used by 3 client organizations")

### Interview Readiness Score: **71 / 100**
Strong story and real internship pedigree. Needs quantified impact, cloud exposure, and visible GitHub activity to compete at higher levels.

---

## Key Learnings

1. **ATS systems filter before humans see your resume** — keyword alignment is not optional, it's the entry gate.
2. **Factual accuracy is non-negotiable** — the optimizer rewrites and reorganizes but never invents. Invented metrics backfire in interviews.
3. **Bullet point quality matters more than quantity** — achievement-focused, specific bullets outperform long lists of responsibilities.
4. **Gap analysis is as valuable as the resume itself** — knowing what's missing gives a clear action plan for upskilling.
5. **Structure signals professionalism** — consistent heading hierarchy, clean skill categorization, and a strong summary dramatically improve ATS parsing and recruiter first impressions.
6. **One resume does not fit all roles** — ideally, tailor the keyword section and summary for each specific JD.
7. **A hackathon win like SIH 2024 deserves prominent placement** — it's a recruiter magnet that most candidates don't have.

---

## Tools Used

- **Claude (claude.ai)** — ATS analysis, gap analysis, resume rewriting, recruiter feedback
- **Claude Artifacts** — Built an interactive ATS optimizer UI (Claude-in-Claude)
- **docx npm library** — Programmatic generation of the `.docx` resume file
- **Prompt Engineering** — Structured system prompt with strict accuracy rules and output format

---

*Day 11 of #CareerApplicationsWithClaude*