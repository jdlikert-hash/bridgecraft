# Changelog

All notable changes to **BridgeCraft** (formerly *The Behavioral Profiler*) are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [2.0.0] - 2026-09-21 — *The Adaptive Operational Console*

BridgeCraft 2.0 represents a comprehensive architectural leap from a single-purpose incident triage calculator to an end-to-end tactical communication, de-escalation, and longitudinal team coaching platform.

### Added
- **Multi-Domain Operational Frames (Lenses):**
  - Instant domain morphing across 4 high-stakes operational environments:
    - 🏢 **IT Operations & Incident Command** (`it_ops`): Sev-1 war rooms, SRE on-call rotations, Slack incident channels, and telemetry isolation.
    - 💼 **Customer Success & Enterprise CRM** (`crm_sales`): Escalated executive reviews, contract renewal churn risks, and SLA breach save briefs.
    - 💳 **Banking Hardship & Loss Mitigation** (`financial_hardship`): Foreclosure prevention, loss mitigation workouts, and CFPB compliance.
    - 🩺 **Crisis Counseling & Mental Health** (`counseling_crisis`): Crisis hotline intake, somatic grounding protocols, and emotional safety.
  - Full URL deep-linking support (`?lens=it_ops`, `?lens=crm_sales`, `?lens=financial_hardship`, `?lens=counseling_crisis`).
  - Dynamic domain theming with custom CSS variable palettes for each frame.
- **Level 2 Conversational Diagnostic Probes:**
  - Integrated expandable helper drawers under Motivator, Stressor, and Conflict Stance chips.
  - Provides non-invasive, conversational questions responders can ask live on bridge calls to pinpoint distress patterns without asking invasive questions.
- **Adaptive Cognitive Framing Engine:**
  - Shifted beyond dated NLP terminology into applied cognitive science and mental dialects.
  - Automatically maps behavioral cues into 6 sensory processing styles:
    - *Auditory-Digital* (Thinker / Logic & Data)
    - *Evaluative Vision* (Persister / Standards & Values)
    - *Somatic Kinesthetic* (Harmonizer / Relational & Support)
    - *Dynamic Kinetic* (Rebel / Spontaneous Problem-Solving)
    - *Action & Velocity* (Promoter / Direct Movement & Payoffs)
    - *Internal Mental Imagery* (Imaginer / Reflection & Spatial Schema)
  - Displays real-time linguistic markers and verbal alignment scripts.
- **1-on-1 Coaching Console & Longitudinal Task Tracker:**
  - New 5th operational tab dedicated to engineering managers, leads, and coaches.
  - Interactive SVG 2x2 **Skill-Will Matrix** dynamically plotting tasks into four actionable quadrants:
    - *Guide* (Cyan · High Will / Low Skill)
    - *Delegate* (Emerald · High Will / High Skill)
    - *Direct* (Rose · Low Will / Low Skill)
    - *Excite* (Amber · Low Will / High Skill)
  - Longitudinal task management with rating history linked to specific stakeholder observations.
  - Dynamically generated coaching strategy cards synthesizing quadrant leadership stances with the stakeholder's dominant PCM cognitive dialect.
- **Tactical De-Escalation Rehearsal Sandbox:**
  - 1-click export of structured training dossiers (`.md`) formatted specifically for external AI roleplay (**Google NotebookLM, Microsoft Copilot, ChatGPT, Claude**).
  - Explicit **Air-Gap Architecture**: BridgeCraft operates 100% locally with zero cloud APIs; users manually import dossiers into their external LLM of choice for simulation drills.
  - Embedded **Anti-"Cloning" Ethical Standard** ensuring all dossiers serve strictly as operational flight simulators for tactical empathy.
- **Multi-Observer Intelligence & Alias Merge Engine:**
  - Aggregates observations across multiple observers and operational contexts (Outages, 1-on-1s, All-Hands).
  - Calculates **Base Consensus %** and detects **Situational Adaptation** (e.g. Thinker during quiet sprints vs. Promoter blowout during P1 outages).
  - 1-click **Merge Duplicate Record** utility to consolidate aliases and misspellings while retaining full chronological history.
- **Custom Battlecard Engine:**
  - In-app inline editor allowing responders to customize tactical "Say This" and "Avoid" scripts for any archetype in any domain.
  - Graceful factory reset support per archetype or entire domain.
- **Desktop Typography Scaling (+20%):**
  - Added responsive base font-size scaling (`@media (min-width: 1024px) { html { font-size: 120%; } }`), naturally expanding container width to 1228.8px and scaling all fonts, chips, and buttons by +20% for comfortable laptop ergonomics without browser zoom.
  - Preserved standard 100% (16px) scaling on mobile devices for touch-optimized responsiveness.
- **Restored GitHub Header Integration:**
  - Added prominent GitHub repository button to the top navigation header alongside the 5 tabs.
- **Visual Reference Suite:**
  - Created [BridgeCraft_Visual_UI_Tour.pdf](docs/BridgeCraft_Visual_UI_Tour.pdf) (7-page executive visual reference) and 6 high-resolution screenshots to anchor AI video generators (e.g. NotebookLM) on authentic UI captures.

### Changed
- **Rebranded Platform:** Renamed from *The Behavioral Profiler* to **BridgeCraft: Tactical Incident Communication & De-Escalation Console**.
- **Branding Assets:** Added custom dual-tower suspension bridge emblem and matching SVG favicon.
- **Streamlined Navigation:** Removed redundant and static "Active Domain" badge from the lens strip.
- **Documentation Overhaul:** Engineered [BRIDGE_CRAFT_MASTER_GUIDE.md](BRIDGE_CRAFT_MASTER_GUIDE.md) and [README.md](README.md) for automated video and podcast generation.

---

## [1.0.0] - 2026-09-18 — *The Behavioral Profiler Initial Release*

Initial prototype release focused on rapid incident triage for IT operations and war room communications.

### Added
- Core two-tier Process Communication Model (PCM) engine: Base channel vs. Phase distress driver.
- 6 incident archetypes: Thinker, Persister, Harmonizer, Rebel, Promoter, Imaginer.
- Dual-Lens DISC leadership alignment mapping (High D, I, S, C).
- Instant Calibrated Incident Playbook with copyable Slack status updates and frontline de-escalation scripts.
- Single-domain IT operations focus.
- 100% offline client-side storage architecture (`localStorage`) with zero network dependencies.
- Independent authorship and workplace non-assignment declarations for Jack Likert.
