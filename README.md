# BridgeCraft v2.1.2 — Strategic Field Manual & Architecture

> **A tactical incident communication, de-escalation, and situational alignment console designed for frontline operators, client advocates, and people leaders across high-pressure environments.**  
> *(See [CHANGELOG.md](CHANGELOG.md) for full release history up to v2.1.2)*

> 🎙️ **Definitive Master Guide for Google NotebookLM (Audio Overview / Podcast & Slide Decks):**  
> For the complete chapter-by-chapter curriculum engineered for **Google NotebookLM** podcast generation, executive briefing synthesis, and feature walkthrough decks, see **[BRIDGE_CRAFT_MASTER_GUIDE.md](BRIDGE_CRAFT_MASTER_GUIDE.md)**.  
> 🖼️ **Visual UI Tour & Ground-Truth PDF Reference:** See **[BridgeCraft_Visual_UI_Tour.pdf](docs/BridgeCraft_Visual_UI_Tour.pdf)** (or view the HTML version at [`docs/BRIDGECRAFT_VISUAL_TOUR.html`](docs/BRIDGECRAFT_VISUAL_TOUR.html)).

---

## 1. Executive Summary

High-pressure operations inevitably strain team coordination. When urgency is elevated, different stakeholders process information through distinct lenses—some require verified data and timelines, others demand rapid bottom-line summaries, and others focus on team consensus or risk avoidance. Misalignment across these communication styles creates unnecessary friction and operational delay.

**BridgeCraft** serves as an interactive behavioral assessor designed to run alongside active workflows. By observing a few initial cues, operators can determine how a colleague, client, or leader processes urgency under stress and access tailored talk tracks (what to say and what to avoid) to keep discussions productive and aligned.

---

## 2. Core Psychological Engine: The Two-Tier Model

The Assessor is built upon principles adapted from Dr. Taibi Kahler's **Process Communication Model (PCM)**—the framework famously utilized by NASA for astronaut crew selection and crisis de-escalation.

Traditional personality frameworks (like MBTI or Big Five) are descriptive and static—they tell you who someone is on a relaxed Sunday morning. PCM is **dynamic and behavioral**—it models how an individual's communication channel shifts under acute stress.

### The Two-Tier Architecture:
1. **Base (The Communication Channel / Filter):**
   - The neurological baseline established early in life.
   - Dictates how the person *perceives* information: through Thoughts (logic), Opinions (values), Emotions (feelings), Reactions (fun/spontaneity), Actions (direct movement), or Inactions (reflection).
   - **Tactical rule:** Speak to their Base to be understood.

2. **Phase (The Current Distress Driver & Conflict Stance):**
   - The psychological battery charger that needs replenishment right now.
   - Dictates how the person *acts out* when their needs are starved or when an incident creates acute pressure.
   - **Tactical rule:** Address their Phase need to de-escalate conflict.

```
+-------------------------------------------------------------+
|                     THE BEHAVIORAL STACK                    |
+-------------------------------------------------------------+
|  [PHASE] Current Stressor / Conflict Stance (Acute Distress)|
|          --> Determines: What they are demanding / fearing   |
+-------------------------------------------------------------+
|  [BASE]  Speech Tempo / Focus / Posture (Operating Channel) |
|          --> Determines: The vocabulary & cadence you speak  |
+-------------------------------------------------------------+
```

---

## 3. The 6 Core Archetypes in Incident Context

| Archetype | Perceptual Filter | What Triggers Distress in an Incident | Distress Behavior ("The Tell") | Tactical Incident Response (Do This) | What NEVER to Do |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **The Thinker** | Logic, Data, Structure | Ambiguity, lack of data, moving goalposts | Over-explains, nitpicks, weaponizes facts, micromanages | Provide structured bullet points, timestamps, and verifiable data | Don't make emotional appeals or hand-wave details |
| **The Persister** | Values, Principles, Respect | Perceived incompetence, broken trust, ethical compromise | Becomes dogmatic, preaches, pushes rigid opinions | Solicit their opinion, validate their dedication, align on principles | Don't dismiss their convictions or call their concern "trivial" |
| **The Harmonizer** | Empathy, Relationships | Hostility, aggression, cold detachment | Over-apologizes, freezes, makes careless mistakes to solicit rescue | Use "we" language, acknowledge personal stress, provide psychological safety | Don't bark orders or treat them as a mere cog in the machine |
| **The Rebel** | Spontaneity, Reactions | Strict constraints, micromanagement, dull bureaucracy | Blames others, acts sarcastic in Slack, actively defies process | Offer discrete choices, keep energy dynamic, challenge them to problem-solve | Don't impose heavy-handed rules or lecture them on protocol |
| **The Promoter** | Direct Action, Immediate Wins | Stagnation, analysis paralysis, slow deliberation | Manipulates, escalates prematurely, steamrolls others | Give the bottom-line payoff immediately, challenge them to clear blockers | Don't provide long backstories or show hesitation |
| **The Imaginer** | Reflection, Spatial Clarity | Sensory overload, rapid-fire cross-talk, forced group consensus | Completely withdraws, goes unresponsive on the bridge call | Give them quiet space, send 1-on-1 direct requests rather than open questions | Don't force public on-the-spot group brainstorming |

