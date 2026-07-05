# 🕵️ Marketing Detective

**Day 34 Challenge** – An interactive detective game that teaches marketing strategy through real-world case analysis. Investigate marketing campaigns, gather evidence, identify the primary mistake, and learn from detailed explanations and improvements.

![Marketing Detective Preview](https://via.placeholder.com/800x400?text=Marketing+Detective)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🎯 Core Gameplay

- **10+ Detailed Marketing Cases** – Each case includes company name, industry, campaign objective, target audience, marketing channels, budget allocation, campaign metrics, customer comments, social media performance, one primary marketing mistake, three supporting clues, correct explanation, and suggested improvements.
- **Case Assignment** – Receive a randomized marketing case with full campaign details and performance data.
- **Investigation Board** – Interactive corkboard-style interface where you drag and drop evidence clues.
- **Solve the Case** – Once you've placed at least 3 pieces of evidence, reveal the primary marketing mistake.
- **Learning Report** – After solving, view the mistake, what really happened, and suggested improvements.

### 🎨 Premium Detective Aesthetic

- **Corkboard Theme** – Realistic cork texture with push pins, sticky notes, and file folders.
- **Dark Detective UI** – Premium dark theme with glowing accents and paper textures.
- **Draggable Evidence** – Interactive evidence cards that you can drag onto the investigation board.
- **Case Closed Animation** – Celebratory overlay when you solve the case.
- **Smooth Transitions** – Animated cards, hover effects, and progress indicators.

### 🎮 User Flow

| Step | Phase | Description |
|------|-------|-------------|
| 1 | **Theme Selection** | Choose from 5 color themes (Claude Orange, Ocean Blue, Forest Green, Midnight Purple, Rose) |
| 2 | **Case Assignment** | Review the marketing case with company details, campaign objectives, and performance metrics |
| 3 | **Investigation** | Drag evidence clues onto the investigation board to build your case |
| 4 | **Solve the Case** | Reveal the primary marketing mistake when you've placed enough evidence |
| 5 | **Learning Report** | View the mistake, explanation, and suggested improvements |

### 📊 Case Data Structure

Each case contains:

- **Company Name** & **Industry**
- **Campaign Objective** & **Target Audience**
- **Marketing Channels** & **Budget Allocation**
- **Campaign Metrics**: Reach, CTR, Engagement, Conversions, Sales
- **Customer Comments** & **Social Media Performance**
- **Primary Marketing Mistake** – The core problem
- **3 Supporting Clues** – Evidence to discover
- **Correct Explanation** – What really happened
- **Suggested Improvements** – Actionable recommendations

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Framework | React 18 (via CDN) + Babel Standalone JSX |
| Styling | Pure Vanilla CSS (no frameworks) |
| Logic | Vanilla JavaScript with React hooks |
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
2. **Choose** your color theme from the options.
3. **Click** "Start Your Investigation" to begin.
4. **Review** the case assignment – read about the company, campaign objective, target audience, budget, and performance metrics.
5. **Click** "Begin Investigation" to enter the investigation board.
6. **Gather evidence** – click on evidence clues to select them, or drag them directly onto the investigation board.
7. **Place evidence** – drop at least 3 pieces of evidence onto the board.
8. **Solve the case** – click "Solve the Case" when you're ready.
9. **Review** the learning report – see the marketing mistake, explanation, and suggested improvements.
10. **Replay** – click "New Case" to get a fresh case with a different marketing challenge.

---

## 🎯 Learning Objectives

After playing, you will understand:

- How to analyze marketing campaigns from a strategic perspective
- Common marketing mistakes and their root causes
- The importance of audience targeting and message alignment
- How to identify gaps between campaign objectives and execution
- Practical marketing improvements for real-world scenarios
- The relationship between marketing channels, budget, and performance metrics

---

## 🎨 Customization

### 📝 Marketing Cases
Edit the `MARKETING_CASES` array to add, remove, or modify cases. Each case object should include all required fields (company, industry, objective, audience, channels, budget, metrics, comments, social, mistake, clues, explanation, improvements).

### 🎨 Themes
Add new themes by editing the `THEMES` array with an `id`, `label`, and `color`. Modify theme colors in the CSS `[data-theme]` selectors.

### 🎮 Game Mechanics
- Adjust the number of evidence pieces required to solve a case (currently 3) in the `canSolve` logic.
- Modify the case selection logic to change how cases are randomized.

---

## 📚 Sample Cases

The game includes 10 detailed marketing cases covering:

1. **Organic Skincare** – Influencer targeting mismatch
2. **Health Tech** – Acquisition vs. retention imbalance
3. **Specialty Coffee** – Digital vs. local engagement
4. **EdTech** – Upsell before fixing UX issues
5. **Renewable Energy** – Technical vs. benefit messaging
6. **Fashion Retail** – Post-purchase experience neglect
7. **B2B Consulting** – Generic vs. vertical-specific messaging
8. **Pet Products** – Unpersonalized cross-selling
9. **Telemedicine** – Patient retention and reminders
10. **Green Cleaning** – Packaging for retail vs. social media

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by real-world marketing case studies and strategic analysis.
- Built as an educational tool for marketers, entrepreneurs, and anyone interested in marketing strategy.
- Designed with a premium detective aesthetic for an engaging learning experience.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy investigating! 🕵️**