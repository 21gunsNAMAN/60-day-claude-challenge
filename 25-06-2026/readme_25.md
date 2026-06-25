# 🦈 AI Shark Tank Simulator

**Day 25 Challenge** – A fully interactive, single‑file HTML experience where you pitch your startup to four AI judges, answer their questions, and get an investment decision with real‑time scoring and feedback.

![Shark Tank AI Preview](https://via.placeholder.com/800x400?text=AI+Shark+Tank+Simulator)

---

## 🚀 Live Demo

No installation needed – just open the `index.html` file in your browser.  
All logic runs client‑side; no backend, no dependencies, no data sent anywhere.

---

## ✨ Features

### 📝 Pitch Submission
- Enter your startup name, problem, solution, revenue model, target audience, and funding ask.
- Review your pitch before entering the Q&A round.

### 🧠 4 Distinct AI Judges
Each judge has a unique personality and focus area:
- **🦈 Venture Capitalist** – Market size & scalability
- **🧑‍💼 Founder** – Execution & team
- **👤 Customer** – Usefulness & value
- **💰 Angel Investor** – Profitability & ROI

### 💬 Dynamic Q&A Round
- Each judge asks 2 questions (total 8).
- Type your answers; the judge reacts with tailored feedback based on your response quality.
- Skip option available if you're stuck.

### 📊 Scoring System (out of 100%)
Five categories are scored:
- Market Potential
- Innovation
- Business Model
- Execution
- Investment Worthiness

Scores are calculated using:
- Clarity and detail in your pitch
- Length and richness of your Q&A answers
- Positive reaction sentiment from judges

### 🏆 Investment Decision
After the Q&A, you receive one of four verdicts:
- 🟢 **Invest** (score ≥ 85)
- 🟡 **Come Back Later** (70–84)
- 🟠 **Acquire** (55–69)
- 🔴 **Reject** (< 55)

Each decision includes:
- Suggested valuation
- Funding amount
- Detailed reasoning

### 🎉 Bonus Features
- **Confetti** animation on high‑score funding success.
- **Downloadable PDF Report** – export your pitch, scores, and decision as a PDF.
- **Leaderboard** – stores top 20 scores locally in your browser.
- **Share Result** – copy a formatted summary to your clipboard or use the Web Share API.

---

## 🛠️ Technology

| Area | Used |
|------|------|
| Frontend | Vanilla HTML, CSS, JavaScript |
| Styling | Dark theme with Shark Tank vibes, CSS animations, responsive design |
| PDF Export | [jsPDF](https://github.com/parallax/jsPDF) (loaded from CDN) |
| Icons | Font Awesome 6 |
| Data persistence | `localStorage` for leaderboard |

---

## 📂 Project Structure

```
index.html          # Single self‑contained file (all HTML, CSS, JS)
```

No other files or dependencies required – everything is in one file for maximum portability.

---

## 🧑‍💻 How to Use

1. **Open** `index.html` in any modern browser (Chrome, Firefox, Edge, Safari).
2. **Click** “Start Your Pitch” and fill in the form.
3. **Review** your pitch and hit “Start Q&A Round”.
4. **Answer** each judge’s two questions. Submit or skip.
5. **View** your final score, investment decision, and detailed breakdown.
6. **Celebrate** with confetti if you get funded! 🎊
7. **Download** your PDF report, **share** your result, or check the **leaderboard**.

---

## 🎨 Customization

You can easily modify the judges, questions, scoring logic, or styling:

- **Judge list:** Edit the `JUDGES` array in the JavaScript section.
- **Questions:** Change the `questions` array for each judge.
- **Scoring:** Adjust the weights and thresholds in the `calculateScores()` function.
- **Verdict thresholds:** Modify the score ranges in `generateDecision()`.
- **Styling:** Edit the CSS variables at the top of the `<style>` block.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by the TV show *Shark Tank* and the Y Combinator startup pitch format.
- Built as a fun project to demonstrate AI‑powered interactive experiences without a backend.

---

## 📬 Feedback

If you have suggestions or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy pitching! 🦈**