---

## 4. DISC vs. PCM: Strategic Synthesis

A common question is: **"Should we incorporate DISC alongside this, or is it overkill?"**

### The Diagnosis:
- **DISC** is macro, static, and universally understood in corporate management:
  - **D (Dominance):** Direct, firm, results-oriented (Fast + Task)
  - **I (Influence):** Outgoing, enthusiastic, inspiring (Fast + People)
  - **S (Steadiness):** Calm, patient, accommodating (Deliberate + People)
  - **C (Conscientiousness):** Analytical, reserved, precise (Deliberate + Task)
- **PCM** is micro, dynamic, and distress-oriented:
  - It explains why an engineer who is normally a quiet "C" suddenly starts barking orders like an aggressive "D" (Promoter phase distress), or why a manager who is normally a "D" suddenly withdraws completely into silence (Imaginer phase distress).

### The Recommendation:
**Do not force a redundant 20-question DISC test into the incident triage flow.** During an outage or high-stress conflict, cognitive load must remain minimal.

Instead, utilize a **Synthesized Dual-Lens approach**:
1. **Automatic DISC Mapping:** The engine can natively display the DISC archetype corresponding to the observed PCM pattern:
   - *Thinker* $\rightarrow$ **High C** (Analytical / Systematic)
   - *Persister* $\rightarrow$ **High D / High C** (Principled / Determined)
   - *Harmonizer* $\rightarrow$ **High S** (Supportive / Empathetic)
   - *Rebel* $\rightarrow$ **High I / D** (Expressive / Disruptive)
   - *Promoter* $\rightarrow$ **High D** (Driver / Competitive)
   - *Imaginer* $\rightarrow$ **High C / S** (Reflective / Deliberate)
2. **The "Incident High-D Reality":** In operational emergencies, almost all executives and clients temporarily adopt an aggressive **High-D presentation** ("What is broken, when is it fixed, who is fixing it?"). Recognizing whether this is their *true base* or a *distress phase masking a panic-stricken Thinker or Harmonizer* allows frontline staff to tailor their response perfectly.
3. **Adaptive Cognitive Framing & Mental Dialects:** Every individual uses specific linguistic markers that reveal how they map the world around them. We don't just listen to words; we analyze cognitive framing. If language indicates a visual processing style, we adapt our communication to paint a clearer picture; if auditory, we tune responses to resonate. It is applied behavioral science designed to speak a stakeholder's exact mental dialect:

| PCM Archetype | Processing Style | Mental Dialect | Primary Cognitive Markers | Task Alignment Script |
| :--- | :--- | :--- | :--- | :--- |
| **The Thinker** | **Analytical** | Auditory-Digital (Logic) | *makes sense, analyze, process, data, compute, logic, criteria* | *"Does this sequence make logical sense? Can you process the metrics and analyze the failure criteria?"* |
| **The Persister** | **Evaluative** | Vision & Standards | *in my view, perspective, respect, standards, integrity, verify* | *"In your view, what standard must we hold? We respect your perspective and trust your judgment on quality."* |
| **The Harmonizer** | **Relational** | Somatic Kinesthetic | *feels like, touch base, grasp, handle, heavy lift, comfortable, support* | *"How does this workload feel to you? Let's touch base so you feel completely supported and grounded."* |
| **The Rebel** | **Spontaneous** | Dynamic Kinetic | *sounds cool, kick around, toss out, fun, crazy idea, vibe, wild* | *"Sounds like a fun puzzle—wanna kick around some ideas, toss out the rulebook, and test something wild?"* |
| **The Promoter** | **Direct** | Action & Velocity | *bottom line, jump on it, hit the ground running, nail it down, win, move* | *"Bottom line: let's jump on this right now, nail it down before 3 PM, and secure the win."* |
| **The Imaginer** | **Reflective** | Internal Mental Imagery | *picture, imagine, envision, reflect, contemplate, space, horizon* | *"Take mental space to picture how this should look. When you've envisioned the full schema, ping me."* |

