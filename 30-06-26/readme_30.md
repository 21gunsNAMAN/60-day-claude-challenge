# 🚚 Supply Chain Builder

**Day 30 Challenge** – An interactive, beginner‑friendly game that teaches supply chain fundamentals through hands‑on decision‑making. Build your own supply chain, learn the trade‑offs, and see your business metrics come to life.

![Supply Chain Builder Preview](https://via.placeholder.com/800x400?text=Supply+Chain+Builder)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🏗️ Build Your Supply Chain (5 Decisions)

| Step | Decision | Options |
|------|----------|---------|
| 1 | **Number of Suppliers** | Single Supplier vs. Multiple Suppliers |
| 2 | **Factory Location** | Domestic Factory vs. Offshore Factory |
| 3 | **Warehouse Strategy** | Centralized vs. Decentralized Warehouses |
| 4 | **Transportation Method** | Road, Rail, Sea, or Air |
| 5 | **Inventory Strategy** | Low, Balanced, or High Inventory |

### 📊 Live Business Metrics

After every decision, five animated progress bars update in real time:

- **Cost** – How much money you spend
- **Delivery Speed** – How fast products reach customers
- **Risk** – Exposure to disruptions
- **Customer Satisfaction** – How happy customers are
- **Sustainability** – Environmental impact

### 🧠 Educational Design

Every decision is preceded by a plain‑language explanation:

- **📖 What this means** – Clear definition of the concept
- **💡 Why it matters** – Real‑world business impact
- **Trade‑off explained** – After each choice, you see how your decision affects the metrics

### 📊 Final Dashboard

After completing all 5 decisions, you receive:

- **Overall Supply Chain Score** (0–100)
- **Strengths & Weaknesses** – Your top and bottom performing areas
- **Biggest Risk** – Personalized risk assessment
- **3 Practical Improvements** – Actionable recommendations to improve your supply chain

### 🎨 Premium Design

- **Dark enterprise dashboard** theme
- **Fully responsive** – works on desktop, tablet, and mobile
- **Rounded cards** with smooth hover effects
- **Animated progress bars** showing metric changes in real time
- **Replay button** to start a new randomized simulation

### 🎲 Randomized Gameplay

Every playthrough is unique:
- Random company generation (name, industry, products, countries served, demand level)
- Fresh decisions and outcomes each time

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Framework | React 18 (via CDN) + Babel Standalone JSX |
| Styling | Custom CSS (no Tailwind, no external assets) |
| Logic | Vanilla JavaScript with React hooks (`useState`, `useCallback`, `useMemo`) |
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
2. **Read** the welcome screen – it explains what a supply chain is in simple language.
3. **Click** 🚀 **Start Building**.
4. **Review** your company profile – industry, products, countries, and demand level.
5. **Make** your first decision (suppliers). Read the concept and why it matters, then choose an option.
6. **See** the trade‑off explanation and watch your metrics update.
7. **Repeat** for the next 4 decisions (factory, warehouse, transportation, inventory).
8. **View** your final dashboard – overall score, strengths, weaknesses, biggest risk, and 3 improvements.
9. **Replay** to build a new supply chain with a different company.

---

## 🎯 Learning Objectives

After playing, you will understand:

- What a supply chain is and why it matters.
- The trade‑offs between cost, speed, risk, satisfaction, and sustainability.
- How supplier choice affects risk and flexibility.
- Why factory location impacts cost and delivery speed.
- The benefits and drawbacks of centralized vs. decentralized warehouses.
- How transportation methods balance speed vs. cost.
- The impact of inventory levels on customer service and cost.

---

## 🎨 Customization

### 📝 Company Generation
Edit the `generateCompany` function to change industries, product lists, countries, or demand levels.

### ⚖️ Decision Steps
Edit the `STEPS` array to add, remove, or modify decisions and their options.

### 📊 Metrics
Adjust the `generateMetrics` function to change initial metric values.

### 🎯 Scoring Weights
Modify the weights in the `generateDashboard` function to change how the overall score is computed.

### 🎨 Styling
Edit the CSS variables and classes to customize colors, spacing, or fonts.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by real‑world supply chain management and enterprise dashboard design.
- Built as an educational tool for business students, supply chain professionals, and anyone curious about how products get from factory to customer.
- React and Babel used for component‑based UI development.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy building! 🚚**