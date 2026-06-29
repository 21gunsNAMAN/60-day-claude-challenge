# 📦 Operation Lifeline: Supply Chain Crisis Lab

**Day 29 Challenge** – An immersive, interactive supply chain crisis simulation game where you step into the role of a crisis commander. Navigate disruption, negotiate with suppliers, lead your team, and build a resilient supply chain – all in a premium dark‑themed dashboard experience.

![Operation Lifeline Preview](https://via.placeholder.com/800x400?text=Operation+Lifeline+Supply+Chain+Crisis+Lab)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🎮 Complete Game Flow (5 Phases)

| Phase | Name | Description |
|-------|------|-------------|
| 1 | **Company Profile** | A random fictional company is generated with industry, revenue, factories, warehouses, suppliers, inventory days, lead time, and countries – displayed as modern cards. |
| 2 | **Crisis Alert** | One random crisis is generated from 8 types (factory fire, supplier bankruptcy, port strike, cyberattack, flood, raw material shortage, political conflict, shipping delay) with urgency and business impact. |
| 3 | **War Room** | Choose **3 of 6** response actions. Each action dynamically updates Cost, Inventory, Profit, Delivery Speed, and Customer Satisfaction using animated progress bars. |
| 4 | **Supplier Negotiation** | Four rounds of branching negotiation. Each choice affects Trust, Price, and Lead Time. A negotiation score is tracked. |
| 5 | **CEO Boardroom** | Five multiple‑choice leadership questions. Your answers influence executive decision‑making scores. |
| 6 | **AI Strategy** | Choose **2 of 5** AI investments (Demand Forecasting, Inventory Optimization, Supplier Risk Monitoring, Warehouse Vision, Procurement Copilot). Each shows expected business impact. |

### 📊 Final Dashboard

After completing all phases, you receive:

- **Overall Crisis Score** (0–100)
- **6 Component Scores**: Leadership, Negotiation, Resilience, Cost Control, Risk Management, Customer Satisfaction
- **Personalized Feedback**: Biggest mistake, best decision, expert recommendation, and lessons learned

### 🎨 Design

- **Premium dark theme** inspired by enterprise dashboards
- **Fully responsive** – works on desktop, tablet, and mobile
- **Rounded cards** with smooth hover effects
- **Animated progress bars** showing metric changes in real time
- **Modern typography** with a clean, professional feel
- **Replay button** to start a new randomized simulation every time

### 🧠 Randomized Gameplay

Every playthrough is unique:
- Random company generation (name, industry, revenue, factories, warehouses, suppliers, inventory days, lead time, countries)
- Random crisis selection (type, urgency, impact)
- Random initial metrics and outcomes
- Dynamic consequences for every decision

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Framework | React 18 (via CDN) + Babel Standalone JSX |
| Styling | Custom CSS (no Tailwind, no external assets) |
| Logic | Vanilla JavaScript with React hooks (`useState`, `useEffect`, `useMemo`, `useCallback`, `useRef`) |
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
2. **Start** the simulation from the welcome screen.
3. **Review** your company profile – understand your assets and vulnerabilities.
4. **Face** the crisis – read the alert and understand the urgency and impact.
5. **Enter the War Room** – select **three** actions to respond to the crisis. Each action affects your metrics differently.
6. **Negotiate** with suppliers over four rounds – choose your strategy carefully to balance trust, price, and lead time.
7. **Lead** your team through five CEO boardroom questions – there are no wrong answers, but some choices build stronger resilience.
8. **Invest** in two AI capabilities – each delivers measurable business impact.
9. **Review** your final dashboard – see your overall score, component scores, personalized feedback, and expert recommendations.
10. **Replay** to face a new crisis with a new company!

---

## 🎯 Learning Objectives

After playing, you will understand:

- How supply chain disruptions impact business metrics (cost, inventory, profit, delivery, satisfaction).
- The trade‑offs involved in crisis response actions.
- How supplier relationships affect trust, pricing, and lead time.
- The importance of leadership and decision‑making in crisis situations.
- How AI investments can improve supply chain resilience.
- How to balance short‑term survival with long‑term sustainability.

---

## 🎨 Customization

### 📝 Crisis Types
Edit the `CRISIS_TYPES` array to add, remove, or modify crisis scenarios.

### ⚙️ War Room Actions
Edit the `WAR_ROOM_ACTIONS` array to change available response actions and their metric impacts.

### 🤖 AI Investments
Edit the `AI_INVESTMENTS` array to add or modify AI capabilities and their business impact.

### 🧠 CEO Questions
Edit the `CEO_QUESTIONS` array to change the leadership questions, options, and scoring.

### 🎯 Scoring Weights
Adjust the weights in the `calculateFinalScore` function to change how the overall score is computed.

### 🏢 Company Generation
Edit the `generateCompany` function to change industry lists, naming conventions, or value ranges.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by real‑world supply chain crisis management and enterprise dashboard design.
- Built as an educational tool for business students, supply chain professionals, and anyone interested in decision‑making under uncertainty.
- React and Babel used for component‑based UI development.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy crisis commanding! 📦**