4. **Applied Tactical Empathy (Christopher Voss Doctrine):** High-stakes operational triage incorporates principles from master hostage negotiator Christopher Voss (*Never Split the Difference*):
   - **Tactical Labels in Level 2 Diagnostic Probes:** Direct questions often trigger defensive rationalization. Non-interrogative labels (*"It seems like..."*, *"It sounds like..."*) identify the emotional dynamic without demanding an answer, eliciting a biological *"That's right"* agreement that de-escalates amygdala arousal.
   - **Boundary Statements in Red Lines:** Accommodating high-conflict, volatile archetypes (Promoter and Rebel) is often misinterpreted as weakness, inviting manipulation. Standardized Adult-state boundary scripts halt boundary-pushing while keeping the conversation professional and aligned.
   - **Accusation Audits in High-Stakes Templates:** Pre-emptively voicing the stakeholder's worst-case fears and grievances at the top of CRM Sales and Financial Hardship action templates defuses emotional ammunition before they can fire it.

---

## 4.5 The Frontline Behavioral Stack: Real-Time De-Escalation (Zero Jargon)

BridgeCraft synthesizes advanced psychological models (social neuroscience, conflict dynamics, negotiation postures, and autonomic regulation) **without bogging operators down in clinical acronyms or academic definitions**. 

Frontline engineers, incident commanders, and client advocates don't need a psychology degree—they need clear, plain-English answers to four critical operational questions:

| Behavioral Dimension | The Plain-English Operational Reality | The Frontline Action (What You Do) |
| :--- | :--- | :--- |
| **1. The Core Trigger** | **What stole their patience?** When people panic or lash out, their brain felt a sudden threat to **Certainty** (shifting timelines), **Control** (feeling dictated to), **Respect** (competence questioned), or **Safety** (fear of blame). | **Give the specific antidote:** If they need certainty, give a firm checkpoint timestamp (*"Next update at 2:15 PM with delta metrics"*). If they feel pushed around, offer two binary options. |
| **2. The Conflict Trap** | **How are they baiting you?** Under acute stress, people unconsciously drag you into traps: **The Attacker** (shouting and demanding compliance), **The Helpless Deflector** (freezing and deflecting all decisions), or **The Data Weaponizer** (flooding the room with trivia to avoid responsibility). | **Deploy the Circuit Breaker:** Never take the bait. If they attack, don't apologize or argue policy. Use the scripted **Circuit Breaker** line to reset the conversation into Adult-to-Adult problem-solving. |
| **3. Negotiation Stance** | **What posture are they taking?** Are they **Bulldozing** (forcing resolution by power), **Holding a Principled Stand** (protecting standards), or **Appeasing** (over-promising just to end the call)? | **Counter their move:** Bulldozers need firm boundaries and options. Principled leaders need their mission acknowledged first. Appeasers need gentle probing for hidden operational risks. |
| **4. Brain Bandwidth** | **Can their brain even hear logic right now?** Acute panic triggers fight-or-flight, dropping working memory and reasoning bandwidth by **~80%**. | **Regulate biology before logic:** Never dump complex telemetry or policy on an angry stakeholder. Drop your vocal cadence, slow your breathing, and label their reality first. Once they physically exhale, their reasoning bandwidth returns. |

---

## 5. Four Operational Frames & Tactical Domains

BridgeCraft provides four specialized operational frames ("lenses"), each featuring tailored observational cues, specialized communication channels, and domain-specific action templates:

