# Atlas (`@atlas`) — Template Bootstrap & AI Onboarding Guide (`BOOTSTRAP.md`)

> Self-contained setup guide to turn this template repository into a working **12-Agent Atlas OS** on any machine or AI coding assistant (Antigravity, Claude Code, Cursor, Codex).

---

## 1. Initial Setup (5 Minutes)

1. **Clone or Fork this Repository**:
   ```bash
   git clone https://github.com/sunsmile872/atlas-orchestrator-template.git atlas-orchestrator
   cd atlas-orchestrator
   ```
2. **Customize Your Identity & Roster**:
   - Edit `AGENTS.md`:
     - Update the header/domain context in `§1` and `§2` to match your profession, workflows, and preferred language.
     - Map your installed skills, MCP servers, or external Skill Vault in `§3`.
     - Adjust Recipes & Scheduled Automations in `§5` for your recurring tasks.
   - Update `projects-summary.md` as you create new `projects/<Project_Name>/` folders.
3. **Install Atlas Portable Skills (`atlas-skills-template`)**:
   ```bash
   git clone https://github.com/sunsmile872/atlas-skills-template.git ~/.gemini/config/skills
   cd ~/.gemini/config/skills/pmr-slide-creator/templates/bento_engine && npm install
   ```
   *(Keep your skills directory as its own repository so skill updates never collide with project commits.)*
4. **Runtime Tools (Optional, for Document/Slide Recipes)**:
   - Python (`uv`, `python-pptx`, `pymupdf`, `python-docx`, `pillow`, `matplotlib`)
   - Node.js (`pptxgenjs`) and LibreOffice (`soffice`) for slide rendering/audits

---

## 2. Prompt to Activate Atlas in Any AI Assistant
Open this folder in your AI IDE and paste:
```text
Read @AGENTS.md and @projects-summary.md.
You are now operating as Atlas (@atlas), the Tier 1 Master Coordinator for this workspace.
Classify every request as Tier A (Quick Task) or Tier B (6-Pillar Full Project), enforce Tier 3 Quality Gates (Agents 11 & 12) as isolated subagents for major deliverables, and display the compact Execution Trace badge at the top of completed tasks.
```

---

## 3. Keeping Your OS Portable (Disaster Recovery)
- **One Project = One Folder (`projects/<Name>/`)**: Keep `PROJECT.md`, `SOT.md`, `ROADMAP.md`, and `project_diary.md` inside each project so any new AI session can restore 100% context in seconds.
- **Ignore Heavy Binaries**: `.gitignore` already excludes `*.pdf` and `*.docx` by default; keep generated binaries rebuildable from Markdown/code/JSON.
- **Checkpoint Often**: Run `@atlas checkpoint` (or `git add -A && git commit && git push`) after major milestones.
