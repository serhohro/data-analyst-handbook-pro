# 📊 Data Analyst Handbook PRO 

> **The ultimate interactive, offline-first reference, learning, and sandbox environment for Data Analytics & Engineering.**
> Covers Python, NumPy, Pandas, SQL, Excel, DAX, Statistics, Visualization, and AI Engineering across 4 languages (RU / EN / DE / UA).

---

## 🌟 Overview

**Data Analyst Handbook PRO** is an all-in-one, browser-based workspace designed for data analysts, analytics engineers, and data scientists. It provides an extensive command library, full cross-stack operation comparisons, interactive query builders, an in-browser live code sandbox (Python & SQL), interactive debug scenarios, adaptive testing with certificate generation, and local AI support — all packed into a clean, standalone, offline-first HTML application.

---

## 🔥 Key Features

### 📚 Command Library (193 Cards)
- **Comprehensive Coverage:** Deep dive into Python, NumPy, Pandas, SQL, Excel, DAX, Data Cleaning, Statistics, and Visualization.
- **Unified Standard Card Structure:** Every single command card is structured as:
  `What` → `Why` → `Syntax` → `Example` → `Result` → `Errors` → `Analogues in Excel / SQL / DAX / Pandas`
- **Smart UX:** Typo-tolerant instant search, multi-module filtering, and difficulty filters.
- **Personalization:** 
  - ⭐ **Favorites System:** Save frequently used commands and toggle "Show Favorites Only".
  - 📝 **Personal Notes:** Add custom notes to any card (automatically persisted in your browser).
- **Fully Multilingual:** Instant switcher across 🇷🇺 **Russian**, 🇬🇧 **English**, 🇩🇪 **German**, and 🇺🇦 **Ukrainian**.

---

### 🔄 Stack Matrix & ⚖️ Compare Mode
- **60 Operations Side-by-Side:** Compare implementations seamlessly across **Python**, **Pandas**, **SQL**, **Excel**, and **DAX**.
- **🤖 Dedicated AI Engineering Block:** Deep-dive cards & matrix entries for modern LLM stacks, including Embeddings, RAG, Autonomous Agents, Prompt Engineering, Guardrails, and Vector Search.
- **⚖️ Interactive Compare Mode:** Select any operation from a dropdown to see its exact syntactical equivalent rendered side-by-side across every tool simultaneously.
- **4-Language Descriptions:** Detailed breakdowns of each operation in all supported languages.

---

### 🧱 Query Builder
- **Visual SQL & DAX Constructor:** Build queries intuitively by selecting tables, fields, aggregations, `WHERE` conditions, sorting, and `LIMIT`.
- **Dual Output:** Simultaneously generates valid **SQL queries** and **DAX measures**.
- **⚡ Direct Sandbox Execution:** Click **"Test in Sandbox"** to instantly push your generated query into the live SQLite engine for execution.

---

### 💻 In-Browser Sandbox & 📈 Live Charts
- **Real Execution Engines (Zero Setup):**
  - **Python / Pandas:** Runs full Python code natively via **Pyodide** (WebAssembly).
  - **SQL / SQLite:** Runs relational queries locally via **sql.js**.
- **Custom Data Support:** Pre-loaded with demo dataset (`orders`, `customers`) or upload your own `.csv` files.
- **On-Demand Engine Loading:** Heavy engines load from CDN *only when you click run*, keeping the initial app lightweight.
- **📈 Native Live Charts:** Render Bar, Line, Pie, and Histogram charts directly on HTML5 Canvas without relying on bulky external visualization libraries.

---

### 🐛 Debug Mode & 🧪 Practice
- **🐛 Debug Mode:** 12 realistic "find the bug" scenarios covering Pandas, SQL, DAX, Excel, and Python errors across all 4 languages.
- **🧪 Practice Mode:** Generate randomized hands-on analytical tasks filtered by topic with hidden collapsible solutions.

---

### 📝 PRO Exam & 🏆 Certification
- **44 Adaptive Questions:** Evaluates full analytics mastery.
- **Adaptive Difficulty Engine:** Dynamically adjusts question challenge based on performance (Correct → Harder, Incorrect → Easier).
- **Spaced Repetition:** Smartly re-queues incorrectly answered questions more frequently.
- **🏆 Print / PDF Certificate:** Automatically generates a formatted completion certificate upon passing.

---

### 📊 Progress Dashboard
- Module-by-module completion tracking.
- Identifies weak topics and tracks exam attempt history.
- **Data Portability:** Full JSON **Export / Import** functionality to backup or transfer your learning progress across devices.

---

### 🤖 Local AI & ⌘K Smart Search
- **Local Database First:** Instant fuzzy matching across the entire Library and Matrix.
- **Local Ollama Integration:** Optional fallback to local Ollama LLMs with automatic CORS connection diagnosis and step-by-step setup assistance.
- **⌘K / Ctrl+K Palette:** Quick-command palette for fast, keyboard-driven navigation across the whole app.

---

## 🛠 Stack Comparison Matrix Preview

| Operation | Python | Pandas | SQL | Excel | DAX |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Aggregation** | `sum()` / `len()` | `df.groupby().agg()` | `GROUP BY` / `SUM()` | Pivot Tables / `SUMIFS` | `SUMMARIZE()` / `CALCULATE()` |
| **Filtering** | `[x for x in data if ...]` | `df.query()` / `df[...]` | `WHERE` / `HAVING` | Filter / `FILTER()` | `FILTER()` / `CALCULATE()` |
| **Joining Data** | `dict` merges / `zip` | `pd.merge()` / `join()` | `INNER / LEFT JOIN` | `XLOOKUP()` / `VLOOKUP()` | `RELATED()` / Relationships |
| **Ranking** | `sorted(key=...)` | `df['col'].rank()` | `ROW_NUMBER() OVER()` | `RANK.EQ()` | `RANKX()` |
| **Null Handling**| `None` / `math.isnan` | `df.fillna()` / `isna()` | `COALESCE()` / `IS NULL` | `IFERROR()` / `ISBLANK()`| `COALESCE()` / `ISBLANK()` |
| **AI / RAG** | `openai` / `langchain` | Vector Embeddings | Vector DB Extensions | Excel AI Formulas | Custom DAX AI Metrics |

---

## 💻 Tech Stack & Architecture

- **Frontend:** Pure Vanilla HTML5, CSS3, JavaScript (ES6+).
- **Styling:** Custom CSS with Light/Dark theme engine, high contrast palettes, and print optimization (`@media print`).
- **Wasm Engines (CDN On-Demand):** Pyodide (Python/Pandas) & sql.js (SQLite).
- **Storage:** LocalStorage API for offline persistence (Notes, Favorites, Progress, Themes).

---

## 🚀 Quick Start

1. Clone or download the repository.
2. Open `index.html` (or `Data_Analyst_Handbook_PRO.html`) in any modern browser (Chrome, Firefox, Edge, Safari).
3. **No server, npm install, or Python backend setup required!**

> ℹ️ *Note: Internet access is only required during the first click of Sandbox execution to load Pyodide/sql.js engines, or when connecting to local Ollama instances.*

---

## 📄 License & Status

- **Status:** Active Development
- **License:** MIT License

---
⭐ **If you find this handbook useful, don't forget to star the repository!**
