# Day 7 — Claude Model Selection & Reasoning Effort

> **Claude Fundamentals · 30-Day Challenge**
> Topic: Choose the right model before writing the perfect prompt

---

## What I Learned Today

Claude is not a single tool — it's a family of models, each optimized for different types of work. Today I learned that selecting the **right model + the right effort level** before prompting is just as important as writing a good prompt.

### The Three Models

| Model | Speed | Intelligence | Best For |
|-------|-------|-------------|----------|
| **Haiku 4.5** | ⚡ Fastest | Good | Quick lookups, one-liners, simple rewrites, rapid iteration |
| **Sonnet 4.6** | ⚡⚡ Balanced | Great | Most daily tasks — coding, research, explanations, summaries |
| **Opus 4.6** | 🐢 Slower | Best | Deep research, complex algorithms, system design, strategy |

### The Four Effort Levels

| Level | When to Use |
|-------|-------------|
| **Low** | Fast, simple answers — definitions, quick lookups |
| **Standard** | Default for most tasks — covers ~80% of daily use |
| **High** | When accuracy matters — tricky bugs, exam prep, assignment submissions |
| **Max** | Hardest problems only — complex algorithms, thesis-level research, architecture decisions |

---

## My Personalized Claude Strategy

**Profile:** Student · Coding + Research & Learning · Heavy User · Coding Help focus

### Recommended Primary Model: Claude Sonnet 4.6

Sonnet is the best fit because:
- It handles real coding challenges with depth and accuracy
- It explains concepts clearly for learning (not just copy-pasting)
- As a heavy user, it preserves message limits better than Opus
- It balances speed and intelligence for long daily sessions

### Recommended Default Effort: Standard

Standard covers 80% of tasks. Upgrade to High when submitting assignments or tackling tricky bugs. Reserve Max for the hardest algorithm or architecture problems.

---

## My Personalized Workflow Table

| Task | Best Model | Best Effort | Reason |
|------|-----------|-------------|--------|
| Quick syntax check / one-liner | Haiku | Low | No deep thinking needed, just speed |
| Write a function or module | Sonnet | Standard | Needs context-awareness and code quality |
| Debug a tricky bug | Sonnet | High | Accuracy matters; reasoning through edge cases |
| Understand a new concept | Sonnet | Standard | Good explanation depth without overkill |
| Research paper summary | Sonnet | Standard | Balanced depth for academic reading |
| Exam / assignment prep | Sonnet | High | Stakes are higher; thoroughness helps |
| Complex algorithm / system design | Opus | Max | Needs Claude's deepest reasoning ability |
| Code review / refactor | Sonnet | High | Careful attention to edge cases and style |
| Brainstorm project ideas | Haiku | Standard | Speed matters; creativity doesn't need max compute |
| Thesis / deep research synthesis | Opus | High | High-stakes academic output needs best reasoning |

---

## When to Use Each Model

### 🟢 Haiku
- Checking a syntax error
- Getting a quick definition
- Generating a short list or brainstorm
- Rewriting a short paragraph
- Fast iteration on tiny code snippets

### 🔵 Sonnet (Primary)
- Writing functions, classes, or modules
- Debugging most errors
- Understanding new programming concepts
- Summarizing research papers
- Explaining assignments or problems
- Code reviews and refactoring
- Most daily study and coding sessions

### 🟡 Opus
- Designing a complex system architecture
- Solving advanced algorithm challenges
- Synthesizing multiple research papers into an argument
- Planning a major project from scratch
- When Sonnet's answer isn't deep enough

---

## Biggest Mistakes to Avoid

1. **Using Opus for every task** — it's overkill for simple questions and burns through message limits fast
2. **Always using Max effort** — Standard handles 80% of tasks; save Max for when it truly matters
3. **Pasting code without context** — always tell Claude what the code is *supposed* to do
4. **Accepting the first answer blindly** — especially for bugs; ask Claude to explain its reasoning
5. **Skipping Haiku for tiny tasks** — using Sonnet for a one-word definition wastes your daily limit
6. **Not using Claude for learning** — don't just copy code; ask Claude to teach *why* the solution works

---

## Final Recommendation

> **If I could use only ONE model and ONE effort level:**
> ### Claude Sonnet 4.6 · Standard Effort
>
> As a heavy-user student focused on coding, Sonnet gives the intelligence to handle real programming challenges, explain concepts deeply, and assist with research — without burning through limits like Opus would. Standard effort covers the vast majority of daily tasks reliably and quickly. Upgrade to High or Max only when stakes are high: a tough bug, an assignment deadline, or a hard algorithm.

---

## Tools & Resources

- **Claude Counter** (Browser Extension) — monitors Claude usage, message limits, and consumption inside Claude's web interface
  - Install from: GitHub repository (search "Claude Counter extension")
  - Steps: Open repo → Follow installation → Install in browser → Open Claude.ai → Verify counter appears → Monitor usage

- **Model Selection Guide:** [claude.com/resources/tutorials/choosing-the-right-claude-model](https://claude.com/resources/tutorials/choosing-the-right-claude-model)
- **Official Docs:** [platform.claude.com/docs/en/about-claude/models/choosing-a-model](https://platform.claude.com/docs/en/about-claude/models/choosing-a-model)

---

## Key Learnings

- Model selection is a skill, not a setting — choosing the right model *before* prompting changes the quality of outputs
- Heavy users should default to Sonnet to preserve daily message capacity
- Effort level controls how much Claude "thinks" before answering — more effort = slower but more accurate
- Claude is best used as a tutor, not just a code generator — always ask *why*, not just *what*
- Haiku is underrated for quick, repetitive tasks during study sessions

---

## Task Checklist

- [x] Read the provided resources on model selection
- [x] Opened Claude and used the Claude Usage Strategy prompt
- [x] Answered the profile questions (Student · Coding · Heavy User · Coding Help)
- [x] Generated personalized Claude strategy
- [x] Documented strategy and key learnings
- [ ] Take screenshots of the generated workflow
- [ ] Create Day7 folder in GitHub repository
- [ ] Create `day7.md` file and paste this content
- [ ] Commit and push changes
- [ ] Submit GitHub commit URL

---

*Day 7 of 30 · Claude Fundamentals Challenge*
