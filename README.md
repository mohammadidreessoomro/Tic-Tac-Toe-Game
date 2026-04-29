# 🎮 3D Tic-Tac-Toe

A fully interactive **3D Tic-Tac-Toe** game built with vanilla JavaScript and Three.js. No frameworks, no build tools — just open and play.

🔗 **Live Demo:** [Play Now](https://YOUR-USERNAME.github.io/tictactoe-3d)

---

## ✨ Features

### Game Modes
- 👥 **Human vs Human** — two players on the same screen
- 🤖 **Human vs AI** — play against the computer

### AI Difficulty Levels
| Level | Strategy |
|-------|----------|
| 🟢 Easy | 100% random moves — great for beginners |
| 🟡 Medium | Wins/blocks when it can, but makes random mistakes 45% of the time |
| 🔴 Hard | Full **Minimax algorithm** with **Alpha-Beta pruning** — mathematically unbeatable |

### 3D Visuals (Three.js)
- X pieces rendered as 3D cross geometry
- O pieces rendered as 3D torus (ring)
- Smooth **scale-pop animation** when pieces spawn
- **3D win line** drawn through the winning combo
- Board stays flat — only pieces rotate in 3D space

### Controls
- 🖱️ **Click / Tap** — place your move
- 🔄 **Drag** — rotate the 3D pieces at any angle
- Works on both **mouse and touch** devices

### UI / UX
- Turn indicator with colored dots
- Status bar — "X's turn", "O wins!", "It's a draw!"
- 🤖 "Thinking..." indicator when AI is calculating
- Win cells highlight on game end
- Score tracking across games (X Wins / O Wins / Draws)
- Dark theme

---

## 🚀 How to Run Locally

No installation needed. Just open the file:

```bash
git clone https://github.com/YOUR-USERNAME/tictactoe-3d.git
cd tictactoe-3d
# open index.html in your browser
```

Or use a local server:
```bash
npx serve .
# then open http://localhost:3000
```

---

## 🌐 Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under **Source**, select `main` branch → `/ (root)`
4. Click **Save**
5. Your game will be live at:
   `https://YOUR-USERNAME.github.io/tictactoe-3d`

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| HTML5 / CSS3 | Layout, flat board grid, dark UI |
| Vanilla JavaScript | Game logic, AI, event handling |
| [Three.js r128](https://threejs.org/) | 3D piece rendering via WebGL |
| Google Fonts | Bebas Neue + DM Mono |

---

## 📁 Project Structure

```
tictactoe-3d/
├── index.html      # entire game (single file)
├── README.md       # this file
└── .gitignore      # standard ignores
```

---

## 🧠 How the AI Works

- **Easy** — picks a random empty cell every time
- **Medium** — checks for winning/blocking moves, but intentionally fails 45% of the time to stay beatable
- **Hard** — uses the **Minimax algorithm** with **Alpha-Beta pruning**:
  - O is the **maximiser** (+10 for O win)
  - X is the **minimiser** (-10 for X win)
  - Explores every possible future game state
  - Always picks the optimal move — cannot be beaten

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

Made with ❤️ using Three.js
