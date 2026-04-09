# Clipping-site```markdown
# lvlitup MotionForge — 119% Accurate Clip Architect Dashboard

**Built for @grantswinton_ (lvlitup), AI Agent Architect in Atlanta.**

MotionForge is a fully offline, browser‑based second‑brain orchestration system that simulates 10 specialized AI agents dedicated to achieving **literal perfection in video motion realism**. Every agent maintains its own persistent knowledge base following the Karpathy/Spisak architecture (`raw/` → `wiki/` → `outputs/`), all stored locally in IndexedDB.

> **Core mission**: Eliminate “floaty” AI video artifacts by enforcing Newtonian physics, kinematic precision, temporal coherence, and biomechanical authenticity across every frame.

---

## 🧠 How It Works

MotionForge runs entirely in your browser—no server, no API keys. All “AI” logic is simulated client‑side with deterministic, explainable rules that mimic the behavior of a real second‑brain pipeline. The result is a **fast, private, and infinitely compoundable** motion analysis environment.

### The 10 Specialized Agents

| # | Agent Name | Domain |
|---|------------|--------|
| 1 | Motion Physics Validator | Newtonian & non‑linear dynamics |
| 2 | Kinematic Trajectory Optimizer | Velocity, acceleration, path timing |
| 3 | Temporal Coherence Guardian | Frame‑to‑frame consistency, flicker elimination |
| 4 | Collision Realism Auditor | Rigid/soft bodies, friction, bounce |
| 5 | Biomechanics Architect | Human gait, weight shift, micro‑twitch |
| 6 | Camera Path Synchronizer | Dolly, parallax, lens distortion |
| 7 | Fluid & Particle Specialist | Liquids, smoke, cloth, hair |
| 8 | Velocity Calibrator | Sub‑frame precision, zero floating |
| 9 | Multi‑Agent Orchestrator | Scene‑wide coordination |
| 10 | Meta‑Accuracy Auditor | 0‑119% overall realism scoring |

Each agent maintains its own **second brain** with:
- **`raw/`** – User‑added notes, transcripts, motion references.
- **`wiki/`** – AI‑generated Markdown‑style pages with summaries, entities, and backlinks.
- **`outputs/`** – Query results, reports, and synthesized insights.
- **`schema/CLAUDE.md`** – Agent‑specific rules governing organization and linting.

---

## 🚀 Features

- **Offline‑First** – One HTML file. After the first load, everything runs locally.
- **Second‑Brain Simulation** – Ingest raw data → auto‑generate wiki pages → query with citations.
- **Per‑Agent Chat Interface** – Ask questions like *“Optimal acceleration curve for a 2.3s jump”* and get answers grounded in the agent’s stored knowledge.
- **Lint & Health Checks** – Detect contradictions, stale claims, and suggest new raw sources.
- **Video Clip Studio** – Upload a test clip (simulated) → analyze motion vectors → generate a 119% accuracy report with overlaid arrows, heatmaps, and physics graphs.
- **Multi‑Agent Orchestration** – Cross‑reference up to 5 agents for scene‑level coherence.
- **Live Dashboard** – See brain sizes, compound scores, and activity feed in real time.
- **Export Vault** – Download the entire second‑brain state as JSON (ready for real Claude Code integration).

---

## 📦 Installation & Usage

1. **Download** the `index.html` file (the entire application is self‑contained).
2. **Open** it in any modern browser (Chrome, Edge, Firefox, Safari).
3. **Start ingesting** motion references:
   - Use the **Quick Ingest** card on the Dashboard.
   - Or navigate to **Agent Brain** → select an agent → click **+ Add Note**.
4. **Query** any agent’s brain to retrieve synthesis.
5. **Analyze** a clip in the **Studio** tab to see motion overlays.
6. **Orchestrate** multiple agents for cross‑domain validation.
7. **Export** your vault anytime via the sidebar button.

No build step, no dependencies beyond Tailwind (loaded via CDN).

---

## 🧬 Architecture (Karpathy/Spisak Second‑Brain)

MotionForge implements the exact three‑layer pipeline described by Nick Spisak:

```

┌─────────┐     ┌─────────┐     ┌─────────┐
│  raw/   │ ──▶ │  wiki/  │ ──▶ │ outputs/│
└─────────┘     └─────────┘     └─────────┘
▲               │               │
│               ▼               ▼
User Input    AI Summaries    Query Results
Entities        Reports
Backlinks

```

- **Ingestion**: Raw text is stored and immediately processed by a simulated AI that extracts entities and creates a wiki page.
- **Wiki Maintenance**: Pages include summaries, cross‑references to other wiki entries, and a creation timestamp.
- **Querying**: The system searches both raw and wiki stores, returning a synthesized answer that cites its sources.
- **Linting**: Runs consistency checks (e.g., flags the word “float” as a physics violation).

---

## 🔧 Extending the System

MotionForge is designed to be a foundation. You can extend it by editing the single HTML file.

### Add a New Agent

1. Append an object to `AGENT_DEFINITIONS`:
   ```js
   { id: 10, name: "Your Agent", icon: "🧪", domain: "..." }
```

1. The IndexedDB upgrade will automatically create the necessary object stores.
2. The UI will populate the new agent in sidebars and selects.

Customize AI Simulation

All “intelligence” lives in the SimulatedAI namespace:

· processRawToWiki(agentId, rawText, existingWiki) – Modify to change how wiki pages are generated.
· queryBrain(...) – Replace with a call to a real LLM API if desired.
· lintBrain(...) – Add custom validation rules.

Enable Real Video Processing

The canvas overlays are currently static demonstrations. To connect actual video analysis, hook into the analyze-clip-btn handler and replace the mock report with real frame‑extraction + motion‑vector logic (e.g., using OpenCV.js or a WebAssembly module).

Export as True ZIP

The current export downloads a JSON file. To produce a folder‑structured ZIP (mimicking a real filesystem), integrate a pure‑JavaScript ZIP library like JSZip and modify the export-vault-btn handler.

---

⌨️ Keyboard Shortcuts

· Tab navigation between UI sections is fully supported.
· Copy/paste works in all text areas and input fields.

---

🎨 Theming & Personalization

The UI follows a dark cyber‑minimalist aesthetic:

· Base: #0a0a0a
· Neon cyan (#00f0ff) for physics‑related elements.
· Neon magenta (#ff00c1) for kinematic/velocity accents.

All motion accents (hover states, graph edges) use cubic-bezier transitions that echo the theme of “perfect motion.”

---

📄 License

This project is provided as a reference implementation for the lvlitup workflow. You are free to modify and use it for personal or commercial purposes.

---

Built with precision by @grantswinton_ — because 100% motion accuracy isn’t enough.

```
```
