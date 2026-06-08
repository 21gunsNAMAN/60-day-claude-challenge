# 🌍 Day 8 — Personal Environmental Health Analyzer

## AB Talks: 30 Days of Claude AI Challenge

> **Day 8 Theme:** Claude Artifacts — Building Real Interactive Applications from Prompts

---

## 📌 What I Built

A fully interactive **Personal Environmental Health Analyzer** dashboard built entirely with a single Claude prompt — no code written manually.

The artifact analyzes real-time AQI (Air Quality Index), PM2.5, PM10, and water quality data for **10 Indian cities**, with a personalized deep-dive for **Rishikesh, Uttarakhand**.

---

## 🎯 Challenge Objectives

| # | Task | Status |
|---|------|--------|
| 1 | Read provided resources on Claude Artifacts | ✅ |
| 2 | Watch the solution video | ✅ |
| 3 | Open Claude.ai and start a new conversation | ✅ |
| 4 | Paste the Environmental Health Analyzer prompt | ✅ |
| 5 | Allow Claude to build the dashboard | ✅ |
| 6 | Generate the downloadable HTML application | ✅ |
| 7 | Test filters, charts, and interactive elements | ✅ |
| 8 | Take screenshots of the dashboard | ✅ |
| 9 | Create Day8 folder in GitHub repository | ✅ |
| 10 | Create this day8.md file | ✅ |
| 11 | Upload screenshots, HTML, and learnings | ✅ |
| 12 | Commit and push changes | ✅ |

---

## 🛠️ Prompt Used

> *Role:* Senior Data Analyst + Environmental Researcher + UX Designer + Frontend Dashboard Developer
>
> The prompt instructed Claude to:
> - Auto-detect user location and fetch live AQI + water quality data
> - Generate a full analysis (cleanest city, most polluted, averages, trends, anomalies)
> - Build a dark-themed, mobile-responsive dashboard with 5 tabs, 6+ charts, and interactive filters
> - Produce a Personal Report Card with A–F grades and a 0–100 health score
> - Provide personalized recommendations for air, water, hair, and skin health

---

## 📊 Dashboard Features

### Key Metrics Panel
- Average AQI across 10 cities
- Highest AQI city (Kolkata — 103)
- Lowest AQI city (Bengaluru — 44)
- Rishikesh AQI (68 — Satisfactory)
- Overall Environmental Health Score (62/100)

### 📈 Visualizations
- AQI Comparison Bar Chart (all cities)
- PM2.5 Levels Chart (µg/m³)
- PM10 Levels Chart (µg/m³)
- AQI Distribution Donut Chart
- City Health Rankings (horizontal bar)
- Seasonal AQI Trend Line (Rishikesh)
- Environmental Score Comparison

### 🎛️ Interactive Filters
- City Selector dropdown
- Pollutant Selector (AQI / PM2.5 / PM10)
- Health Risk Filter (Low / Moderate / High)
- AQI Range Slider
- Compare Mode toggle

### 📋 5 Dashboard Tabs
1. **Overview** — All cities, charts, and detail cards
2. **Health Analysis** — AQI impact on lungs, sleep, energy, exercise + water impact on hair & skin
3. **Report Card** — Air Score (64), Water Score (58), Overall Grade (B−)
4. **Insights** — Top cleanest/polluted cities, anomalies, trend analysis
5. **Recommendations** — Daily actions, indoor air, outdoor guide, hair care, skin care, water improvements

---

## 🔍 Key Findings

### Air Quality
| City | AQI | Category | Health Score |
|------|-----|----------|-------------|
| Bengaluru | 44 | 🟢 Good | 82 |
| Mumbai | 56 | 🟡 Satisfactory | 70 |
| Pune | 59 | 🟡 Satisfactory | 72 |
| Chennai | 67 | 🟡 Satisfactory | 74 |
| **Rishikesh** | **68** | **🟡 Satisfactory** | **62** |
| Ahmedabad | 68 | 🟡 Satisfactory | 63 |
| New Delhi | 73 | 🟡 Satisfactory | 60 |
| Haridwar | 82 | 🟡 Satisfactory | 58 |
| Hyderabad | 91 | 🟡 Satisfactory | 52 |
| Kolkata | 103 | 🟠 Moderate | 48 |

