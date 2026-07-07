# 🧠 Cognitive Pattern Explorer

**Day 36 Challenge** – A psychology-inspired self-reflection experience that explores thinking patterns through interactive scenarios. Designed to feel calm, game-like, and exploratory rather than like a test.

![Cognitive Pattern Explorer Preview](https://via.placeholder.com/800x400?text=Cognitive+Pattern+Explorer)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🎯 Core Experience

- **Calm & Stress Modes** – Toggle between two visual and experiential modes to explore how environment might influence your thinking.
- **Three Interactive Chapters** – Each chapter builds on the previous one, creating a cohesive self-reflection journey.
- **5 Thinking Tendencies** – Analytical Thinker, Emotional Intuitive, Overthinking Loop Style, Action-First Decision Maker, and Balanced Reflective Thinker.
- **Non-Diagnostic Language** – Uses reflective phrases like "you often..." and "this suggests..." instead of absolute labels. Educational only – never clinically assesses mental health.

### 📖 Chapter Flow

| Chapter | Name | Description |
|---------|------|-------------|
| 1 | **Discover Your Thinking Style** | Answer 5 multiple-choice questions about how you approach problems, decisions, and pressure. |
| 2 | **Choose Your Priorities** | Drag cards to rank what matters most to you – revealing what you value when making decisions. |
| 3 | **Map Your Thinking** | Use sliders to rate how often you pause, analyze, feel, act, and review in your daily life. |

### 📋 Final Reflection Journal

After completing all chapters, you receive:

- **Primary Thinking Pattern** – Your dominant tendency with personalized insight
- **Percentage Breakdown** – Visual bar chart showing all 5 tendencies
- **Key Metrics** – Primary pattern percentage, balanced reflector score, and range of styles
- **Personalized Insight** – What your pattern means for you, with mode-specific context
- **Mode Reflection** – Calm Mode or Stress Mode perspective on your thinking

### 🎨 Design

- **Calm Modern Aesthetic** – Warm, earthy tones with soft shadows and gentle animations
- **Smooth Transitions** – Page transitions, hover effects, and ambient animations
- **Progress Indicators** – Step dots and progress bars showing your journey
- **Responsive Layout** – Works beautifully on desktop, tablet, and mobile
- **Keyboard Accessibility** – Full keyboard navigation support
- **Reduced Motion Support** – Respects system preferences for reduced motion

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Structure | HTML5 |
| Styling | Pure Vanilla CSS (no frameworks) |
| Logic | Pure Vanilla JavaScript (no frameworks) |
| Drag-and-Drop | Native HTML5 Drag & Drop with Touch Fallback |
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
2. **Choose** your mode – 🌿 Calm Mode or 🔥 Stress Mode.
3. **Click** "Begin Exploration" to start.
4. **Chapter 1 – Discover Your Thinking Style:**
   - Answer 5 multiple-choice questions.
   - Choose the option that resonates most with you.
   - Progress bar shows your advancement.
5. **Chapter 2 – Choose Your Priorities:**
   - Drag items from "Available" to "Ranked" in order of priority.
   - Use native drag-and-drop or touch drag on mobile.
   - Click the ✕ button to remove an item from ranked.
6. **Chapter 3 – Map Your Thinking:**
   - Adjust 5 sliders to reflect your approach to each pattern.
   - Each slider ranges from 0 to 100.
   - All sliders must be set to proceed.
7. **View Your Journal:**
   - See your primary thinking pattern.
   - Explore the percentage breakdown of all five tendencies.
   - Read personalized insights and reflections.
8. **Replay** – Click "Explore Again" to start a new journey with fresh reflections.

---

## 🎯 Learning Objectives

After completing the experience, you will:

- Understand your natural thinking tendencies and how they influence your decisions.
- Recognize when you lean toward analysis, emotion, overthinking, action, or balance.
- Identify what you value most when making important decisions.
- Gain awareness of your typical patterns under different conditions.
- Reflect on how you can leverage your strengths and balance your blind spots.
- Develop a vocabulary for describing your thinking style to others.

---

## 🎨 Customization

### 📝 Questions
Edit the `CHAPTER1_QUESTIONS` array to add, remove, or modify questions and options. Each option should include a `tendency` property mapping to one of the five thinking styles.

### 📋 Priority Items
Edit the `PRIORITY_ITEMS` array to change the items available for ranking in Chapter 2.

### ⏱️ Timeline Items
Edit the `TIMELINE_ITEMS` array to change the items and descriptions in Chapter 3.

### 🎨 Themes
- Modify CSS variables in the `:root` selector to adjust colors, spacing, and typography.
- The `.mode-stress` class applies dark theme variations – edit these to customize.

### 📊 Scoring Logic
- Adjust the scoring weights in the `generateJournal` function.
- Modify the `calculateScores` and `calculateTimelineScores` functions to change how tendencies are calculated.

---

## 🧠 Thinking Tendencies

| Tendency | Emoji | Description |
|----------|-------|-------------|
| **Analytical Thinker** | 📊 | Approaches the world through logic, data, and systematic thinking. Values evidence and reason. |
| **Emotional Intuitive** | 💛 | Deeply attuned to emotions – navigates life through empathy and feeling. |
| **Overthinking Loop Style** | 🔄 | Has a rich inner world and explores every angle. Sometimes gets caught in thought loops. |
| **Action-First Decision Maker** | ⚡ | Decisive and action-oriented. Trusts instincts and moves quickly to create change. |
| **Balanced Reflective Thinker** | 🌿 | Integrates both thinking and feeling. Seeks wisdom by balancing different perspectives. |

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by cognitive psychology, reflective practice, and self-discovery frameworks.
- Built as an educational tool for personal growth and self-awareness.
- Designed with a calm, exploratory aesthetic to encourage thoughtful reflection.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy exploring! 🧠**