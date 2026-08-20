# 📊 Data Analyst Handbook PRO 

> **An offline-first, single-file reference, practice, examination, and sandbox environment for Data Analytics, BI, and AI Engineering.**

**193 Commands** · **60 Cross-Stack Operations** · **44-Question Adaptive Exam** · **Python/Pandas + SQL Sandbox** · **Query Builder** · **Live Charts** · **4 Languages**

---

## 🌟 Overview

**Data Analyst Handbook PRO ** is a single self-contained HTML file that works as an all-in-one environment for learning, practicing, and referencing modern data analytics tools — no install, no server, no build step.

Useful for:

- 📊 Data Analysts & BI Analysts
- 🧠 Data Scientists
- 🐍 Python / SQL developers
- 🎓 Students preparing for a Data Analyst role
- 💼 Interview candidates

Everything — the command reference, sandboxes, exam bank, and your personal progress — lives in **one `.html` file** and your browser's `localStorage`.

---

## 🔥 Features

### 📚 Command Library — 193 cards
Covers Python, NumPy, Pandas, SQL, Excel, DAX/Power BI, Data Cleaning, Statistics, and Visualization. Every card follows the same structure:

```
What it does → Why an analyst needs it → Syntax → Example → Result → Common Errors → Excel / SQL / DAX / Pandas analogues
```

Includes search (typo-tolerant), filters by module/difficulty, ⭐ favorites, and personal notes per card.

### 🔄 Cross-Stack Matrix — 60 operations
One analytical operation shown side-by-side across Python / Pandas / SQL / Excel / DAX, including a dedicated **AI Engineering** block (embeddings, RAG, vector search, agents, prompt engineering, guardrails).

### ⚖️ Compare Mode — 253 items
Pick any operation from the Matrix **or any of the 193 Library commands** and see its implementation across every tool at once, with a live search filter.

### 🧱 Query Builder
Assemble a SQL query visually (table → fields → aggregation → WHERE → sort → LIMIT) and get a matching SQL query and DAX measure generated simultaneously. One click sends the query to the SQL Sandbox to actually run it.

### 💻 In-Browser Sandbox
- **Python / Pandas** via Pyodide (WebAssembly) — real code execution
- **SQL** via sql.js (SQLite compiled to WebAssembly)
- Built-in demo tables (`orders`, `customers`) or upload your own CSV
- Engines load from CDN only when you open the Sandbox tab — the file itself stays lightweight

### 📈 Live Charts
Bar, Line, Pie, and Histogram charts rendered on plain HTML5 Canvas from the demo dataset — no charting library required.

### 🐛 Debug Mode
12 "find the bug" scenarios across Pandas, SQL, DAX, Excel, and Python, each with a revealed fix and explanation.

### 🧪 Practice Mode
Random task generator pulling from the Command Library, with the solution hidden until you're ready to check it.

### 🎓 PRO Exam
- 44 questions covering SQL, DAX, Pandas, Excel, Python, NumPy, Statistics, Visualization, Data Cleaning, and Business Analytics
- **Adaptive difficulty** — a correct answer raises the difficulty of the next question, a wrong one lowers it
- **Spaced repetition** — questions you got wrong come back more often on your next attempt
- Score, level (Junior → PRO), and history saved automatically
- 🏆 Printable certificate on completion

### 📊 Progress Dashboard
Accuracy by module, weak-topic detection, full attempt history, and one-click **export/import of your progress as JSON** (backup or move between devices).

### 🤖 Smart Search + Optional Local AI
Searches the local Library and Matrix first (with typo tolerance). If nothing is found, you can optionally query a **locally running Ollama** instance — no data ever leaves your machine, and no internet is required beyond the initial page load.

### 🔎 Command Palette
`Ctrl+K` / `⌘K` opens an instant fuzzy search across the entire Library and Matrix from anywhere in the app.

### 🌍 Multilingual
Full interface, Library content, Matrix descriptions, and Exam questions are available in:

| | |
|---|---|
| 🇬🇧 | English |
| 🇷🇺 | Russian |
| 🇩🇪 | German |
| 🇺🇦 | Ukrainian |

### 🎨 Other
- 🌙 / ☀️ Dark and light themes (with proper contrast in both)
- 🖨️ Print / export the whole handbook to PDF via the browser print dialog
- A short onboarding tour on first launch

---

## 🛠️ Technology Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 (custom properties for theming) |
| Logic | Vanilla JavaScript (ES6+), no framework |
| Python engine | Pyodide (WebAssembly), loaded on demand |
| SQL engine | sql.js (SQLite via WebAssembly), loaded on demand |
| Storage | Browser `localStorage` |
| Charts | HTML5 Canvas |
| Optional local AI | Ollama (`localhost:11434`) |

---

## 🚀 Quick Start

1. Download the `.html` file.
2. Open it in any modern browser (Chrome, Edge, Firefox, Safari).

That's it — no Python, Node.js, npm, or backend server needed for the core Handbook.

### Optional: Sandbox engines
The Python and SQL Sandboxes fetch Pyodide / sql.js from a CDN **the first time** you open them (a few MB). After that first load in a session, everything runs locally in the browser.

### Optional: Local AI (Ollama)
To use the "Ask Ollama" fallback in Smart Search:
```bash
OLLAMA_ORIGINS="*" ollama serve
```
This is required because the app is opened as a local file (`file://`), and Ollama blocks cross-origin requests by default.

---

## ⚠️ Honest Limitations

- **Not a hosted app.** There's no `git clone` / server / GitHub Pages deployment — it's a single portable HTML file you open directly.
- **Not installable as a PWA.** True "Install as App" behavior requires a `manifest.json` + Service Worker served over `http(s)`, which isn't possible from a local `file://` HTML file. If you host this file yourself (e.g. GitHub Pages, Netlify), a PWA wrapper becomes feasible as a separate addition.
- **One exam, not eight.** There is a single 44-question PRO exam pulling from all modules with adaptive difficulty — not separate per-technology exam tracks.
- Sandboxes and Ollama require internet / a local service respectively; the rest of the app works fully offline.

---

## 🗺️ Roadmap Ideas

- Grow the Library beyond 193 commands
- Expand the exam bank beyond 44 questions
- Additional real-world datasets in the Sandbox
- Gamification (streaks, badges) — intentionally left out of the current version

---

## 📄 License

MIT — see `LICENSE` for details.

---

**Learn. Practice. Debug. Examine. Build.**
One analytical problem, five technologies, one file.