### Water Quality (Rishikesh)
- **TDS:** ~217 mg/L (moderately hard)
- **Total Hardness:** ~90–107 mg/L
- **pH:** ~7.2–7.4 (acceptable)
- **Concern:** Seasonal coliform spikes, especially during monsoon
- **Source:** River Ganga at Triveni Ghat

---

## 😲 Most Surprising Observation

**Rishikesh — a Himalayan pilgrimage town — records PM2.5 at 6× the WHO annual guideline**, despite having no heavy industry. The culprits: ceremonial smoke from Ganga Aarti, tourist vehicle density, seasonal crop burning in neighboring states, and valley geography that traps particulates overnight.

Meanwhile, **Bengaluru — a metro of 13 million people — consistently outperforms several Himalayan towns**, thanks to its 920m elevation, green canopy, and favorable wind patterns.

---

## 💡 Key Learnings

### About Claude Artifacts
1. **Artifacts generate real, runnable applications** — not just text descriptions or code snippets. The output is a live, interactive HTML app.
2. **Prompt structure matters enormously.** Breaking the request into clear sections (Data Rules → Analysis → Dashboard → Filters → Design) gave Claude a clear "architecture" to follow.
3. **Claude auto-fetches live data** when no dataset is provided — it used IQAir, AQI.in, AQICN, and CPCB sources automatically.
4. **Role-stacking in prompts works.** Assigning Claude multiple expert roles (Data Analyst + UX Designer + Frontend Dev) produces significantly richer output than a single role.
5. **Design instructions translate into real CSS.** "Dark theme, premium UI, smooth animations" directly produced a polished dark-mode dashboard with gradients and transitions.

### About Environmental Data
6. PM2.5 levels in Indian cities — even "clean" ones — are well above WHO guidelines year-round.
7. Water hardness in Himalayan towns like Rishikesh is often overlooked but has real impact on hair and skin health.
8. June is India's best month for AQI in most cities — pre-monsoon winds clear particulate build-up from summer.

### About the Workflow
9. One prompt → complete product. This is the core insight of Day 8. Claude Artifacts compress what would normally be a multi-day development effort into minutes.
10. The downloadable HTML file runs entirely in-browser — no server, no dependencies, no installation needed.

---

## 🗂️ Files in This Folder

```
Day8/
├── day8.md                          ← This file
├── index.html                       ← Complete downloaded dashboard application
└── screenshots/
    ├── 01_overview_metrics.png      ← Key metrics + AQI comparison chart
    ├── 02_city_cards.png            ← Interactive city detail cards
    ├── 03_health_analysis_tab.png   ← Air & water health impact panel
    ├── 04_report_card_tab.png       ← Personal Environmental Report Card
    ├── 05_insights_tab.png          ← Top cities, anomalies, trend chart
    └── 06_recommendations_tab.png   ← Personalized action recommendations
```

---

## 🔗 Data Sources

| Source | URL | Used For |
|--------|-----|----------|
| IQAir | iqair.com/in-en/india | Real-time AQI & PM2.5 |
| AQI.in | aqi.in/dashboard/india | City-level AQI comparison |
| AQICN | aqicn.org | Station-level Rishikesh data |
| CPCB India | cpcb.nic.in | Official India AQI bulletin |
| Tandfonline / Academia.edu | (peer-reviewed) | Ganga water quality parameters |

---

## 🚀 How to Run the Dashboard

1. Download `index.html` from this folder
2. Open it in any modern browser (Chrome, Firefox, Safari, Edge)
3. No internet connection required — fully self-contained
4. Interact with tabs, filters, sliders, and city cards

---

## 📅 Challenge Progress

| Day | Topic | Status |
|-----|-------|--------|
| Day 1 | Introduction to Claude | ✅ |
| Day 2 | Prompt Engineering Basics | ✅ |
| Day 3 | Claude for Writing | ✅ |
| Day 4 | Claude for Research | ✅ |
| Day 5 | Claude for Code | ✅ |
| Day 6 | Claude for Data Analysis | ✅ |
| Day 7 | Claude for Creative Work | ✅ |
| **Day 8** | **Claude Artifacts & Interactive Apps** | **✅ Today** |

---

*Part of the AB Talks: 30 Days of Claude AI Challenge*
*Built with Claude Sonnet · Data from IQAir, AQI.in, CPCB · June 2026*
