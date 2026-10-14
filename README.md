# 🎰 Sycuan Casino — Lucky Reels

A neon-styled, fully playable **3×3 fruit slot machine** that runs entirely in the browser. Single self-contained HTML file — no build step, no dependencies, no server required.

![Status](https://img.shields.io/badge/status-playable-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Dependencies](https://img.shields.io/badge/dependencies-none-success)

---

## 🎮 Play

**Live demo:** _add your GitHub Pages URL here after deploying, e.g._ `https://<your-username>.github.io/<repo-name>/`

Or just open `index.html` in any modern browser.

### How to play

| Control | Action |
| --- | --- |
| **SPIN** (or press `Space`) | Spin the three reels |
| **BET − / BET +** | Change the bet per line (1 → 100) |
| **LINES** | Toggle active paylines (1 → 5) |
| **MAX BET** | Jump to the highest bet and all 5 lines |
| **⟳ Auto** | Toggle auto-spin |
| **🔊 Sound** | Toggle sound effects |
| **RESTART** (or press `R`) | Reset to 1,000 credits |

### Rules

- You start with **1,000 credits**.
- **5 paylines**: 3 rows + 2 diagonals. Match **3 identical symbols** on a line to win.
- Payout = **bet per line × symbol multiplier** (Cherry 3× up to Diamond 50×).
- **💎 Scatter bonus**: land 3+ diamonds anywhere for an extra payout.
- **Win condition**: grow your credit balance. **Lose condition**: run out of credits — an "Out of Credits" screen appears with your stats and a **Play Again** button.

---

## 🚀 Run locally

No tooling needed. Pick whichever you prefer:

**Option A — just open it**

```bash
# macOS
open index.html
# Windows
start index.html
# Linux
xdg-open index.html
```

**Option B — serve it (recommended, avoids any file:// quirks)**

```bash
# Python 3
python3 -m http.server 8000
# then visit http://localhost:8000
```

```bash
# or Node.js
npx serve .
```

---

## 🌐 Deploy to GitHub Pages (step by step)

1. **Create a new repository** on GitHub (e.g. `sycuan-casino-slots`). Leave it empty — do **not** add a README, .gitignore, or license, since this bundle already includes them.

2. **Push this bundle** from your machine (see the exact commands in the section below).

3. **Enable GitHub Pages:**
   - Open your repo on GitHub.
   - Go to **Settings → Pages** (left sidebar).
   - Under **Build and deployment → Source**, choose **Deploy from a branch**.
   - Set **Branch** to `main` and the folder to **`/ (root)`**.
   - Click **Save**.

4. **Wait ~1 minute**, then refresh the Pages settings page. Your site will be live at:

   ```
   https://<your-username>.github.io/<repo-name>/
   ```

   Because the game is `index.html` at the repo root, it loads automatically — no extra configuration.

5. *(Optional)* Add a custom domain under **Settings → Pages → Custom domain**.

> **Tip:** Every time you push to `main`, GitHub Pages redeploys automatically.

---

## 📁 Project structure

```
.
├── index.html    # The entire game (HTML + CSS + JS, self-contained)
├── README.md     # This file
├── LICENSE       # MIT
└── .gitignore    # Common junk files
```

---

## 🛠️ Tech

- Vanilla **HTML + CSS + JavaScript** — zero frameworks, zero dependencies.
- **Web Audio API** for spin/win/lose sound effects (only starts after your first interaction, per browser autoplay rules).
- Fully responsive; works on desktop and mobile.

---

## ⚠️ Disclaimer

This is a **demo game for entertainment only**. It uses virtual credits and involves **no real money, no wagering, and no prizes**. It is not a gambling product and is not intended to simulate or encourage real-money gambling.

---

## 📄 License

Released under the [MIT License](LICENSE).
