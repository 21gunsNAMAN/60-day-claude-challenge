# 🔍 Media Integrity Analyzer

**Day 33 Challenge** – An interactive media literacy learning tool that teaches you how to spot exaggerated headlines and emotional manipulation in the media you consume every day. Two guided challenges help you build critical thinking skills through discovery, not testing.

![Media Integrity Analyzer Preview](https://via.placeholder.com/800x400?text=Media+Integrity+Analyzer)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🎨 Customizable Color Themes

Choose from five premium dark themes:
- **Claude Orange** (default)
- **Ocean Blue**
- **Forest Green**
- **Midnight Purple**
- **Rose**

### 🕵️ Challenge 1: Headline Detective

| Step | Description |
|------|-------------|
| **Read** | A fictional news headline and matching article |
| **Click** | Decide if you would click the headline (Yes / Maybe / No) |
| **Identify** | Click on parts of the headline you think are exaggerated or misleading |
| **Reveal** | View the Headline Accuracy Score, highlighted mismatches with explanations, a fair rewritten headline, and a key takeaway |

### ❤️ Challenge 2: Emotion Detector

| Step | Description |
|------|-------------|
| **Read** | A fictional social media post, reel caption, or article excerpt |
| **Feel** | Select how the post makes you feel from a list of emotions |
| **Identify** | Click on the words or phrases that influenced your feelings |
| **Reveal** | View the target audience, intended emotional response, manipulation technique, highlighted emotional phrases, a neutral rewrite, and a key takeaway |

### 📊 Live Media Integrity Metrics

Four metrics update in real time as you progress:

- **Headline Accuracy** – How well you spot exaggerations
- **Source Reliability** – Your ability to evaluate credibility
- **Emotional Manipulation** – Your awareness of emotional hooks
- **Audience Targeting** – Your understanding of who content is designed for

### 📋 Final Media Integrity Dashboard

After completing both challenges, you receive:

- **Overall Media Integrity Score** (0-100%)
- **What You Learned** – A summary of your progress
- **Biggest Red Flag** – Personalized feedback on your biggest vulnerability
- **3 Practical Media Literacy Habits** – Actionable tips for everyday life
- **Replay Button** – Generates completely new scenarios for fresh practice

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Structure | HTML5 |
| Styling | Pure Vanilla CSS (no frameworks) |
| Logic | Pure Vanilla JavaScript (no frameworks) |
| Architecture | Single HTML file, no backend, no APIs, no images |
| Offline | Runs completely offline after initial load |

---

## 📂 Project Structure

```
index.html          # Single self‑contained file (HTML + CSS + JS)
```

No other files or dependencies – everything is in one file for maximum portability.

---

## 🧑‍💻 How to Play

1. **Open** `index.html` in your browser.
2. **Choose** your color theme from the options.
3. **Click** "Start Learning" to begin.
4. **Challenge 1 – Headline Detective:**
   - Read the headline and article.
   - Decide if you would click the headline.
   - Click on the exaggerated or misleading parts.
   - Click "Reveal Analysis" to see your score and learn from the breakdown.
5. **Challenge 2 – Emotion Detector:**
   - Read the social media post or excerpt.
   - Select how it makes you feel.
   - Click on the words that influenced your feelings.
   - Click "Reveal Analysis" to see the breakdown.
6. **Review** your live metrics as you progress.
7. **View** your final Media Integrity Dashboard.
8. **Replay** to practice with new random scenarios.

---

## 🎯 Learning Objectives

After completing the challenges, you will understand:

- How headlines can exaggerate or distort the truth
- How to spot emotional manipulation in social media content
- Why it's important to read beyond the headline
- How content creators use language to influence your feelings
- Practical habits for becoming a more critical media consumer
- How to identify target audiences and hidden agendas

---

## 🎨 Customization

### 📝 Scenarios
- **Headline scenarios**: Edit the `HEADLINE_SCENARIOS` array to add, remove, or modify headlines, articles, mismatches, rewrites, and takeaways.
- **Post scenarios**: Edit the `POST_SCENARIOS` array to add, remove, or modify social media posts, target audiences, emotions, manipulation techniques, and rewrites.

### 🎨 Themes
- Add new themes by editing the `THEMES` array with an `id`, `label`, and `color`.
- Modify theme colors in the CSS `[data-theme]` selectors.

### 📊 Metrics
- Adjust scoring logic in the `renderReveal1` and `renderReveal2` functions.
- Modify metric calculation formulas to change difficulty or emphasis.

### 📋 Dashboard
- Edit the `lessons` array in the `renderDashboard` function to change the practical habits displayed.
- Modify the red flag logic to provide different feedback.

---

## 🧠 Educational Design

This tool is built on **discovery learning** principles:

- **No prior knowledge required** – every concept is explained before the challenge
- **Learn by doing** – active participation reinforces understanding
- **Immediate feedback** – reveals show exactly what you missed and why
- **Practical application** – lessons connect to everyday media consumption
- **Safe practice environment** – fictional scenarios with no real-world consequences

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by media literacy education and critical thinking frameworks.
- Built as an educational tool for students, educators, and anyone who wants to become a more discerning media consumer.
- Designed with a premium editorial aesthetic for an engaging learning experience.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy analyzing! 🔍**