# 📋 Prior Authorization Story Simulator

**Day 27 Challenge** – An interactive, narrative-driven educational tool that simulates a patient's journey through the prior authorization (PA) process in US healthcare. Built as a single‑file HTML app with Tailwind CSS and vanilla JavaScript.

![Prior Authorization Story Simulator Preview](https://via.placeholder.com/800x400?text=Prior+Authorization+Story+Simulator)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 👥 Characters
- **👦 Rahul** – Patient navigating the healthcare system. Appears in **left‑aligned chat bubbles**.
- **👧 Priya** – Healthcare operations specialist guiding Rahul. Appears in **right‑aligned chat bubbles**.
- **Narrators & Doctors** – Appear as **centered italic text** (never as chat bubbles) to provide context and exposition.

### 📖 8 Interactive Scenes

| Scene | Name | Description |
|-------|------|-------------|
| 1 | **Doctor Visit** | Rahul visits Dr. Patel, diagnosed with Rheumatoid Arthritis, prescribed Humira. |
| 2 | **Insurance Roadblock** | Provider submits PA directly to StarCare Health (payer). PA saved on file permanently. |
| 3 | **What is PA?** | Priya explains prior authorization in plain language. Includes AMA 2023 survey data. |
| 4 | **Insurance Review** | Priya walks through eligibility, clinical documentation, ICD‑10 match, and step therapy history. |
| 5 | **Denial** | Denied for missing step therapy documentation. Denial ≠ permanent. Includes cost impact data. |
| 6 | **Appeal** | Gather documents, Letter of Medical Necessity, formal appeal filing. |
| 7 | **Approval** | PA approved, saved on file. Reference number issued. No repeat PA needed. |
| 8 | **Takeaways** | Two perspectives: Patient (what Rahul learned) + System (denial rate, appeal rate, resolution time). |

### 🎮 Interactive Choices
- After each scene, you choose between **two response options**.
- Your choice influences the dialogue and progression.
- Creates a personalized, engaging learning experience.

### 📊 Progress Tracking
- **Progress bar** at the top shows completion percentage.
- **Scene indicator** displays current scene number.
- **Scene name** updates as you advance.

### 🎨 Design
- Clean, healthcare‑inspired design system.
- Distinct bubble styles for each character (Rahul in blue, Priya in teal).
- Centered italic text for narrators and doctors.
- Fully responsive – works on desktop, tablet, and mobile.
- Smooth animations and transitions.

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Structure | HTML5 |
| Styling | Tailwind CSS (CDN) + Custom CSS |
| Logic | Vanilla JavaScript (ES6) |
| DOM Manipulation | `createElement` + `appendChild` (never `innerHTML` on chat container) |
| Data | Scene data stored in JavaScript array |

---

## 📂 Project Structure

```
index.html          # Single self‑contained file
```

No other files or dependencies – everything is in one file for maximum portability.

---

## 🧑‍💻 How to Use

1. **Open** `index.html` in your browser.
2. **Read** the narrative text (centered italic) – it sets the scene.
3. **Read** the chat bubbles:
   - 👦 **Rahul** (left) – patient perspective.
   - 👧 **Priya** (right) – healthcare specialist guidance.
4. **Choose** your response from the two options at the bottom.
5. **Advance** through all 8 scenes.
6. **Learn** about the prior authorization process along the way.
7. **Restart** anytime using the "↻ Restart" button.

> **Pro Tip**: Take your time reading each scene – the educational content is designed to build understanding step by step.

---

## 📚 Educational Content

The simulator integrates real‑world prior authorization knowledge:

### 📊 Data & Statistics
- **AMA 2023 PA Survey**: "PA causes treatment delays in the majority of cases."
- **Industry Data**: PA denials cost physician offices 2+ staff hours per denial to resolve.
- **Benchmarks**: Average denial rate is 8–12%, with a resolution time of 3–5 days for appeals.

### 📋 Key Concepts Explained
- **Step Therapy** – Trying lower‑cost alternatives before higher‑cost treatments.
- **Medical Necessity** – Clinical justification for the requested treatment.
- **ICD‑10 Match** – Diagnosis code alignment with the treatment.
- **Appeal Process** – Gathering documentation, Letter of Medical Necessity, formal filing.
- **Denial ≠ Permanent** – Denials can be appealed and resolved.

### 🏥 System Perspective
- How health systems track **denial rates**, **appeal rates**, and **resolution times**.
- The impact of PA on **disease progression** and **patient outcomes**.
- The **collaborative nature** of the PA process between providers, payers, and patients.

---

## 🎯 Learning Objectives

After completing the simulator, users will understand:

1. What prior authorization is and why it exists.
2. The key steps in the PA workflow (Provider → PA Request → Payer).
3. What insurance reviewers look for (eligibility, documentation, ICD‑10, step therapy).
4. Why denials happen and how to appeal them.
5. The patient experience and emotional impact of the process.
6. System‑level metrics and improvement strategies.
7. The importance of documentation and communication.

---

## 🎨 Customization

You can easily modify the scenes, characters, or content:

### 📝 Scene Data
Edit the `SCENES` array in the JavaScript section:

```javascript
const SCENES = [{
    id: 'scene1',
    name: 'Your Scene Name',
    narrative: 'Your narrative text here...',
    messages: [
        { speaker: 'rahul', text: 'Rahul\'s message...' },
        { speaker: 'priya', text: 'Priya\'s message...' }
    ],
    choices: [
        { label: 'Choice 1 Label', nextSceneId: 'scene2' },
        { label: 'Choice 2 Label', nextSceneId: 'scene2' }
    ]
}];
```

### 🎨 Styling
- Modify the CSS variables at the top of the `<style>` block.
- Change colors, fonts, spacing, or animations.
- Tailwind classes are used throughout for rapid customization.

### 👥 Characters
- Add new speakers by extending the `createBubble` and `createNarrator` functions.
- Customize avatar emojis and colors.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by real‑world prior authorization processes in the US healthcare system.
- Built as an educational tool to demystify the PA workflow for patients and healthcare professionals.
- Data sources: AMA 2023 Prior Authorization Survey, industry benchmarks.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy learning! 📋**