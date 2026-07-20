# Hi there, I'm a Software Engineer 👋

I have 7+ years of experience building integrations, automations, and internal tools that solve real business problems. I specialize in backend architecture, data flow, and accelerating full-stack product development through **AI-assisted tooling, local LLM orchestration, and autonomous agent workflows**.

Here is a look at what I build, how I ship to production, and the systems I use to engineer software from concept to deployment.

---

## 🚀 Featured Production & Systems Architecture

### 🌮 Live Production Ordering Platform (Food Truck Ecosystem)
`[Proprietary / Closed Source]` • `[Live in Production]` • `[Progressive Web App]`
Architected and deployed a commercial-grade full-stack ordering platform and Kitchen Display System (KDS) engineered for real-time order tracking and native OS audio notifications. 
* **AI-Assisted Prototyping:** Utilized AI coding assistants (Claude Code, Gemini) to rapidly scaffold complex UI components and backend logic, accelerating initial time-to-market while maintaining strict production reliability standards.

### 🤖 Workflow Management System
`[Systems Architecture]` • `[Local LLMs / Claude Code]` • `[Workflow Automation]`
Engineered a custom task-tracking dashboard featuring complex state routing and agile workflow automation. Designed to manage autonomous AI development agents and streamline backlog execution.
* **Agentic Tooling:** Instead of manual prompting, structured markdown tickets are ingested by local LLMs and AI coding assistants to prototype features, refactor code, and execute systems integrations.

```mermaid
graph TD
    A[Engineer / Feature Request] -->|Creates Markdown Ticket| B(Workflow Management System)
    B -->|Ingests Task Specs| C{AI & Agentic Tooling Pipeline}
    C -->|Scaffolds Code & UI| D[Automated Prototyping]
    C -->|Executes Refactoring| E[Backend & SQL Integration]
    D -->|Human Review & Polish| F[(Production Codebase)]
    E -->|Human Review & Polish| F
