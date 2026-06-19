# ⚽ Football Intelligence Hub – README

**An interactive, self‑contained web application that combines data‑driven World Cup predictions, a dynamic football IQ quiz, and a personality assessment inspired by Messi and Ronaldo.**

---

## 🚀 Overview

This project transforms the **Football Intelligence Hub** prompt into a fully functional single‑page HTML experience. It guides users through three connected stages:

1. **Stage 0** – Knowledge Level Check (adapts all following content to the user’s familiarity with football).
2. **Stage 1** – FIFA World Cup 2026 Prediction Report (with optional Excel/CSV upload for evidence‑based analysis).
3. **Stage 2** – Football IQ Quiz (adaptive multiple‑choice questions with a calculated Awareness Score and classification).
4. **Stage 3** – Messi vs Ronaldo Personality Match (mixed‑question quiz that maps the user to one of the legends and assigns a football archetype).

The final output is a **Football Intelligence Profile** – a single, shareable summary containing all predictions, scores, compatibility percentages, and personalised recommendations.

---

## ✨ Key Features

| Feature | Description |
| :--- | :--- |
| **Adaptive Difficulty** | The depth of predictions, quiz questions (beginner/intermediate/advanced), and explanation detail adjust automatically based on the user’s self‑assessed knowledge level. |
| **Workbook Integration** | Users can upload an Excel (`.xlsx`/`.xls`) or CSV file. The tool parses it using **SheetJS** and uses it as a data source to slightly tweak prediction confidences – simulating a fully referenced analysis. |
| **World Cup 2026 Report** | Delivers a most‑likely winner, runner‑up, dark horse, and players to watch – each with a 0‑100% confidence score, supporting evidence, and key risks. |
| **Football IQ Quiz** | Generates 4‑5 questions from a pool of beginner, intermediate, and advanced items. After scoring, it provides a **Football Awareness Score (0‑100)**, a fan classification (e.g., *Football Enthusiast*), and highlights the user’s strongest/weakest knowledge areas. |
| **Personality Assessment** | 12 questions (multiple‑choice + rating scales) that avoid direct Messi vs Ronaldo queries. Calculates compatibility percentages for both legends, explains the match, and assigns one of 8 archetypes (e.g., *Creative Playmaker*, *Relentless Competitor*). |
| **Final Profile** | Combines all results into a polished, printable summary with recommended players, clubs, national teams, and rivalries to explore. |

---

## 🛠️ Tech Stack

- **HTML5** – Semantic structure and layout.
- **CSS3** – Custom dark‑theme styling with responsive design.
- **Vanilla JavaScript** – All logic, state management, and DOM manipulation.
- **SheetJS (CDN)** – Optional library for parsing uploaded Excel/CSV files. Falls back gracefully if the file cannot be parsed.

---

## 📁 File Structure

Since this is a **single‑page application**, the entire project lives in one file:

```
index.html          # Complete application (HTML, CSS, JS)
README.md           # This file
```

No additional dependencies, build tools, or servers are required – just open the HTML in any modern browser.

---

## 📖 How to Use

1. **Open the HTML file** in your browser (Chrome, Edge, Firefox, etc.).
2. **Stage 0** – Select your football knowledge level (A–D) and click *Confirm*.
3. **Stage 1** – (Optional) Upload your Excel/CSV workbook, then click *Generate Prediction Report* or *Skip & use global data*. Review the report and proceed.
4. **Stage 2** – Answer the adaptive quiz questions, then click *Score my quiz* to see your Football Awareness Score and classification. Proceed to the next stage.
5. **Stage 3** – Answer all 12 personality questions (both multiple‑choice and slider‑based ratings). Click *Reveal my profile* to generate your final Football Intelligence Profile.
6. **Review** your complete profile – including predictions, scores, personality match, archetype, and recommendations. Use the *Start Over* button to reset the experience.

---

## 📊 Uploading a Workbook (Stage 1)

- The tool expects an Excel (`.xlsx`, `.xls`) or CSV file.
- If the file is successfully parsed, the prediction confidence values are slightly adjusted – simulating a “data‑driven” effect.
- The file is **never sent to a server** – all processing happens entirely in the browser.
- If you don’t have a workbook, the tool uses a built‑in global dataset so you can still enjoy the full experience.

---

## 🧠 Quiz & Personality Logic

### Quiz Questions
- The question pool contains beginner, intermediate, and advanced items covering **Rules**, **History**, **Tactics**, and **Analytics**.
- The number and difficulty of questions are selected based on the user’s Stage 0 answer.

### Personality Mapping
- Each multiple‑choice and rating‑scale answer is heuristically mapped to traits associated with Messi (e.g., humility, creativity, team‑orientation) or Ronaldo (e.g., intensity, ambition, risk‑taking).
- The final compatibility percentage is normalised to a 0‑100 scale.
- The archetype is derived from which legend the user leans toward and the overall balance of their responses.

---

## 🎨 Customisation

You can easily modify the experience by editing the JavaScript data pools in the `<script>` section:

- **Prediction data** – Update the `getPredictionData()` function to change winners, confidences, evidence, or risks.
- **Quiz questions** – Extend or modify the `questionPool.beginner`, `.intermediate`, and `.advanced` arrays.
- **Personality questions** – Add, remove, or rephrase items in the `personalityQuestions` array.
- **Archetypes** – Adjust the archetype logic inside `computePersonalityProfile()` to add new categories or change descriptions.

---

## 🌐 Browser Support

Works on all modern browsers that support:
- ES6 JavaScript
- CSS Grid & Flexbox
- File API (for uploads)
- `<input type="range">` for sliders

*Internet Explorer is not supported.*

---

## 📦 Running Locally

No installation or build step is required. Simply:

```bash
# Clone or download the repository
# Double‑click on index.html
# Or serve it with any static server:
npx serve .
```

---

## 🤝 Contributing

Feel free to fork this project and submit pull requests for:
- Expanding the question/archetype pools.
- Adding more sophisticated workbook parsing (e.g., extracting real player stats).
- Improving the personality mapping algorithm.
- Enhancing the UI/UX with animations or dark/light mode toggles.

---

## 📄 License

This project is open‑source and available under the **MIT License**.

---

## ❓ Questions or Feedback?

If you encounter any issues or have ideas for improvement, please open an issue in the repository or reach out directly.

---

**Enjoy the experience – and may your football intelligence be ever‑growing!** ⚽🧠