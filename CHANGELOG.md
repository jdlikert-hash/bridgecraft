# Changelog

All notable changes to **BridgeCraft** (formerly *The Behavioral Profiler*) are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [2.1.1] - 2026-09-23 — *Passive Listening Radar & Level 2 Probe Hierarchy Inversion*

Restructured Level 2 Diagnostic Probes to align with core Process Communication Model (PCM) observational methodology. Elevated passive acoustic recognition cues to the primary focal position at the top of cards, reducing live incident cognitive load and eliminating conversational friction.

### Changed
- **Passive Listening Radar as Primary Focal Anchor:**
  - Inverted the internal anatomy of all 16 Level 2 diagnostic probe cards across Psychological Motivator, Acute Stressor, and Conflict Stance drawers.
  - Positioned **"👂 Listen For (Passive Radar)"** in a high-contrast container immediately beneath the card header, allowing operators to diagnose behavioral drivers purely by listening without interrupting or interrogating.
  - Subordinated active conversational prompts (**Tactical Labels** and **Probing Questions**) to a clean secondary block beneath the listening cues.
  - Added flexbox vertical alignment (`flex flex-col justify-between`) to ensure uniform card heights across grid rows.
- **Native Chip Tooltip Lead:**
  - Updated radio chip hover tooltips to lead with `👂 Listen for: ...` before displaying the calibrated Tactical Label and Probing Question.
- **Acute Stressor Companion Briefing Panel:**
  - Added an interactive "Frontline Protocol: Disarming In-Your-Face Reactive Distress" companion briefing panel spanning the remaining 2 grid slots in the Acute Stressor drawer.
  - Eliminates trapped negative space in the 4-choice drawer while equipping operators with 4 immediate, high-yield rules for managing acute physiological flooding and reactive hostility live on calls.
- **Category Probe Microcopy:**
  - Standardized category toggle button labels from "Verbal Probes" to "Diagnostic Probes" and updated tooltips to highlight passive acoustic listening.
- **Master Guide Documentation:**
  - Updated Chapter 4 of the Master Guide to document the passive-first triage hierarchy and completed the cheat sheet with full *Listen for* cues across all 16 diagnostic items.

---

## [2.1.0] - 2026-09-22 — *Christopher Voss Tactical Empathy Integration*

Introduced proven tactical empathy and counter-manipulation frameworks from former FBI hostage negotiator Christopher Voss (*Never Split the Difference*) to enhance de-escalation, disarm defensive posturing, and protect operators during volatile interactions.

### Added
- **Tactical Labels in Level 2 Diagnostic Probes:**
  - Appended calibrated, non-interrogative "Tactical Label" alternatives (e.g. *"It seems like..."*, *"It sounds like..."*) to all 16 Level 2 diagnostic probe cards.
  - Lowers cognitive resistance and prompts a biological *"That's right"* agreement that de-escalates amygdala arousal without demanding answers.
  - Enhanced native chip tooltips to display both the interrogative question and its Tactical Label alternative.
- **Adult-State Boundary Statements in The Codex (Red Lines):**
  - Expanded Red Line ("Never Say This") triggers for volatile, high-conflict archetypes (Promoter and Rebel) across all 4 operational lenses.
  - Integrated standardized Adult-state boundary scripts to halt manipulation, pressure tactics, and protocol bypassing while keeping discussions professional and aligned.
  - Distinct UI badge and styling for Boundary Statements in live playbooks and The Codex.
- **Pre-Emptive Accusation Audits in High-Stakes Action Templates:**
  - Embedded optional `[Accusation Audit (Optional Intro)]` opening sentences at the top of factory action templates for CRM Sales and Financial Hardship lenses.
  - Disarms stakeholder emotional ammunition and defuses worst-case fears upfront before presenting tactical recovery plans.
- **Contextual Fatigue & Burnout Checks in Skill-Will Matrix:**
  - Added clarifying verbiage prompting managers to evaluate for recent incident load, on-call paging volume, and physiological exhaustion in the Excite quadrant (Low Will / High Skill) before applying behavioral interventions.

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
  - Explicit **100% Client-Side Execution**: BridgeCraft operates 100% locally with zero cloud APIs; users manually import dossiers into their external LLM of choice for simulation drills.
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
- **Terminology Shift (Assessor & Assessment):** Transitioned user-facing vocabulary from "profiler" and "profile" to "assessor" and "assessment" across UI controls, button labels, toasts, markdown exports, and documentation to emphasize objective, situational incident alignment over surveillance or labeling.
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
