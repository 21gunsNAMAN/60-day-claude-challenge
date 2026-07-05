# 🧩 Prompt Puzzle — Master AI Prompting Through Play

**Day 35 Challenge** – An interactive, gamified learning experience that teaches prompt engineering through three distinct challenge types. Build, clean, and choose the best prompts across multiple domains while earning scores and receiving personalized feedback.

![Prompt Puzzle Preview](https://via.placeholder.com/800x400?text=Prompt+Puzzle+Master+AI+Prompting+Through+Play)

---

## 🚀 Live Demo

Simply open the `index.html` file in any modern browser. No server, no installation, no data sent anywhere – everything runs locally.

---

## ✨ Features

### 🎯 Two-Question Setup

Before the game starts, you answer two questions:

1. **Which domain would you like to practice prompting for?**
   - ✍️ Creative Writing
   - 📊 Business & Strategy
   - 💻 Technology & Code
   - 📚 Education & Learning
   - 💚 Health & Wellness
   - ⚖️ Legal & Compliance

2. **Choose your difficulty**
   - 🌱 Beginner – Gentle introduction
   - 🚀 Intermediate – Real-world challenges
   - 🧠 Advanced – Expert-level prompts

### 🧩 Three Challenge Types

Each scenario includes all three challenge types:

| Challenge | Description | What You Learn |
|-----------|-------------|----------------|
| **Build the Prompt** | Drag correct blocks into place to construct an effective prompt | Structure, essential elements, what to include |
| **Clean the Prompt** | Identify issues in a weak prompt and see the optimized version | Common mistakes, how to improve |
| **Choose the Best Prompt** | Select the most effective prompt from three options | Quality assessment, balance, trade-offs |

### 📊 Live Scoring

Your performance is tracked in real-time with:

- **Accuracy** – How many challenges you got right
- **Time** – How quickly you complete challenges
- **Moves** – Number of drag-and-drop actions
- **Wrong Placements** – Incorrect selections
- **Hints Used** – Number of hints requested
- **Optimization Bonus** – Bonus points for efficient play

### 📋 Prompt Performance Report

After completing all challenges, you receive:

- **Prompt Score** – Overall percentage
- **Rating & Rank** – Expert, Proficient, Competent, Developing, or Beginner
- **Prompt DNA Visualization** – 5-dimension chart (Specificity, Context, Clarity, Structure, Creativity)
- **Personalized Feedback** – Tailored to your performance
- **Next Milestone** – What to focus on next
- **Final Optimized Prompt** – A reference prompt you can use

### 🎨 Premium UI

- **Dark modern theme** with purple accents
- **Drag-and-drop** interactivity
- **Floating notifications** for feedback
- **Score animations** and micro-interactions
- **Hover effects** and smooth transitions
- **Progress indicators** showing your advancement

---

## 🛠️ Technical Stack

| Area | Technology |
|------|------------|
| Framework | React 18 (via CDN) + Babel Standalone JSX |
| Styling | Pure Vanilla CSS (no frameworks) |
| Logic | Vanilla JavaScript with React hooks |
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
2. **Select** your domain from the six options.
3. **Choose** your difficulty level (Beginner, Intermediate, or Advanced).
4. **Click** "Start Puzzle" to begin.
5. **Complete** all three challenge types for each scenario:
   - **Build** – Drag the correct blocks to construct the prompt.
   - **Clean** – Identify issues in the weak prompt.
   - **Choose** – Select the best prompt from three options.
6. **View** your live scores updating in real-time.
7. **Receive** your Prompt Performance Report after completing all challenges.
8. **Replay** with new randomized scenarios.

---

## 🎯 Learning Objectives

After playing, you will understand:

- **Prompt Structure** – What elements make an effective prompt
- **Specificity** – Why vague prompts yield vague results
- **Context** – How to provide relevant background information
- **Clarity** – How to write clear, unambiguous instructions
- **Balance** – When to use detail vs. when to keep it simple
- **Common Mistakes** – What to avoid in prompt writing
- **Optimization** – How to refine and improve prompts

---

## 📚 Sample Scenarios

The game generates 6–8 randomized scenarios per domain. Each scenario includes:

- **Desired Output** – What the prompt should generate
- **Correct Prompt Blocks** – Essential elements to include
- **Distractor Blocks** – Irrelevant or misleading elements
- **Weak Prompt** – A poorly written prompt
- **Optimized Prompt** – A well-crafted prompt
- **Over-Engineered Prompt** – A prompt that's too complex
- **Weak AI Output** – What a weak prompt produces
- **Optimized AI Output** – What a great prompt produces
- **Prompt Principle** – The key lesson for that scenario

---

## 🎨 Customization

### 📝 Domains
Edit the `DOMAINS` array to add, remove, or modify domains.

### 📊 Difficulties
Edit the `DIFFICULTIES` array to change difficulty levels.

### 📚 Scenarios
Edit the `generateScenarios` function to add new scenarios, modify existing ones, or change the number of scenarios generated.

### 🎯 Scoring
Modify the scoring logic in the challenge handlers to adjust how points are awarded.

### 🧬 DNA Visualization
Adjust the DNA dimensions in the report generation to change what's visualized.

---

## 📝 License

MIT License – feel free to use, modify, and distribute for personal, educational, or commercial purposes.

---

## 🙌 Acknowledgements

- Inspired by prompt engineering best practices and educational game design.
- Built as an interactive learning tool for anyone who wants to communicate more effectively with AI.
- Designed with a premium gaming aesthetic for an engaging learning experience.

---

## 📬 Feedback

If you have suggestions, improvements, or find a bug, please open an issue or reach out. Contributions are welcome!

---

**Happy prompting! 🧩**