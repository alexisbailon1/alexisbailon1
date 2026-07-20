# Hi there, I'm a Software Engineer 👋

I have 7+ years of experience building integrations, automations, and internal tools that solve real business problems. I specialize in backend architecture, real-time data synchronization, and modern developer workflows—leveraging **local LLM orchestration, custom agent bridges, and structured tooling** as a force multiplier to ship full-stack software faster without sacrificing architectural control.

Here is a look at what I build, how I ship to production, and the systems I engineer from concept to deployment.

---

## 🚀 Featured Production & Systems Architecture

### 🌮 Live Production Ordering Platform (Food Truck Ecosystem)
`[Proprietary / Closed Source]` • `[Live in Production]` • `[Progressive Web App]`
Architected and deployed a commercial-grade, multi-role Progressive Web App engineered for real-time order synchronization across front-of-house tablets, an iOS-optimized Kitchen Display System (KDS) with Web Audio alerts, and an administrative control panel. Built with **React 19, Vite, Tailwind CSS v4, and Firebase Realtime Database**.
* **Systems & Workflow Engineering:** Designed low-latency database hooks and role-based state routing. Implemented strict agent operating rules (`AGENTS.md`) and living technical documentation (`DOCUMENTATION.md`) to maintain absolute architectural control while cutting boilerplate scaffolding and feature time-to-market by 50%.

### 🤖 Workflow Management System
`[Systems Architecture]` • `[FastAPI / React 19]` • `[Local LLM Orchestration]`
Engineered a self-hosted, local-first Kanban hub designed to coordinate software development across multiple repositories between human developers and autonomous AI agents. Built with a **FastAPI REST backend, React/Vite UI, and SQLite running in WAL (Write-Ahead Logging) mode**.
* **Concurrent Agentic Bridge:** Developed a custom command-line bridge (`ticket_tool.py`) that safely exposes shared SQLAlchemy models to external developer agents (like Claude Code). Enables automated task fetching and audit logging without database lock contention, shell exposure, or API key leaks.
* **Private Code Review Pipeline:** Integrated a local, one-click review loop that scopes git diffs and project planning docs to a ticket's target path, routing them to an offline **Qwen2.5-Coder model running in LM Studio** for immediate architectural feedback.

```mermaid
graph TD
    subgraph Hub [Workflow Management System — Local Host]
        API[FastAPI Server & REST API] <-->|WAL Mode Concurrent R/W| DB[(SQLite Database)]
        CLI[CLI Bridge: ticket_tool.py] <-->|WAL Mode Concurrent R/W| DB
    end
    UI[React 19 Kanban UI] <-->|HTTP / API| API
    Agent[External Developer Agents / Claude Code] -->|Executes Tasks & Logs Audit Trail| CLI
    API -->|Sends Code Diffs & Planning Context| LLM{Local LM Studio / Qwen2.5-Coder}
    LLM -->|Posts Automated Code Reviews| DB
```

---

## 💻 Open Source & Active Applications

### ⛽ E85 Fuel & Technical Utility Application
`[Open Source]` • `[Native Android]` • `[Kotlin / Jetpack Compose]`
Developed a native Android utility application engineered with a single-activity Composable architecture and a pure, stateless calculation core (`FuelCalculator`). Solves complex splash-blending algebra on the fly to help automotive enthusiasts hit target ethanol blends with real-time input validation and persistent state.
* **Engineering Focus:** Demonstrates clean MVVM separation, custom Material 3 interactive UI elements, unit-testable algorithmic logic, and height-adaptive layouts.
* **AI-Accelerated Architecture Migration:** Originally developed and utilized as a complete, private application built in **.NET MAUI**, then systematically re-architected and migrated to native **Kotlin and Jetpack Compose** for its public open-source release. Leveraged AI tooling as a code-translation engine to accelerate the C#-to-Kotlin migration and scaffold modern Material 3 layouts, backed by rigorous manual refactoring and on-device performance optimization.
* **[Explore the Codebase ➔](https://github.com/alexisbailon1/e85-calculator)**

### 🃏 Pokémon TCG Scanner & Valuation Tracker
`[Active Development / Closed Source]` • `[Computer Vision / On-Device ML]` • `[Offline-First Android]`
An offline-first Android cataloging tool that transforms a device camera into an automated card ingestion and financial valuation pipeline. Built with **Kotlin, Jetpack Compose, Room SQLite, and the TCGdex API**.
* **Custom On-Device ML Pipeline:** Currently in active development, transitioning from classical computer vision to a **custom fine-tuned vision model** trained specifically for Pokémon TCG cards. The specialized model natively detects physical card boundaries and precisely localizes printed set codes, card numbers, and card names in a single inference pass—overcoming foil glare and angled captures.
* **Collector Accounting & Deduplication:** Integrates **64-bit perceptual hashing (pHash)** with Hamming-distance matching for instant visual deduplication. Features sealed "Rip Session" tracking that decouples initial purchase costs from individual card pulls, rendering live ROI and valuation history charts via Vico.

---

## 🛠️ Technical Arsenal
* **Languages & Backend:** PHP, JavaScript, Kotlin, Python, SQL, Microsoft SQL Server, FastAPI, SQLAlchemy, RESTful APIs.
* **Frontend & Mobile:** React 19, Vite, Tailwind CSS v4, Android (Native), Jetpack Compose, Material 3, Progressive Web Apps (PWA).
* **Database & Integrations:** SQLite (WAL Mode), Firebase Realtime Database & Auth, Room SQLite, Zapier, Tray.io, Atlassian Jira, Git/GitHub.
* **Systems & Vision Architecture:** OpenCV (Adaptive Edge Detection / Perspective Warping), ML Kit OCR, CameraX, Perceptual Hashing (pHash), Web Audio API.
* **Developer Tooling & Orchestration:** Local LLM Deployment (LM Studio, Qwen2.5-Coder, Gemma, Llama), Claude Code (CLI / Headless), Google Antigravity (Gemini), ChatGPT Codex (CLI / Headless), Custom CLI Agent Bridges, Automated Scaffolding & Code Review Pipelines.
