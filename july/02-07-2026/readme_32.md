# 📈 Think Like a Marketing Strategist: Grow This Brand

**Day 32 Challenge** – An interactive marketing strategy simulator that teaches beginners how marketers think, not just what they do. Build a brand strategy, choose platforms, define content pillars, and get a personalized Growth Report.

![Think Like a Marketing Strategist Preview](https://via.placeholder.com/800x400?text=Think+Like+a+Marketing+Strategist)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🎯 Three Brand Modes

| Mode | Description |
|------|-------------|
| 🏢 **Use My Own Business** | Enter your business details and build a strategy tailored to your company. |
| 🙋 **Build My Personal Brand** | Use your name, expertise, and story as the brand. Platforms and content pillars adapt for personal branding. |
| 🎲 **A New Client Has Arrived** | Get a randomly generated business with industry, audience, budget, competitors, and a marketing challenge. |

### 🧠 Step-by-Step Marketing Strategy Flow

| Step | Name | Description |
|------|------|-------------|
| 1 | **Understand** | Review the brand's industry, audience, budget, competitors, and challenge. Learn why understanding is the foundation of strategy. |
| 2 | **Choose Platforms** | Select the best social platforms. Each platform shows suitability for your brand type. Personal brands get LinkedIn, X, YouTube, and newsletter weighting. |
| 3 | **Define Content Pillars** | Choose exactly 3 content pillars from 8 options. Each pillar shows its supporting goals. |
| 4 | **Build a Roadmap** | A 4-week content roadmap with weekly goals and strategies. Personal brands get Week 1 focused on defining POV and optimizing bio/profile. |
| 5 | **Handle an Unexpected Event** | A random marketing event appears (viral post, podcast invite, public disagreement, etc.). Choose how to respond and learn the consequences. |
| 6 | **View Your Growth Report** | Get a final score with 4 dimensions, best decision, biggest mistake, and 3 personalized marketing lessons. |

### 🤖 "How to Ask Claude" Cards

After every major section, a reusable prompt card appears:

- **Teaches prompt engineering** while learning marketing.
- **Personalized prompts** – for personal brand mode, prompts reference the person's name and niche.
- **Copy button** – easily copy prompts to use with Claude or other AI assistants.
- **Practical application** – learn to ask better questions.

### 📊 Growth Report

After completing all steps, you receive:

- **Overall Score** (0-100) with grade (A, B, C, D)
- **4 Dimension Scores**: Audience Understanding, Platform Strategy, Content Strategy, Growth Potential
- **Best Decision** – your strongest strategic choice
- **Biggest Mistake** – area with the most opportunity
- **3 Marketing Lessons** – personalized based on your strategy
- **Personal brand lessons** reference authenticity, consistency, and niche clarity

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Framework | React 18 (via CDN) + Babel Standalone JSX |
| Styling | Custom CSS (no Tailwind, no external assets) |
| Logic | Vanilla JavaScript with React hooks (`useState`, `useCallback`, `useMemo`, `useEffect`) |
| Architecture | Single HTML file, no backend, no APIs, no images |
| Offline | Runs completely offline after initial load |

---

## 📂 Project Structure

```
index.html          # Single self‑contained file (HTML + CSS + JSX)
```

No other files or dependencies – everything is in one file for maximum portability.

---

## 🧑‍💻 How to Play

1. **Open** `index.html` in your browser.
2. **Choose** your brand path:
   - 🏢 Use My Own Business – enter your business details
   - 🙋 Build My Personal Brand – enter your name, niche, and story
   - 🎲 A New Client Has Arrived – get a random business
3. **Understand** the brand – review the profile and learn why this matters.
4. **Choose** your social platforms – select up to 4. Learn why each platform is suitable (or not).
5. **Define** your 3 content pillars – pick from 8 options, each with supporting goals.
6. **Build** your 30-day content roadmap – review weekly goals and strategies.
7. **Handle** an unexpected marketing event – choose how to respond.
8. **View** your Growth Report – see your score, strengths, weaknesses, and lessons.
9. **Replay** to try a different brand or strategy.

---

## 🎯 Learning Objectives

After playing, you will understand:

- **Marketing strategy fundamentals** – why understanding the brand and audience comes first.
- **Platform selection** – how to choose the right channels for your brand.
- **Content pillars** – how to structure content around themes that support business goals.
- **Roadmap planning** – how to think in weekly goals and strategies, not just individual posts.
- **Event response** – how to handle unexpected marketing moments.
- **Personal branding** – authenticity, consistency, and niche clarity.
- **Prompt engineering** – how to ask AI for better marketing advice.

---

## 🎨 Customization

### 📝 Brand Data
- Business generation: Edit the `generateRandomBusiness` function.
- Industries, audiences, budgets, competitors, challenges: Edit the arrays at the top of the script.

### 📱 Platforms
- Business platforms: Edit the `PLATFORMS` array.
- Personal brand platforms: Edit the `PERSONAL_PLATFORMS` array.
- Adjust suitability, weights, and descriptions.

### 📚 Content Pillars
- Business pillars: Edit the `CONTENT_PILLARS` array.
- Personal brand pillars: Edit the `PERSONAL_PILLARS` array.
- Add or remove pillars, adjust goals and descriptions.

### ⚡ Events
- Business events: Edit the `EVENTS` array.
- Personal brand events: Edit the `PERSONAL_EVENTS` array.

### 📊 Scoring & Report
- Adjust scoring weights in the `generateReport` function.
- Modify grade thresholds and lesson generation logic.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by real‑world marketing strategy frameworks and personal branding principles.
- Built as an educational tool for marketers, entrepreneurs, and anyone building a brand.
- Designed to teach strategic thinking, not just content creation.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy strategizing! 📈**