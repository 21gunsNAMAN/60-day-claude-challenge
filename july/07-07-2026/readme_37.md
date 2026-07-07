# 🧭 Task Compass — Learn How Work Flows Through Real Organizations

**Day 37 Challenge** – An interactive management simulation that teaches ownership, delegation, collaboration, and escalation through realistic workplace scenarios. Instead of testing job titles, it teaches how work actually moves through organizations.

![Task Compass Preview](https://via.placeholder.com/800x400?text=Task+Compass+Learn+How+Work+Flows)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🎯 Choose Your Workplace

Before starting, you select the type of organization you'd like to explore:

- 💻 Tech Company
- 🚀 Startup
- 🏢 Corporate Office
- 🏥 Hospital / Healthcare
- 🛍️ Retail Business
- 🏭 Manufacturing
- 🎬 Media / Creative Agency
- 💼 Freelancer / Small Business
- 📌 Other (custom)

### 🎮 Three Progressive Stages

| Stage | Name | Description | # Questions |
|-------|------|-------------|-------------|
| 1 | **Who Owns This?** | Drag one role into the ownership slot for a realistic task. Learn who owns it, why, and who assists. | 3 |
| 2 | **Task Routing** | Build the correct workflow by dragging roles into order. Watch the task flow through the organization. | 3 |
| 3 | **Collaboration Challenge** | Assign up to 4 departments that need to collaborate on complex problems. Learn about teamwork. | 3 |

### 📚 What You Learn

- **Ownership** – Who has the knowledge, authority, and accountability to resolve issues
- **Delegation** – How work flows through an organization, step by step
- **Collaboration** – Which teams need to work together to solve complex problems
- **Workflow Thinking** – How to build efficient, value-adding processes

### 📊 Final Results & Reflection

After completing all stages, you receive:

- **Percentage Scores** – Ownership, Delegation, Collaboration, and Workflow Thinking
- **Radar Chart** – Visual representation of your strengths
- **Personalized Reflection** – What you understood well, where you over-assigned, where you underestimated collaboration, and one key insight about how organizations work
- **Confetti Celebration** – Satisfying completion animation

### 🎨 Premium Design

- **Dark Mode** – Modern, eye-friendly dark theme
- **Glassmorphism** – Elegant glass-like cards and panels
- **Drag-and-Drop** – Native drag-and-drop with touch fallback
- **Smooth Animations** – Fade-in, slide-up, and snap animations
- **Progress Indicators** – Step dots and progress bars
- **Responsive Layout** – Works on desktop, tablet, and mobile
- **Keyboard Accessibility** – Full keyboard navigation support
- **Hover Effects** – Interactive feedback on all elements

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
2. **Choose** your workplace type from the options.
3. **Click** "Start Exploration" to begin.

### Stage 1 – Who Owns This?
1. Read the task description.
2. Drag one role card into the ownership slot.
3. Click "Submit" to see the answer.
4. Read the explanation – primary owner, why they own it, and assisting roles.
5. Progress to the next question.

### Stage 2 – Task Routing
1. Read the task description.
2. Drag available steps into the routing zone in the correct order.
3. Use the arrows to visualize the flow.
4. Click "Submit" to see the correct workflow.
5. Read the explanation of why this order is commonly used.

### Stage 3 – Collaboration Challenge
1. Read the complex situation.
2. Select up to 4 departments that need to collaborate.
3. Click "Submit" to see the answer.
4. Read the reasoning, primary owner, supporting teams, and communication flow.

### Final Reflection
1. View your percentage scores across four dimensions.
2. Explore the radar chart visualization.
3. Read your personalized reflection.
4. Click "Explore Again" to replay with new scenarios.

---

## 🎯 Learning Objectives

After completing the experience, you will understand:

- How to identify the **primary owner** of a task in different organizational contexts
- Why certain roles are the right owners based on **knowledge, authority, and accountability**
- How work **flows through organizations** step by step
- Why **workflow order matters** – each step adds value
- Which **teams need to collaborate** on complex problems
- How to build efficient **communication flows** between teams
- The difference between **ownership, delegation, and collaboration**
- How **real organizations** actually function

---

## 🎨 Customization

### 📝 Scenarios
Edit the `SCENARIOS` object to add, remove, or modify workplace types and their scenarios. Each scenario includes:
- `stage1` – Ownership questions with roles, correct answer, assisting roles, and explanation
- `stage2` – Routing questions with steps, correct order, and explanation
- `stage3` – Collaboration questions with departments, correct teams, primary owner, supporting teams, reasoning, and communication flow

### 🎨 Workplace Types
Add new workplace types to the `workplaceOptions` array in the `renderWelcome` function.

### 📊 Scoring
Modify the scoring logic in the `renderResults` function to adjust how scores are calculated and displayed.

### 🎯 Radar Chart
Adjust the `radarData` array in the `renderResults` function to change the dimensions displayed.

---

## 🧠 Example Scenarios

### Stage 1 – Who Owns This?
> **Task:** "A customer reports that payments fail only on iPhones."
> 
> **Correct Owner:** Frontend Developer
> 
> **Why:** The Frontend Developer owns the iOS payment flow. They understand the client-side code, the payment SDK integration, and the specific conditions that affect iPhone users.
> 
> **Assisting:** QA Engineer, Backend Developer

### Stage 2 – Task Routing
> **Task:** "A customer reports a bug where the dashboard shows incorrect data."
> 
> **Correct Workflow:** Customer Support → QA Engineer → Backend Developer → Product Manager → Customer
> 
> **Why:** Support triages and escalates. QA reproduces and documents the bug. Backend investigates the data issue. Product Manager prioritizes the fix. The solution is communicated back to the customer.

### Stage 3 – Collaboration Challenge
> **Task:** "Customer satisfaction scores have dropped 15% over the past month."
> 
> **Teams:** Customer Support, Product Management, Engineering, Quality Assurance
> 
> **Primary Owner:** Customer Support
> 
> **Communication Flow:** Support → Product → Engineering → QA → Support (feedback loop)

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by organizational design, management theory, and real-world workplace dynamics.
- Built as an educational tool for students, new managers, and anyone curious about how organizations function.
- Designed with a premium management simulation aesthetic for an engaging learning experience.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy navigating! 🧭**