# 📊 CHAOSS Augur Microtasks – GSoC 2025

Welcome to my submission for the CHAOSS Augur Google Summer of Code (GSoC) 2025 Microtasks. This repository contains:

- ✅ Completed Microtasks (0, 2, and 4)
- 📈 A suite of D3.js-based interactive visualizations
- 🛠️ Contributions and observations from working with Augur & GrimoireLab

---

## ✅ Microtasks Overview

### 🛠️ Microtask 0: Set Up Augur Dev Environment
- Successfully installed and configured the Augur development environment.
- Followed the official [installation guide](https://oss-augur.readthedocs.io/en/dev/getting-started/installation.html) and development docs.
- Set up Postgres, cloned Augur, installed Python dependencies, configured `.env`, and verified data collection via workers.
- Additionally explored [GrimoireLab](https://chaoss.github.io/grimoirelab-tutorial/) for CHAOSS ecosystem context.

---

### 🪲 Microtask 2: Installation Issues Identified
While installing and configuring Augur, I encountered and documented several issues:
- No clear instructions for windows given.
- `psycopg2` version conflicts during installation.
- PostgreSQL permissions requiring role adjustments (`createuser`, `createdb`).
- Missing environment variables not clearly mentioned in docs.
- Suggested potential improvements in installation clarity via a future PR.

---

### ✨ Microtask 4: "Anything You Want to Show Us"
For this open-ended task, I focused on **data visualization** — an area I’m passionate about — and created several interactive charts using **D3.js**. These visualizations aim to make Augur data more accessible and actionable.

---

## 📈 Interactive Visualizations

| Visualization | Type | Purpose |
|---------------|------|---------|
| **Contributor Activity** | Line Chart | Track commit frequency over time |
| **Contributor Network** | Force-Directed Graph | Reveal collaboration clusters |
| **Issue Timeline** | Gantt-style Bar Chart | Display issue resolution duration |
| **Calendar Heatmap** | Calendar Heatmap | Visualize community contributions daily |

➡️  **[View Visualizations](https://github.com/Akshatb2006/Augur-Microtask/blob/master/Visualizations/Readme.md)**

---

## 🙌 Thank You

Thanks to the CHAOSS community and mentors for maintaining such an open, welcoming project. I’m excited by the potential of visual analytics to enhance open source insights, and I hope these contributions reflect that enthusiasm.

> – Akshat 🚀


