# Atlas (`@atlas`) — Multi-Agent Personal OS Template

> Open-source, domain-agnostic blueprint for a **12-Agent Mesh (3 Tiers)** orchestrator with **Adaptive 2-Tier Governance (6 Pillars)**, **8 Workflow Recipes**, **4 Scheduled Automations**, and strict **Anti-Slop / Zero-Fabrication Guardrails**.

---

## 1. Quick Start (10 Seconds)

1. Fork or clone this repository and open it in your AI coding workspace (e.g., Antigravity).
2. Customize [`AGENTS.md`](AGENTS.md) with your own skills, tools, calendars, and long-term memory path.
3. Open [`index.html`](index.html) (or view the live GitHub Pages diagram) to explore all 12 Agents, Recipes, and Guardrails.
4. Talk to `@atlas` using short 3–5 word prompts:

| Goal | Example Prompt | What Atlas Does Behind the Scenes |
| :--- | :--- | :--- |
| **Start a Research Proposal** | `@atlas research topic X` | Scaffolds `projects/[Name]/` (`SOT.md`, `ROADMAP.md`), searches $\ge 2$ databases, verifies citations 1:1 |
| **Resume a Project (New Chat)** | `@atlas resume [Project]` | Reads `PROJECT.md`, `SOT.md`, and `ROADMAP.md` to restore 100% context |
| **Paper Deep Dive / Quiz** | `@atlas journal club this paper` | Extracts 1-paragraph mental model + statistical weaknesses + 5-question recall quiz |
| **Build Deck + Handout** | `@atlas presentation for topic Y` | Locks facts in `SOT.md` $\rightarrow$ drafts slides + speaker notes + visual QA |
| **Privacy-Safe Media Prep** | `@atlas blur faces + align 1:1` | Local de-identification + strict 1:1 comparison without AI photo alteration |
| **Study / NotebookLM Prep** | `@atlas extract slides / split PDF` | Converts video lectures to PDF slides and splits large books (`<500p` / `<200MB`) |
| **Schedule & App Dev** | `@atlas check calendar / build app` | Syncs calendars, runs modern web checks, TDD, and code/accessibility review |
| **Monthly Finance Sync** | `@atlas reconcile monthly budget` | Reconciles inflows/outflows via `Agent 08` (Single Writer) and updates long-term memory |

---

## 2. Core Architecture Highlights

* **Adaptive 2-Tier Governance:** Quick Tasks run in one turn with zero file clutter; Full Projects create 6 structured pillars in `projects/[Project_Name]/` (`PROJECT.md`, `AGENTS.md`, `SOT.md`, `ROADMAP.md`, `UX.md`, `project_diary.md` + `NotebookLM_Bundle/`).
* **Single-Writer Memory Rule:** Only `Agent 08` writes to persistent long-term memory (`USER.md` / `MEMORY.md`), preventing race conditions when multiple agents run in parallel.
* **Independent Tier 3 QA Gates:** `Agent 11` checks citations & statistical logic; `Agent 12` enforces PDF/visual integrity, code quality, and Banned AI Lexicon removal.
* **Compact Execution Trace (`🧭 Trace:`):** Work responses open with a single-line pipeline badge (including Tier 3 QA Gate status) in Chat UI only—with zero mid-turn tool spam and skipped on casual Q&A.
* **Optional Skill Vault Wiring:** Keep custom skills in your own separate/private GitHub repository and optionally set `SKILL_VAULT_BASE` in [`index.html`](index.html) to turn agent skill chips into direct links.
* **RTK – Ponytail – Caveman Discipline:** Minimal terminal output ingestion, minimal code footprint, and high-density bullet reporting.

---

## 3. Repository Contents

* [`AGENTS.md`](AGENTS.md) — Complete system prompt & routing specification
* [`README.md`](README.md) — Human-friendly guide & prompt cheat sheet
* [`projects-summary.md`](projects-summary.md) — Central index of active Full Projects
* [`index.html`](index.html) — Interactive SVG Architecture Diagram (Dark Navy / Teal / Mint)
* `projects/` — Workspace directory for your own 6-Pillar projects
