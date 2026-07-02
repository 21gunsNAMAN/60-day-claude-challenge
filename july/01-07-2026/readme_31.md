# 📡 AI Supply Chain Control Tower

**Day 31 Challenge** – An interactive operations simulation where you step into the role of Head of Operations, managing real-time supply chain alerts to maximize business performance before time runs out.

![AI Supply Chain Control Tower Preview](https://via.placeholder.com/800x400?text=AI+Supply+Chain+Control+Tower)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🎮 Core Gameplay

- **Real-Time Alert Management**: A stream of operational alerts appears randomly. Each alert has a priority level, description, time limit, and business impact.
- **Strategic Decision-Making**: Choose the best action for each alert from 2-4 options. Every decision affects your business KPIs.
- **Live KPI Dashboard**: Seven key metrics update instantly as you make decisions.
- **3-Minute Challenge**: The game lasts 180 seconds. Alert frequency increases as time progresses.
- **Multiple Active Alerts**: Handle several alerts simultaneously – just like a real control room.

### 📊 Key Performance Indicators (KPIs)

| KPI | Description | Display |
|-----|-------------|---------|
| **Service Level** | Order fulfillment reliability | Percentage |
| **Customer Satisfaction** | Customer happiness score | Percentage |
| **Inventory Health** | Stock availability and turnover | Percentage |
| **Transportation Efficiency** | Logistics performance | Percentage |
| **Operating Cost** | Total operational expenses | Currency ($M/$B) |
| **Revenue Protected** | Revenue safeguarded from disruptions | Currency ($M/$B) |
| **Score** | Overall performance | Points (0-200+) |

### 🚨 Alert Types (10+ Random Scenarios)

| Alert | Priority | Description |
|-------|----------|-------------|
| Port Congestion | Critical | Major port backlog causing shipping delays |
| Supplier Delay | High | Key supplier missed shipment deadline |
| Truck Breakdown | High | Delivery truck broke down en route |
| Warehouse Stockout | Critical | Critical inventory level detected |
| Customs Inspection | Medium | Random customs inspection holding shipment |
| Demand Spike | High | Unexpected surge in customer orders |
| Machine Failure | Critical | Production machine offline |
| Weather Disruption | High | Severe weather affecting logistics routes |
| Inventory Count Error | Medium | System shows inaccurate inventory levels |
| Damaged Shipment | High | Shipment arrived with damaged goods |

### 🎯 Player Actions

Each alert provides action buttons such as:

- **Expedite Shipment**
- **Use Backup Supplier**
- **Reroute Trucks**
- **Increase Production**
- **Transfer Inventory**
- **Approve Air Freight**
- **Ignore**
- **Delay Decision**

### ⏱️ Game Mechanics

- **Time Pressure**: 3-minute countdown with visual warnings at 60s and 30s.
- **Increasing Difficulty**: Alert frequency increases as time progresses.
- **Delayed Consequences**: Some decisions trigger consequences after several seconds.
- **Priority System**: Critical alerts have red borders and pulse animation.
- **Score System**: Points awarded for correct decisions, penalties for wrong ones.

### 🎨 Visual Design

- **Premium Dark Theme**: Enterprise-grade operations control center aesthetic.
- **Animated KPI Cards**: Glowing effects and color-coded performance indicators.
- **Live Scrolling Event Log**: Real-time log of all decisions and events.
- **Priority Color Coding**:
  - 🔴 Critical (Red)
  - 🟠 High (Orange)
  - 🔵 Medium (Cyan)
  - ⚪ Low (Gray)
- **Pulse Animation**: Critical alerts pulse to draw attention.
- **Responsive Layout**: Works on desktop, tablet, and mobile.

### 🛠️ Additional Features

- **Pause Button**: Pause the game at any time.
- **Help/Instructions Modal**: In-game guidance.
- **Sound Toggle**: Visual-only toggle (no audio required).
- **End-of-Game Summary**: Final score, grade, KPI values, and operational summary.
- **Play Again Button**: Restart with fresh randomized alerts.

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Structure | HTML5 |
| Styling | Custom CSS (vanilla, no frameworks) |
| Logic | Vanilla JavaScript (ES6) |
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
2. **Review** your KPIs at the top – these are your performance metrics.
3. **Watch** the alert feed – new alerts will appear automatically.
4. **Read** each alert carefully – understand the priority, description, and business impact.
5. **Choose** an action for each alert – click one of the action buttons.
   - ✅ **Best** actions (green) give the highest score and KPI improvement.
   - 👍 **Good** actions (cyan) give moderate benefits.
   - ⚠️ **Warn** actions (orange) may have negative consequences.
   - ❌ **Danger** actions (red) will hurt your performance.
6. **Monitor** your KPIs – they update live based on your decisions.
7. **Manage** multiple alerts simultaneously – don't let them expire!
8. **Survive** the 3-minute shift – alert frequency increases over time.
9. **View** your final performance summary when time runs out.
10. **Click** "Play Again" to start a new session.

---

## 🎯 Learning Objectives

After playing, you will understand:

- How to prioritize under time pressure.
- The trade-offs between different operational decisions.
- How supply chain disruptions impact business metrics.
- The importance of balancing cost, speed, and customer satisfaction.
- How to manage multiple issues simultaneously.
- Real-world supply chain challenges and responses.

---

## 🎨 Customization

### 📝 Alert Types
Edit the `ALERT_TYPES` array to add, remove, or modify alert scenarios.

### ⚖️ KPI Settings
Adjust the initial KPI values in the `state.kpis` object.

### ⏱️ Game Duration
Modify `state.maxTime` (in seconds) to change game length.

### 📊 Alert Spawn Rate
Adjust `state.baseSpawnInterval` (in seconds) to control alert frequency.

### 🎯 Scoring Weights
Modify the `score` values in alert actions to change scoring balance.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by real‑world supply chain operations and control room dashboards.
- Built as an educational tool for operations management, supply chain professionals, and anyone interested in decision‑making under pressure.
- Designed with premium enterprise aesthetic for an immersive experience.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy operations commanding! 📡**