| Operational Lens | Primary Operating Channels | Operational Stakes & Core Use Case | Primary Artifact / Script |
| :--- | :--- | :--- | :--- |
| **🏢 IT Operations & Incident Command** (`it_ops`) | Voice incident bridges, Slack/Teams incident channels, on-call paging, status pages | Sev-1 / P1 outages, production downtime, SRE on-call rotations, cross-functional bridge coordination | Incident War Room Status Updates & Telemetry Isolation Scripts |
| **💼 Customer Success & Enterprise CRM** (`crm_sales`) | Executive video calls (Zoom/Meet), high-priority email threads, QBRs, customer save meetings | Furious Sales VPs, contract renewal churn risks, SLA breach executive escalations | Executive Account Save Email & Partnership Alignment Memos |
| **💳 Banking Hardship & Loss Mitigation** (`financial_hardship`) | Inbound phone queues, loss mitigation intake, borrower desk interviews, certified mail notices | Imminent foreclosure, loan modification workouts, CFPB compliance, borrower distress | Borrower Stabilization Script & 3-Step Loss Mitigation Plan |
| **🩺 Crisis Counseling & Mental Health** (`counseling_crisis`) | Crisis hotlines, SMS/chat triage portals, walk-in intake, clinical debriefs | Acute emotional dysregulation, panic hotline intake, trauma-informed triage | Somatic Grounding Protocol & Structured Reality Testing Note |
| **🛡️ Executive Alignment & Upward Defense** (`power_defense`) | Private 1-on-1s, executive reviews, skip-level escalations, capacity negotiations | Coercive power dynamics, staged urgency, unfunded scope mandates, transactional compliance games | Live 30s Card, Multi-Cue Decoder, Domain Trade-Off Memos & Private Incident Log |

### URL Deep-Linking & Standalone Deployment:
- **Instant Domain Switching:** Click any lens on the top Operational Lens strip to morph the entire application in real time.
- **Deep-Linking Support:** Directly bookmark or link your domain using query parameters:
  - `?lens=it` or `?lens=it_ops` (IT Operations)
  - `?lens=crm` or `?lens=crm_sales` (Customer Success & CRM)
  - `?lens=banking` or `?lens=financial_hardship` (Banking Hardship & Loss Mitigation)
  - `?lens=counseling` or `?lens=counseling_crisis` (Crisis Counseling & Mental Health)
  - `?lens=power_defense` or `?lens=defense` (Executive Alignment & Upward Defense)
- **Standalone Domain App Export:** Click **Export Domain App** in the header to download a zero-dependency single HTML file pre-configured and locked to that specific domain for offline team distribution.

---

## 5.5 Upward Defense Workbench: Navigating Power Dynamics & Transactional Games

When communicating downward or across peers, standard Process Communication Model (PCM) de-escalation assumes distress is authentic: an engineer panicked by moving deadlines needs structured certainty; an overwhelmed account manager needs relational support.

However, in corporate power asymmetries, **apparent "Phase distress" from senior stakeholders is frequently an instrumental tactic**—a transactional game designed to extract uncommitted scope, bypass governance, or force immediate compliance through manufactured fear or urgency. Standard PCM emotional appeasement fails here because accommodating manufactured panic rewards the tactic, leading to manager burnout and hidden team overload.

The **Upward Defense** lens (`?lens=power_defense`) replaces appeasement with **Aligned Deference, Objective Multi-Cue Diagnosis, Written Trade-Off Ledgers, and Cross-Functional Governance**.

### The 5 Workbench Modules:

1. **⚡ The Live Card (In-the-Room 30-Second Micro-Loop):**
   - **Pause:** Slow your breathing, keep feet flat, pick up a pen. Delay is an operational defense. Your body will naturally want to agree to relieve discomfort.
   - **Acknowledge:** Validate the priority, not the blame or false premise (*"I hear that [Request] is an executive priority"*).
   - **Pin It:** Never commit to dates, numbers, or scope in the room. Offer to send written trade-off options by a specific time you control.
   - **Tone Modulation (Standard vs. High-Deference):** Toggle High-Deference when operating in strict hierarchical or high power-distance environments. Frame capacity constraints as a respectful consultation (*"To ensure I do not compromise your committed deliverables..."*) without showing defiance.
   - **Exit Lines:** Scripted boundary phrases to pause the discussion when cornered without escalating tension.

2. **🔍 Diagnostic Decoder (Multi-Cue Diagnostic Engine):**
   - Ticks 2–4 observable markers across three distinct categories:
     - *What they Say:* Vague directives, past grievance lists, unwritten promises, "take one for the team".
     - *How they Deliver:* Manufactured urgency, sudden volume/temper displays, private 1-on-1 pressure.
     - *How it is Structured:* Verbal-only mandates, bypassing PMO/lead, dividing peers, shifting criteria.
   - Calculates diagnostic confidence against the 27-game taxonomy.
   - **The Innocent Alternative Check:** Highlights explicit operational checks (*"Could this be innocent?"*) to differentiate legitimate organizational fire drills from manipulative games, preventing hyper-vigilant misattribution.
   - **Domain-Neutral Confirmation Memos:** Auto-generates structured written plans of record across 5 specialized vocabularies: Engineering (PRs, sprints, tech debt), IT Operations (tickets, SLAs, incidents), Finance (budgets, forecasts, audits), Sales (pipeline, accounts, deals), and General Business.

