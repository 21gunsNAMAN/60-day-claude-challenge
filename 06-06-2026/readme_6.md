```markdown
# Day 6 – ATS Resume Analyzer & Optimizer

**AB Talks – 30 Days of AI Tools**

Today I built an **ATS Resume Analyzer** – a complete single‑page web app that simulates an Applicant Tracking System (ATS) to score resumes against a given job description, identify keyword gaps, and provide actionable fixes. I also used an LLM (Claude) to rewrite my own resume for maximum ATS compatibility.

---

## 🧠 What is ATS?

ATS (Applicant Tracking System) software scans resumes before a human ever sees them. It checks for:
- Keyword alignment with the job description
- Proper section headings (Experience, Education, Skills)
- Clean formatting (no columns, tables, images)
- Quantifiable achievements

A low ATS score means your resume is likely filtered out – even if you’re a perfect fit.

---

## 🛠️ Project 1: ATS Resume Analyzer (Web App)

A full‑stack (front‑end only) analyzer that:
- Accepts your resume (paste text or upload .docx/.txt)
- Accepts a job description + optional tech stack / soft skills
- Calls **Claude API** (Anthropic) to generate a detailed ATS report
- Displays score, keyword matches/missing, formatting issues, and a step‑by‑step roadmap to 80+

### Features
- **Drag & drop** file upload (TXT, DOCX)
- **Manual text paste** for PDF fallback
- **Job type toggle** (technical / non‑technical / hybrid) – changes the analysis focus
- **Tag inputs** for required tech stack, nice‑to‑have, and soft skills
- **ATS score ring** with animated fill
- **Breakdown** of 8 sub‑scores (keyword match, formatting, experience relevance, etc.)
- **Keyword clouds** – found, missing, partial matches
- **Critical fixes** and **improvement suggestions** with concrete examples
- **Example bullet points** using missing keywords
- **Roadmap to 80+** – ordered steps to improve the score
- **Tailoring tips** specific to the role

### How It Works
1. User provides resume text and job details.
2. Front‑end builds a structured JSON prompt for Claude.
3. Claude returns a complete JSON object with scores, keywords, fixes, etc.
4. JavaScript renders the results with animated charts and cards.

### Tech Stack
- HTML5 / CSS3 (custom design system – dark theme, clean cards)
- Vanilla JavaScript (no frameworks)
- Claude API (Anthropic) – model `claude-sonnet-4-20250514`
- Mammoth.js – DOCX text extraction

### Setup & Run
> ⚠️ **API Key Required** – The app uses the Claude API. You must add your own key in the `fetch` call inside `runAnalysis()`.

```js
// Inside runAnalysis() – add your API key header
headers: {
  'Content-Type': 'application/json',
  'x-api-key': 'YOUR_ANTHROPIC_API_KEY'
}
```

Then simply open the HTML file in a browser. No build step.

---

## 📄 Project 2: My Own Resume Optimization

Before building the analyzer, I used Claude to rewrite **my resume** (Naman Arora) for ATS. The original resume had:
- Two‑column layout risk
- Inconsistent formatting
- Missing action verbs and quantified impact in some bullets

**Optimized version** (now single‑column, ATS‑friendly):
- Professional summary rewritten with keywords from my target roles (Full‑Stack / AI Engineer)
- Each bullet starts with a strong action verb + metric where truthful
- Clear section headings: `PROFESSIONAL SUMMARY`, `EXPERIENCE`, `EDUCATION`, `KEY PROJECTS`, `TECHNICAL SKILLS`, `CERTIFICATIONS & ACHIEVEMENTS`
- Removed graphics / icons – pure text for parsers

**Example change**  
*Before:* "Built a News Publishing CMS using PHP, MySQL, Bootstrap, Ajax"  
*After:* "Engineered a News Publishing CMS (PHP, MySQL, WordPress, Ajax) that reduced article publishing time by 30% for the digital editorial team."

> All metrics are truthful based on my actual internship experience (e.g., WhatsApp Cloud API integration, multi‑tenant system architecture).

---

## 📈 Key Learnings – Day 6

1. **ATS scoring is not magic** – it’s a function of keyword density, section clarity, and formatting. My analyzer mimics that logic via LLM reasoning.
2. **Prompt engineering is critical** – the JSON output must be strict; otherwise, the front‑end breaks. I iterated on the prompt to enforce exact keys and arrays.
3. **Real‑time animation** (score ring, progress bars) dramatically improves user perception of the analysis.
4. **PDF is still tricky** – client‑side PDF parsing without external libs is limited; I handled it by encouraging manual text paste for reliability.
5. **Resume rewriting requires truthfulness** – even with ATS, fabricating skills/metrics is unethical and backfires in interviews. I only added phrasing improvements, never invented data.

---

## 🔮 What’s Next (Day 7)

- Add a **“Download optimized resume”** feature (PDF generation from the rewritten text)
- Store past analyses in `localStorage` to track improvement over time
- Build a **free ATS score checker** without requiring an API key (rule‑based fallback)

---

## 📁 Files in This Day

| File | Description |
|------|-------------|
| `ats_resume_analyzer.html` | Complete single‑file web app (source code) |
| `Naman_Arora_ATS_Resume.pdf` | My original resume (used for testing) |
| `readme_6.md` | This file |

---

## 🧪 Try It Yourself

1. Open `ats_resume_analyzer.html` in a modern browser.
2. Paste your resume (or upload a `.docx`).
3. Fill in a real job description.
4. Click **Analyze Resume** – you’ll see your ATS score and a custom improvement plan.
5. Use the **“Keyword sentences”** and **“Roadmap to 80+”** to rewrite your resume.

> 💡 The tool is meant for learning and self‑improvement. Always double‑check LLM suggestions against your real experience.

---

**Day 6 complete.**  
Next: Build a resume parser that extracts structured data from any PDF/DOCX – without cloud APIs.

`— AB Talks`