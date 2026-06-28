# 🏥 Hospital Admission Readiness Simulator

**Day 28 Challenge** – A task‑first, interactive simulation where you play the role of a Hospital Admission Coordinator, managing prior authorization, clinical documentation, bed assignment, and care coordination to determine if a patient is ready for admission.

![Hospital Admission Readiness Simulator Preview](https://via.placeholder.com/800x400?text=Hospital+Admission+Readiness+Simulator)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 📋 Setup & Case Configuration
- **Provider & Attending Physician** – Enter facility and doctor names.
- **Diagnosis Selection** – Choose from: Acute MI, CHF, Pneumonia, Elective Surgery, Hip Fracture.
- **Admission Type** – Inpatient, Observation, Emergency, ICU, Same‑Day Surgery.
- **PA Status** – Approved, Pending, or Denied.
- **Admission Date** – Set the date of admission.
- **Dynamic Hints** – Context‑aware guidance (e.g., InterQual/Milliman criteria for Acute MI/CHF, CMS 2‑Midnight Rule for Observation).

### 🏥 Admission Readiness Analysis
- **Readiness Score** (30–60% initial) with weighted scoring:
  - PA Status: 25%
  - Clinical Documentation: 20%
  - Physician Orders: 20%
  - Insurance: 15%
  - Consent: 10%
  - Bed Assignment: 10%
- **Status Grid** – Six key areas with individual scores and status indicators.
- **Denied PA + ICU** – Cannot reach 70% from admin tasks alone.

### 📋 Prior Authorization Branch Logic
- **Approved** → Continue with admission workflow.
- **Pending** → Actions: Follow Up, Upload Docs, Contact Physician.
- **Denied** → Actions: Review Reason, Contact Insurance, Submit Appeal.
- **Appeal Outcome** – 60% chance of successful appeal converting to Approved.

### ⚙️ Workflow Actions
Complete seven essential tasks:
- Assign Bed
- Verify Insurance
- Upload Documentation
- Complete Consent
- Contact Physician
- Notify Nursing
- Prepare Patient Arrival

### 📅 Timeline Milestones
Track progress through nine milestones:
1. PA Review
2. Insurance Verification
3. Bed Assignment
4. Documentation
5. Consent
6. Patient Arrival
7. Registration
8. Clinical Assessment
9. Admission Complete

### 👥 Care Coordination Team
Five care team members with dynamic status:
- Attending Physician
- Case Manager
- Nursing
- Utilization Review (with InterQual/Milliman focus)
- Discharge Planner

### 📊 Risk Tracking
Four risk categories with visual bars:
- Documentation Risk
- Insurance Risk
- Bed Risk
- Clinical Risk (weighted higher for Acute MI, CHF, ICU)

### 📈 Governance Snapshot (≥75% Readiness)
Industry benchmarks (illustrative estimates):
- PA turnaround: 3–5 days
- Inpatient denial rate: ~8–10% (CMS)
- PA rework cost: ~$11/transaction (CAQH)

### 🎯 Final Decision
- **≥ 90%** → ✅ **Admit** – Full summary with all criteria met.
- **< 90%** → ⚠️ **Not Ready** – Missing items, required actions, remaining risks.

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Structure | HTML5 |
| Styling | Tailwind CSS (CDN) + Custom CSS |
| Logic | Vanilla JavaScript (ES6) |
| Data | All state managed in JavaScript memory |
| Styling | Healthcare design system with blues and clean typography |

---

## 📂 Project Structure

```
index.html          # Single self‑contained file
```

No other files or dependencies – everything is in one file for maximum portability.

---

## 🧑‍💻 How to Use

1. **Open** `index.html` in your browser.
2. **Configure** the case:
   - Enter Provider and Attending Physician.
   - Select Diagnosis, Admission Type, PA Status, and Admission Date.
   - Review the dynamic hints that appear based on your selections.
3. **Click** 🏥 **Analyze Admission Readiness**.
4. **Review** the initial analysis:
   - Readiness Score (30–60%).
   - Status grid with individual scores.
   - PA Branch actions.
   - Workflow actions.
   - Timeline milestones.
   - Care team status.
   - Risk tracking.
5. **Take action**:
   - Complete PA branch tasks (if Pending or Denied).
   - Complete workflow actions (Assign Bed, Verify Insurance, etc.).
   - Watch your Readiness Score improve.
6. **Reach** the final decision:
   - **≥ 90%** → ✅ Admit with full summary.
   - **< 90%** → ⚠️ Not Ready with missing items list.
7. **Reset** anytime using the "New Case" button.

---

## 📚 Educational Content

### Key Concepts Explained
- **Prior Authorization** – Approval process for medical services.
- **InterQual/Milliman** – Evidence‑based clinical criteria used by Utilization Review.
- **CMS 2‑Midnight Rule** – Determines if a hospital stay should be inpatient or observation.
- **MOON (Medicare Outpatient Observation Notice)** – Required for Medicare patients under Observation status.
- **Step Therapy** – Trying lower‑cost alternatives before higher‑cost treatments.
- **Denial ≠ Permanent** – Denials can be appealed and resolved.

### System Perspectives
- How PA denials impact hospital operations.
- The role of Utilization Review in concurrent review and denial risk identification.
- How health systems track denial rates, appeal rates, and resolution times.

---

## 🎯 Learning Objectives

After completing the simulator, users will understand:

1. The end‑to‑end hospital admission readiness workflow.
2. How prior authorization status impacts admission readiness.
3. The importance of documentation, insurance verification, and bed assignment.
4. How to escalate pending or denied PAs through appeals.
5. The role of care coordination in admission readiness.
6. How risks (documentation, insurance, bed, clinical) affect readiness.
7. The governance and benchmarks used in healthcare operations.

---

## 🎨 Customization

### 📝 Scenario Data
Modify the `DIAGNOSES`, `ADMISSION_TYPES`, or `PA_STATUSES` arrays.

### ⚖️ Scoring Weights
Adjust the `weights` object in the `calculateScore()` function:
```javascript
const weights = {
    pa: 0.25,
    documentation: 0.20,
    orders: 0.20,
    insurance: 0.15,
    consent: 0.10,
    bed: 0.10
};
```

### 📊 Risk Thresholds
Modify the `getRiskLevel()` function to change risk classification.

### 🎯 Final Decision Thresholds
Adjust the score thresholds in `renderFinalDecision()`:
- `>= 90` → Admit
- `< 90` → Not Ready

### 🏥 Care Team
Edit the `CARE_TEAM` array to add or modify roles.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by real‑world hospital admission processes and prior authorization workflows.
- Built as an educational tool for healthcare administrators, students, and professionals.
- Data sources: CMS, CAQH, AMA, and industry benchmarks (illustrative estimates).

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy coordinating! 🏥**