3. **📚 Games Library (27 Documented Patterns across TA, Karpman, Influence, and Scope):**
   - **Transactional Analysis (Eric Berne):** *NIGYSOB ("Now I've Got You, Son of a Bitch")*, *Why Don't You / Yes But*, *Guilt / Debt Induction*.
   - **Karpman Drama Triangle (Stephen Karpman):** *Persecutor-to-Rescuer Switch*, *Divide and Conquer*.
   - **Influence & Compliance Tactics (Robert Cialdini & Social Psychology):** *Fear-then-Relief*, *Forced Urgency*, *Door-in-the-Face*, *Foot-in-the-Door*, *DARVO*, *Stonewalling*, *Veiled Threat*.
   - **Scope Governance:** *Loaded Question*, *Moving Goalposts*, *Verbal-Only Mandate*.
   - **Custom Game JSON Builder:** Allows teams to add custom organizational games that persist locally and participate in live cue decoding.

4. **🎯 Training Drills: Scenarios & Interactive Flashcards:**
   - **Scenario Practice ("Name the Game"):** 22 realistic, multi-role workplace scenarios (including genuine, innocent requests as negative controls). Operators evaluate dialogue, identify matching games, and receive instant feedback.
   - **Interactive Flashcards (Active-Recall Drills):**
     - Card prompt displays the game name.
     - The operator mentally rehearses: *What cues indicate this game? What payoff is the stakeholder seeking? How do I test innocence? What is my spoken counter?*
     - Click **Reveal** to inspect the cues, payoff, innocent test, and exact spoken counter-line.
     - Click **Next card** to cycle through the catalog.
     - *Recommended drill frequency:* Run 5 flashcards weekly or right before major stakeholder negotiations.

5. **🛡️ Escalation & Objective Incident Logging:**
   - **10-Point Severity Matrix:** Evaluates observed behaviors against clear thresholds: Serious (requires immediate escalation through independent channels like ethics hotlines or HR), Warning Signs (requires written records and mentor consultation), or Routine Tactic (manage with written confirmation).
   - **Objective Incident Record Protocol:** Template for logging private incident notes that meet evidentiary standards—recording exact quotes, physical body language, times, locations, and corroborating witnesses while strictly omitting subjective emotional adjectives.

---

## 6. How to Use the App (60-Second Quick Start)

1. **Fire up the app:** Double-click `bridgecraft.html` (or `the_behavioral_profiler.html`) in any browser (Chrome, Edge, Firefox, Safari). No installation, Node.js, or server required.
2. **Enter the Stakeholder / Speaker Identifier:** Type the name or role (e.g., *"VP Engineering"*, *"Escalated Customer Acme Corp"*, *"On-Call DBA"*).
3. **Observation Mode Toggle (Camera Off vs. Camera On):**
   - **Camera Off (Voice & Slack):** Default mode tailored for modern incident response where video is unavailable. Adapts indicators to tone of voice, pause durations, and Slack message syntax.
   - **Camera On (Video):** Optimizes indicators for physical posture, gestures, and video presence.
   - **Camera-Off Quick Decoder:** Click the in-app cheat sheet to reference how Thinkers, Persisters, Harmonizers, Rebels, Promoters, and Imaginers write in Slack and speak on voice bridges.
4. **Level 1: Tap Base Indicators (Observation):**
   - *Speech Tempo & Typing Cadence:* How fast are they talking/typing?
   - *Primary Focus:* Are they fixated on Tasks, People, Principles, Action, or Ideas?
   - *Channel Demeanor / Posture:* Formal & Structured, Gentle & Measured, or Urgent & High-Energy.
5. **Level 2: Tap Phase Indicators (Distress Probe):**
   - *Motivator:* What are they starving for? (Status, Security, Space, Approval?)
   - *Stressor:* What triggered the blowout? (Time crunch, loss of control, friction?)
   - *Conflict Stance:* When cornered, do they blame, lecture, withdraw, or dominate?
