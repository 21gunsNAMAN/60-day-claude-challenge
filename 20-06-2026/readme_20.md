Here's a complete README.md file for your Face Puzzle game project. It covers all the features, setup instructions, and technical details – perfect for a "Day 20" milestone or any portfolio showcase.

```markdown
# 🧩 Face Puzzle – Day 20

A complete, self-contained face-puzzle game that turns your webcam snapshot into a draggable, sliding-tile challenge.  
Built with vanilla HTML, CSS, and JavaScript – no frameworks, no external dependencies (except CDN-hosted polyfills, if needed).

![Face Puzzle Demo](https://via.placeholder.com/640x400?text=Face+Puzzle+Preview)

---

## ✨ Features

- 📸 **Camera Access**  
  Requests webcam permission via `getUserMedia()` and shows a live preview. A **"Take Photo"** button snaps a square crop of your face.

- 🧩 **Puzzle Generation**  
  Choose difficulty: **3×3**, **4×4**, or **5×5** grid.  
  The captured image is sliced into equal tiles, scrambled randomly (with guaranteed solvability), and rendered as draggable pieces.

- 🖱️ **Drag & Touch Gestures**  
  Supports both mouse (desktop) and touch (mobile/tablet) events.  
  - Drag a piece onto another to swap their positions.  
  - Pieces snap to the nearest grid cell on release.  
  - Dragged piece gets a highlighted border; correctly placed pieces get a green border.

- ⏱️ **Timer & Move Counter**  
  Timer starts on the first drag and displays elapsed time in `mm:ss.t` format.  
  Total moves are counted, and a live progress indicator shows `correct_pieces / total_pieces`.

- 🏆 **Win Detection & Results**  
  Automatically detects when all pieces are in the correct position, stops the timer, and shows an overlay with:
  - Final time  
  - Total moves  
  - Difficulty level  
  - Top 5 best times saved to `localStorage` (with date, time, moves, and difficulty)  
  - A leaderboard of saved best times.

- 🎨 **UI & Polish**  
  Clean, modern, responsive design that works on both desktop and mobile.  
  Buttons included: **Retake Photo**, **Play Again**, **New Photo**.

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge).
- **HTTPS or localhost** – camera access requires a secure context.

### Running the Game
1. Download the single HTML file (`index.html`).
2. Open it in your browser (double-click or use a local server).
   - For the best experience, use a local dev server (e.g., VS Code Live Server, `python -m http.server`, or `npx serve`).
3. Allow camera permissions when prompted.
4. Take a photo, choose a difficulty, and start dragging pieces to solve the puzzle!

---

## 🛠️ Technical Stack

- **Language:** Vanilla JavaScript (ES6)
- **Styling:** Pure CSS3 (no preprocessors)
- **Markup:** HTML5
- **Persistence:** `localStorage` for leaderboard
- **Polyfills:** None required – works in modern browsers
- **CDN Dependencies:** None (self-contained)

---

## 📁 File Structure

```
.
└── index.html          # Complete game – all CSS, HTML, and JS in one file
```

---

## 📖 How to Play

1. **Allow camera access** – your face will appear in the video preview.
2. **Tap “Take Photo”** – the image is captured and shown.
3. **Select difficulty** – 3×3 (easy), 4×4 (medium), or 5×5 (hard).
4. **Click “Start Puzzle”** – the tiles are scrambled.
5. **Drag a tile** (mouse or touch) and drop it onto another tile to swap them.
6. The timer starts on your first drag. Keep swapping until all tiles are in their correct positions.
7. When solved, the results overlay appears with your stats and the leaderboard.
8. Use **“Play Again”** (same photo) or **“New Photo”** to restart.

---

## 🧠 Design Notes

- The puzzle is **always solvable** – the scrambling algorithm uses random swaps (not random placements) to guarantee a valid state.
- Dragged tiles have a higher `z-index` and a scale bump for better visibility.
- The leaderboard stores the **top 5** fastest times per device (globally, not per difficulty).
- The timer is accurate to 1/10th of a second and automatically pauses when the puzzle is solved.

---

## 🌐 Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome  | ✅ Full  |
| Firefox | ✅ Full  |
| Safari  | ✅ Full (macOS/iOS) |
| Edge    | ✅ Full  |

---

## 📦 Local Storage Schema

```json
[
  {
    "date": "2026-06-21T10:30:00.000Z",
    "difficulty": "4×4",
    "time": 12.5,
    "moves": 24,
    "timestamp": 1718975400000
  }
]
```

---

## 🤝 Contributing

This is a self-contained educational project. Feel free to fork and modify it for your own learning or portfolio.

---

## 📄 License

MIT – use it freely, modify it, and share it.

---

## 🙌 Day 20 – Milestone

Built as part of a 100‑day coding challenge.  
Day 20 – fully functional face puzzle with camera integration and leaderboard persistence.

---

**Enjoy the puzzle!** 🧩📸
```
