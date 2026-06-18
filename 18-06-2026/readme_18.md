# Day 18 – Brain-Dump-Action-Planner 🧠

A self‑contained, interactive HTML dashboard that transforms messy meeting transcripts, voice memos, brainstorming sessions, and stream‑of‑consciousness notes into a structured, modern action plan. Built with a clean, Notion‑style interface, this tool helps you surface decisions, track tasks, and resolve conflicts—without ever inventing or inferring missing data.

## 📝 Overview

The **Brain-Dump-Action-Planner** takes raw, unstructured input and organizes it into clear sections:
- **Summary** – High‑level overview of the source material.
- **Key Takeaways** – Important highlights presented as visual cards.
- **Action Items** – Sortable table with tasks, owners, deadlines, and status badges.
- **Open Questions** – Unresolved topics and pending decisions.
- **Risks / Blockers** – Dependencies, risks, and concerns that could impact delivery.
- **Conflicts** – Conflicting deadlines, owners, decisions, or information.
- **Additional Notes** – Supporting context, with collapsible sections for long transcripts.
- **Source Information (Merge Mode)** – Merged sources, duplicate items, and conflict resolution reviews.

## ✨ Features

- **📊 Modern Dashboard UI** – Responsive cards, soft shadows, hover effects, and a clean typographic hierarchy inspired by Notion, Linear, and Asana.
- **🏷️ Status Badges** – Visual indicators for priority, completion, conflicts, and open questions (see legend below).
- **📋 Interactive Action Table** – Clearly displays task ownership, deadlines, and current status.
- **📂 Collapsible Sections** – Keeps long raw notes out of the way until you need them.
- **🔗 Merge Mode Support** – Detects duplicate items, highlights conflicts, and preserves source attribution without automatically resolving anything.
- **🔒 Data Integrity** – Every piece of information displayed comes directly from the provided notes. Missing fields are explicitly shown as `Not specified`—never invented.

## 🎨 Status Badges

| Badge | Meaning |
| :--- | :--- |
| 🔴 High Priority | Urgent task that requires immediate attention |
| 🟠 Medium Priority | Important but not immediately blocking |
| 🟢 Low Priority | Can be scheduled for later |
| ⚠️ Conflict | Conflicting deadlines, owners, or decisions |
| ❓ Open Question | Unresolved topic needing clarification |
| ✅ Completed | Task finished |
| ⏳ Pending | Awaiting action or dependencies |
| 🔄 In Progress | Currently being worked on |

## 🚀 How to Use

1. **Save the artifact** – Copy the complete HTML output into a new file (e.g., `index.html`).
2. **Open in your browser** – Double‑click the file to launch the dashboard.
3. **Interact** – Click the **“Show raw meeting notes”** toggle to expand or collapse supporting text. All tables and cards are fully static but visually scannable.
4. **Adapt the data** – Replace the example meeting notes, tasks, and owner names with your own content. The layout automatically adjusts to the information you provide.

## 🗂️ Required Sections Covered

The dashboard strictly adheres to the output requirements:

- [x] Summary
- [x] Key Takeaways (cards)
- [x] Action Items (interactive table with Task, Owner, Deadline, Status)
- [x] Open Questions
- [x] Risks / Blockers
- [x] Conflicts
- [x] Additional Notes (with collapsible long notes)
- [x] Source Information (Merge Mode only – duplicates & conflicts)

## 🖥️ Technologies

- **Pure HTML5** – Semantic structure.
- **CSS3** – Custom properties, flexbox, grid, animations, and responsive breakpoints.
- **Vanilla JavaScript** – Only used for the collapsible toggle and a small auto‑open on load; no external libraries or frameworks.

## 📌 Notes on Data Integrity

> **Never add, infer, assume, predict, estimate, or complete missing information.**

This tool is designed to be an **honest mirror** of your raw input. If a deadline, owner, or answer isn’t present in the source, the dashboard clearly displays `Not specified`. It preserves all names, dates, numbers, and terminology exactly as provided—making it ideal for accurate project kickoffs, retrospective reviews, and client handoffs.

## 📅 Challenge Progress

This is **Day 18** of a 30‑day build challenge. The focus was on creating a highly reusable, visually polished, and data‑faithful tool that bridges the gap between free‑form thinking and structured execution.

---

*Made with ❤️ for better clarity and action.*