6. **Hit "Calibrate Incident Playbook":**
   - Instantly read the **DISC Leadership Alignment** (High D, I, S, C mapping).
   - Read the **Incident Tactical Playbook ("Do's & Don'ts")** and copyable Slack status updates.
   - Read the **Frontline Strategy** and **Management Insight**.
7. **Save & Export:**
   - Click **Save to Archive** to persist the observation into the multi-observer Field Archive.
   - Click **Export Playbook (.MD)** to download a structured incident debrief markdown report.
   - Click **Rehearsal Sandbox (.MD)** in Field Archive or 1-on-1 Coaching to compile a 100% client-side rehearsal dossier for manual upload into external AI tools (NotebookLM, Copilot, ChatGPT).

---

## 7. Application Architecture & Navigation

1. **Active Console (Rapid Triage):** The core fast-input engine for real-time calibration, DISC alignment, and copy-paste incident scripts. Includes dynamic autocomplete matching known names and aliases, plus collapsible **Level 2 Diagnostic Probes** featuring passive listening radar cues (*"Listen for"*) prominently at the top, Voss **Tactical Label alternatives**, and direct interrogative fallbacks to lower defenses live on calls.
2. **The Field Archive (Multi-Observer Library):** Persistent client-side archive storing multiple timestamped observations per stakeholder. Tracks observer identity, environment context, situational adaptation, and includes a 1-click merge engine for typo consolidation.
3. **The Codex (Tactical Battlecards):** Comprehensive reference manual combining PCM archetypes, DISC quadrants, and frontline de-escalation battlecards. Custom battlecards directly power live Incident Playbooks calibrated on the Active Console. Includes adult-state **Boundary Statements** within Red Line triggers for volatile archetypes (Promoter and Rebel) to counter manipulation. Users can click **Edit Battlecard** to customize the exact talk tracks, boundary scripts, and action templates for any archetype in any domain, with complete local persistence.
4. **1-on-1 Coaching (Skill-Will Matrix & Task Tracker):** Longitudinal coaching matrix enabling managers and incident leads to track individual work assignments, assess situational Skill and Will levels, plot tasks on the interactive Skill-Will Quadrant (Direct, Guide, Excite, Delegate), and receive tailored communication strategies for each task—including contextual **Fatigue & Burnout Checks** in the Excite quadrant before applying behavioral interventions.
5. **Tactical Rehearsal Sandbox (Client-Side AI Handoff):** Compiles multi-observation dossiers, cognitive framing markers, and active coaching tasks into a single markdown file formatted for external roleplay. **BridgeCraft contains NO built-in AI chatbot or cloud APIs**—the user manually imports the file into their external LLM of choice for live training.
6. **Field Manual:** Complete in-app operational documentation, live-fire drill guidelines, and legal protections.

---

## 8. Custom Talk Tracks & Stakeholder Intelligence

BridgeCraft includes a zero-latency, private customization layer allowing teams to tailor the engine to their organization's unique voice and individual relationships:

### A. Global Playbook Customization (Domain-Level)
* **Battlecard Inline Editor:** On "The Codex" tab or directly from the Active Console results card, click **Edit Battlecard** on any archetype.
* **Full Template Control:** Edit "Say This" scripts, "Never Say This" triggers, and the full communication template (e.g., custom Slack, email, or executive memo formats).
* **Graceful Factory Resets:** Reset an individual archetype or click **Reset Domain Defaults** to instantly restore factory defaults without losing stakeholder dossiers.
* **Portable Backups:** All customized battlecards export automatically with JSON backups and restore seamlessly during data migration.

### B. Per-Person Stakeholder Intelligence
High-stakes communication is always personal. BridgeCraft allows users to attach bespoke intelligence to individual stakeholders in The Field Archive:
* **Known Hot Buttons & Taboos:** Record sensitive triggers (e.g., *"Hates technical jargon"*, *"Stressed about Thursday board meeting"*, *"Needs direct VP commitments"*).
* **Bespoke Personal Talk Tracks:** Record scenario-specific scripts with a Trigger, Custom Script ("Say This"), and Avoid notes.
* **Active Console Auto-Surfacing:** Whenever a recognized stakeholder is assessed on the Active Console, an expandable **Stakeholder Intelligence Banner** auto-surfaces above the tactical playbook, presenting their hot buttons and tailored scripts in real time.

