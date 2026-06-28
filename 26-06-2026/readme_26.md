# 🏥 Prior Authorization Workflow Simulator

**Day 26 Challenge** – A gamified, drag‑and‑drop simulation of the US healthcare prior authorization (PA) process. Built as a single self‑contained HTML file with vanilla JavaScript, no external dependencies.

![Prior Authorization Simulator Preview](https://via.placeholder.com/800x400?text=Prior+Authorization+Workflow+Simulator)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. All logic runs client‑side – no server, no installation, no data sent anywhere.

---

## ✨ Features

### 🧩 Core Workflow
- **Three workflow lanes**: Patient, Provider, and Payer – each with dedicated stages.
- **Drag‑and‑drop case movement**: Move the patient case card from one stage to the next by dragging it onto the highlighted drop zone.
- **Four patient scenarios**:
  - Elective Surgery (e.g., total hip replacement)
  - MRI Scan (lumbar spine)
  - Specialty Medication (e.g., Humira)
  - Inpatient Admission (acute pancreatitis)
- **Medical necessity evaluation** – learn what criteria payers use.
- **Document collection** – see the required documents for each scenario.
- **Submission to payer** – simulate the handoff.
- **Review outcomes**: Approval, Pend, Denial, Appeal, and Peer‑to‑Peer Review.

### 📚 Educational
- **Explanations after every step** – each stage includes a detailed description of what happens and why.
- **Scenario‑specific notes** – additional context for the chosen case (e.g., step therapy requirements, clinical indicators).

### 📊 Tracking & Scoring
- **Progress tracker** across the top – shows which stages are completed, active, or pending.
- **Days elapsed counter** – increments as you advance.
- **Efficiency score** – calculated based on days taken vs. expected, and workflow completeness.
- **Workflow summary** on completion – displays outcome, days, efficiency, stages completed, and scenario complexity.

### 🎉 Engagement
- **Celebration animation** with confetti on approval.
- **Keyboard shortcut**: press `Enter` to advance to the next stage (when a drop zone is active).
- **Restart / New Patient** buttons – easily reset or try a random scenario.

### 🖥️ UI & UX
- Modern, clean design using shades of blue with black text.
- Fully responsive – works on desktop, tablet, and mobile.
- Drag‑and‑drop with visual feedback (hover states, drop hints).
- Accessible and intuitive layout.

---

## 🛠️ Technical Requirements (Fulfilled)

| Requirement | Implementation |
|-------------|----------------|
| Single HTML file | ✅ All in `index.html` |
| HTML + CSS + Vanilla JS | ✅ No frameworks, no libraries |
| No external dependencies | ✅ Pure vanilla, no CDNs |
| No `localStorage` | ✅ All state in memory |
| Well‑commented code | ✅ Extensive comments throughout |
| Editable scenario data | ✅ `SCENARIOS` array near the top of the script |
| Fully functional buttons & interactions | ✅ Drag‑and‑drop, buttons, keyboard shortcuts |

---

## 📂 Project Structure

```
index.html          # Single self‑contained file
```

No other files or dependencies – everything is in one file for maximum portability.

---

## 🧑‍💻 How to Use

1. **Open** `index.html` in your browser.
2. **Select** a scenario from the dropdown (or click "New Patient" for a random one).
3. **Read** the educational panel – it explains the current stage.
4. **Drag** the case card (the blue card) from its current stage and **drop** it onto the highlighted drop zone of the next stage.
   - The drop zone is marked with a dashed border and a "Drop case here" hint.
   - You can only move to the immediate next stage – the workflow is linear.
5. **Advance** through all stages: Patient Visit → Medical Necessity → Document Collection → Submission → Payer Review → Outcome Decision.
6. **View** the final outcome, summary, and efficiency score.
7. **Celebrate** if you get an approval! 🎉
8. **Restart** or try a new scenario using the buttons.

> **Pro Tip**: Press `Enter` on your keyboard to quickly advance to the next stage (when a drop zone is active).

---

## 🎯 Scenarios & Complexity

| Scenario | Description | Complexity | Approval Likelihood | Expected Days |
|----------|-------------|------------|---------------------|---------------|
| **Elective Surgery** | Total hip replacement for osteoarthritis | High | 55% | 12 |
| **MRI Scan** | Lumbar spine MRI for chronic back pain | Medium | 78% | 7 |
| **Specialty Medication** | Humira for rheumatoid arthritis | High | 62% | 14 |
| **Inpatient Admission** | Acute pancreatitis with complications | Medium | 85% | 5 |

Each scenario includes a custom set of required documents and educational notes specific to that case.

---

## 🧠 Educational Content

Every stage provides a detailed explanation of the step, including:
- What happens during that stage.
- Why it is important.
- Key considerations (e.g., medical necessity criteria, documentation requirements).
- Scenario‑specific insights (e.g., "For specialty medications, step therapy documentation is critical").

The educational panel updates automatically as you progress, making this a valuable learning tool for healthcare students, new coordinators, or anyone interested in the PA process.

---

## 🎨 Customization

You can easily modify the scenarios, stages, or scoring logic:

- **Scenarios**: Edit the `SCENARIOS` array near the top of the `<script>` section.
- **Stages**: Edit the `STAGES` array to add, remove, or reorder workflow steps.
- **Outcome logic**: Adjust the `determineOutcome()` function to change approval probabilities or decision logic.
- **Efficiency formula**: Tweak the `calculateEfficiency()` function to change how the score is computed.
- **Styling**: Modify the CSS variables and rules at the top of the `<style>` block.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by real‑world prior authorization processes in the US healthcare system.
- Built as an educational tool to demystify the PA workflow.
- Drag‑and‑drop interactions powered by native HTML5 Drag & Drop API.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy simulating! 🏥**