# Day 14 — AI Job Red Flag Detector

**Abtalks 60 Days Claude Challenge**
Date: 14 June 2026 · Difficulty: Beginner · Time: ~30 mins

---

## What I Built

A structured prompt-based tool that turns Claude into an AI Risk Analyst for job seekers — analyzing any job description and company information to surface hidden red flags before you invest time applying.

**Deliverable:** Risk analysis report generated from a real-world JD using the Red Flag Detector prompt.

---

## The Problem This Solves

Most job seekers read JDs hoping to qualify. Almost nobody reads them looking for warning signs. But the signals are always there:

- "Wear many hats" → you'll be underpaid for 3 people's work
- "Fast-paced startup environment" → no processes, constant firefighting
- No salary range → they want to lowball after you're already invested
- 8 years experience for a mid-level role → they're fishing for a senior at junior pay
- "Remote-friendly" → actually in-office 3 days a week

Claude, given the right prompt, catches all of this in 30 seconds.

---

## The Prompt

```
You are an AI Red Flag Detector for job seekers.
Analyze the Job Description and Company Information.

Identify:
1. Unrealistic Requirements
   - Excessive experience for the role
   - Too many skills/responsibilities
   - Contradictory expectations

2. Toxic Workplace Signals
   - Burnout indicators
   - 'Wear many hats', 'Fast-paced', 'rockstar', 'hustle culture'
   - Poor work-life balance signals

3. Remote Job Authenticity
   - Hidden office requirements
   - Relocation expectations
   - Misleading remote claims

4. Hiring Risks
   - Missing salary information
   - Vague responsibilities
   - Excessive qualifications
   - Suspicious hiring practices

5. Company Risks
   - Reputation concerns
   - Stability concerns
   - Growth or layoff indicators

Output:

## Overall Risk Score (0-100)

### Top Red Flags
- List with severity (1-10)

### Positive Signals
- List positives

### Risk Breakdown
| Category     | Risk Level |
|--------------|------------|
| Requirements |            |
| Culture      |            |
| Remote       |            |
| Hiring       |            |
| Company      |            |

### Final Verdict
✅ Apply
⚠️ Apply with Caution
❌ Avoid

### 5 Smart Interview Questions
Generate questions that help validate the identified risks.

Job Description:
[Paste Here]

Company Information:
[Paste Here]
```

---

## Sample Analysis — AI Engineer Role

### Input Used

**JD Excerpt (synthesized for demo):**
> We are looking for a passionate AI Engineer who can wear many hats in our fast-paced startup environment. You'll own end-to-end ML pipelines, manage cloud infrastructure, build internal tools, and support the product team. Must have 5+ years of experience with Python, TensorFlow, PyTorch, AWS, GCP, Docker, Kubernetes, and MLOps. Competitive salary. Fully remote.

**Company Info:**
> Early-stage B2B SaaS startup, 18 months old, 12 employees, Series A not yet closed. Glassdoor: 3.1/5 (3 reviews). LinkedIn: High employee turnover in last 6 months.

---

### Claude's Output

---

## Overall Risk Score: 72 / 100 ⚠️ High Risk

---

### Top Red Flags

| Flag | Severity |
|------|----------|
| "Wear many hats" — classic overload signal | 8/10 |
| "Fast-paced startup" — burnout culture indicator | 7/10 |
| 5+ years for what reads as a mid-level scope | 8/10 |
| No salary figure — only "competitive" (vague) | 7/10 |
| 8 tech stack requirements — unrealistic breadth | 9/10 |
| Series A not closed — financial runway unclear | 8/10 |
| Glassdoor 3.1/5 with high recent turnover | 7/10 |
| "Fully remote" but no async/timezone policy stated | 5/10 |

---

### Positive Signals

- Genuine AI/ML focus — not just buzzword usage
- Small team (12) means actual ownership and impact
- Early stage = potential equity upside if Series A closes
- Remote listed explicitly (not "remote-friendly")