### C. Commercial CRM & Sales Realignment
The **CRM & Sales** operational lens provides authentic commercial and relationship talk tracks:
* **Thinker (CRM):** Commercial milestone checklists, implementation audits, SLA credit calculations, and clear chronological deliverable roadmaps.
* **Persister (CRM):** Partnership ethics, vendor integrity, executive accountability, and long-term governance.
* **Harmonizer (CRM):** High-EQ empathy, taking personal responsibility, providing executive cover with internal VPs, and collaborative relationship preservation.
* **Rebel (CRM):** Direct candid dialogue, cutting corporate red tape, creative commercial concessions, early VIP beta access, and waived fees.
* **Promoter (CRM):** Immediate bottom-line deliverables, dedicated VP sponsor involvement, and commercial deal protection by 5 PM.
* **Imaginer (CRM):** Low-pressure 1-page asynchronous summaries, quiet review windows, and shielding the client from chaotic vendor alignment calls.

### D. Private Offline App Bundler (`Ctrl+Shift+E`)
To protect against unauthorized site cloning, the public header export button has been removed. The author and designated incident commanders can trigger the single-file self-contained domain bundler at any time using the keyboard shortcut **`Ctrl+Shift+E`** (or `Cmd+Shift+E`).

---

## 9. Live-Fire Drills & Multi-Observer Intelligence

A premier use case for **BridgeCraft** is team training exercises. When training frontline support engineers or managers in a live-fire incident simulation:

1. **Simultaneous Observation:** Multiple team members independently observe a stakeholder (e.g. an incident commander or executive actor) during the drill.
2. **Playbook Ingestion:** Observers export their markdown cards (`.md`), and the team lead uses **Import Playbooks** to ingest all files in batch.
3. **Situational Adaptation Analysis:** The Field Archive clusters the cards under the stakeholder and highlights:
   * **Base Consensus:** Percentage agreement on the stakeholder's baseline channel.
   * **Situational Adaptation:** Variations across environments (*"Promoter Phase during high-pressure outages vs. Thinker Phase during 1-on-1 reviews"*).
4. **Typo & Alias Consolidation:** If different observers enter *"Sarah (VP)"*, *"Sarah"*, or make a typo like *"Sarha"*, the **Merge Duplicate Record** utility merges them into a single assessment record while retaining all historical observer logs.

---

## 10. Ethical Code & Field Guidelines

> *"The purpose of BridgeCraft is not manipulation, labeling, or pigeonholing. The purpose is empathy in high-friction environments."*

1. **The Platinum Rule:** The Golden Rule says *"Treat others how you want to be treated."* The Platinum Rule of incident management says *"Treat others how they need to be treated to stay calm and functional."*
2. **Assessments are States, Not Life Sentences:** A person's phase shifts depending on sleep, pressure, life circumstances, and organizational safety. Always assess the *interaction*, not just the *person*.
3. **Strict Client-Side Privacy:** This application runs 100% locally in browser memory. No data, names, notes, or assessments are ever transmitted over a network.

---

## 11. Intellectual Property, Independent Authorship & Workplace Notice

**Copyright (c) 2026 Jack Likert. All Rights Reserved.**

### Declaration of Independent Invention:
This Software (BridgeCraft, formerly known as The Behavioral Profiler), documentation, heuristics, scoring engine, and architecture were conceived, authored, and reduced to practice solely and independently by **Jack Likert** on personal, non-work time, utilizing exclusively personal equipment, personal software licenses, and personal resources, without the use of any employer, client, or third-party facilities, equipment, supplies, confidential information, trade secrets, or funding.

### Not a Work Made for Hire & Workplace Disclaimer:
1. **Not a Work-for-Hire:** Under no circumstances shall this Software, or any portion thereof, be construed as a "work made for hire" under the United States Copyright Act (17 U.S.C. § 101) or any international equivalent.
2. **Workplace Demonstration:** The Author may demonstrate, pilot, or share this tool within workplace environments, incident response teams, or live-fire drills for non-commercial evaluation. **Such demonstration, hosting, or use does not convey, assign, license, or transfer any intellectual property rights, shop rights, patent rights, or claims of ownership to any employer, client, corporation, or entity.**
3. **Evaluation License:** Individual support personnel and incident commanders are granted a limited, personal, non-exclusive, revocable license to execute the Software for non-commercial incident triage and team training. All other rights, including commercial redistribution, sublicensing, or integration into proprietary enterprise products, are strictly reserved by Jack Likert.

See the [LICENSE](file:///c:/profiler/LICENSE) file for the complete legal terms.
