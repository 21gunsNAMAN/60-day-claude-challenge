# Day 9 — Iterative AI Development with NutriScope

## What I Built

**NutriScope** — a single-file HTML nutrition tracking application, built in two iterations using the iterative AI development workflow.

---

## The Core Lesson: MVP First, Then Enhance

The biggest mistake beginners make is prompting AI to build a massive, complex app all at once. This leads to:
- Incomplete or broken outputs
- Hard-to-debug code
- Inconsistent quality

The professional approach is **iterative development**:
1. Build a working MVP
2. Test and validate it
3. Progressively layer on complexity

---

## Iteration 1 — MVP

**Prompt goal:** Build a working, complete nutrition tracker with core features only.

### Features Built
- Profile inputs: age, gender, height, weight, activity level, dietary preference (Vegetarian / Non-Vegetarian / Eggetarian)
- Food database: 20 common Indian foods (Rice, Roti, Dal, Paneer, Curd, Chana, Rajma, Banana, Apple, Milk, Oats, Bread, Egg, Chicken, Fish, Potato, Poha, Idli, Dosa, Spinach)
- Food log: add food, quantity, unit, editable table, remove entries
- Tracks: Calories, Protein, Carbs, Fat, Fiber, Iron, Calcium, Vitamin C, Vitamin D, Vitamin B12
- Dashboard: energy stats, macro progress bars, doughnut chart (Chart.js), deficiency/excess analysis, full nutrient table
- Recommendations: personalised based on dietary preference
- Design: dark theme, premium SaaS UI, mobile responsive, single HTML file

### What Made the MVP Successful
- Clear, bounded scope — only 20 foods, only 10 nutrients
- Single deliverable: one working HTML file
- Focused on the core loop: log food → see progress → get tips

---

## Iteration 2 — Enhanced Version

**Prompt goal:** Progressively add advanced features on top of the working MVP.

### Features Added
| Feature | Detail |
|---|---|
| Food database | Expanded from 20 → 60 foods (added salmon, tuna, mutton, soybean, broccoli, sweet potato, mango, guava, almonds, walnuts, chia seeds, flaxseeds, and more) |
| Nutrients tracked | Added magnesium, zinc, potassium, folate, omega-3 (total: 15 nutrients) |
| CSV import | Upload a `.csv` file to bulk-import food entries |
| 2-day meal planner | Plan breakfast, lunch, dinner, and snacks for two days with live nutrition summary |
| Risk analysis | Contextual health risk cards (anaemia, B12 deficiency, bone health, diabetes carb risk, caloric restriction) |
| Condition-aware targets | Adjusted targets for diabetes, hypertension, osteoporosis, anaemia |
| Advanced charts | Added micronutrient radar chart + meal breakdown bar chart (alongside existing doughnut) |
| Nutrition education | Macros and key micronutrients explained with sources |
| Scientific references | 6 cited sources: ICMR-NIN, USDA FoodData Central, WHO, Mifflin-St Jeor, NIN India, IOM |
| Educational disclaimer | Medical advice caveat prominently displayed |

---

## Comparison: MVP vs Enhanced

| Dimension | MVP | Enhanced |
|---|---|---|
| Foods in database | 20 | 60 |
| Nutrients tracked | 10 | 15 |
| Charts | 1 (doughnut) | 3 (doughnut + radar + bar) |
| Sections / tabs | 4 | 7 |
| Meal planning | ✗ | ✓ 2-day planner |
| CSV import | ✗ | ✓ |
| Risk analysis | ✗ | ✓ |
| Health conditions | ✗ | ✓ (4 conditions) |
| Education section | ✗ | ✓ with sources |
| File size | ~12 KB | ~28 KB |

---

## Key Learnings

**1. MVP First is non-negotiable**
Trying to build the enhanced version in one shot would have produced a bloated, error-prone output. Starting with the MVP gave a clean, tested foundation.

**2. Iterative prompting = better quality**
Each prompt had a single, clear goal. The AI could focus on doing one thing well rather than juggling 20 requirements simultaneously.

**3. Scope control is a skill**
Knowing what to include in the MVP (and what to hold back) is just as important as knowing what to build. The MVP had everything needed to be useful — nothing more.

**4. Single-file HTML is powerful**
No backend, no dependencies beyond a CDN-hosted Chart.js. The entire app — UI, logic, data, charts — ships as one file anyone can open in a browser.

**5. AI builds faster when you think first**
The clearest prompts produced the cleanest code. Time spent defining requirements before prompting paid off in output quality.

---

## Files in This Folder

| File | Description |
|---|---|
| `nutri-scope-mvp.html` | Iteration 1 — working MVP with 20 foods, 10 nutrients, core dashboard |
| `nutri-scope-enhanced.html` | Iteration 2 — full featured app with 60 foods, meal planner, risk analysis, education |
| `day9.md` | This file |

---

## Tech Stack

- Pure HTML + CSS + Vanilla JavaScript
- [Chart.js 4.4.1](https://www.chartjs.org/) via CDN
- No backend, no build step, no framework
- Mobile responsive, dark theme

---

## Nutrient Data Sources

- **ICMR-NIN (2020)** — Recommended Dietary Allowances for Indians
- **USDA FoodData Central** — International food composition database
- **NIN India** — Indian Food Composition Tables
- **Mifflin-St Jeor Equation** — BMR / TDEE calculation
- **WHO Global Nutrition Targets 2025**
- **Institute of Medicine (IOM/NAP)** — Dietary Reference Intakes

---

*Built as part of a 30-day AI product building challenge. Day 9 focus: iterative development and MVP-first thinking.*