---

### Risk Breakdown

| Category     | Risk Level |
|--------------|------------|
| Requirements | 🔴 High — 8 tech stack items + 5 yrs for broad scope |
| Culture      | 🔴 High — "wear many hats", "fast-paced" language |
| Remote       | 🟡 Medium — stated remote but no async policy detail |
| Hiring       | 🔴 High — no salary, vague comp, broad scope |
| Company      | 🔴 High — pre-Series A, low Glassdoor, recent churn |

---

### Final Verdict

⚠️ **Apply with Caution**

The role has genuine upside — real AI work, ownership, and early equity potential. But the risk flags are serious: financial instability, cultural red flags, and an unrealistic skill wish-list suggest either poor management or deliberate understaffing. Proceed only if you can validate comp, runway, and scope in the first call.

---

### 5 Smart Interview Questions

1. **"What does the engineering team's typical week look like — and what percentage of time is spent on planned work vs reactive tasks?"**
   *(Validates "fast-paced" and burnout risk)*

2. **"You mentioned 8 different technologies in the JD — which 2-3 are non-negotiable for day one, and which are aspirational?"**
   *(Validates unrealistic requirements)*

3. **"Can you share the current runway and expected Series A timeline? How does that affect team headcount plans?"**
   *(Validates financial stability risk)*

4. **"What's the on-call expectation, and how is it compensated? Is there an incident review culture or a blame culture?"**
   *(Validates work-life balance and culture)*

5. **"For the remote setup — is there a core overlap window expected, and how does the team handle async communication across timezones?"**
   *(Validates remote authenticity)*

---

## Key Learnings

**1. Job descriptions are marketing documents**
JDs are written to attract candidates, not to inform them. Every phrase is a signal. "Competitive salary" means they won't tell you. "Startup mindset" means no processes. Claude reads between the lines systematically.

**2. The risk score changes your mindset**
Without a score, you convince yourself to overlook flags. A number — 72/100 — makes it concrete. You can't unsee it. It forces a deliberate decision rather than optimistic application.

**3. Interview questions are the output that matters most**
Knowing the red flags is half the job. The smart questions are what let you validate them in a 30-minute call. Claude generates both together, which is the real value.

**4. This works for any career level**
A fresher worries about "excessive experience requirements." A senior worries about "equity vesting" and "runway." The same prompt surfaces different concerns depending on the JD — the prompt is role-agnostic.

**5. Prompt engineering as a career tool**
The structured output format (score → flags → table → verdict → questions) is itself a design decision. Changing the output format changes what you notice. This is prompt engineering applied to real life.

---

## How to Use This Yourself

```
1. Find any job posting
2. Copy the JD text
3. Find the company on LinkedIn, Glassdoor, Crunchbase
4. Copy relevant info (size, funding, reviews, recent news)
5. Open Claude → paste the prompt → replace [Paste Here] placeholders
6. Read the score, review flags, save the interview questions
7. Apply with clarity, not hope
```

---

## What I Would Build Next

- A web app that scrapes a LinkedIn job URL and auto-runs this analysis
- A browser extension that overlays a risk badge on LinkedIn job cards
- A comparison mode: analyze 3 JDs simultaneously and rank them
- Integration with Glassdoor API for live company data

---

## Files in This Folder

```
day14/
├── day14.md               ← this file
├── sample_jd.pdf          ← job description used for analysis
└── screenshots/
    ├── prompt_input.png
    ├── risk_score.png
    ├── red_flags.png
    └── interview_questions.png
```

---

## Part of

**Abtalks 60 Days Claude Challenge**
Day 14 of 60 — building real, shareable things with Claude every day.

*@Anthropic @ABTalksOnAI @AnilBajpai*

---

*Generated using Chain-of-Thought Reasoning · Abtalks 60 Days Challenge · Day 14*