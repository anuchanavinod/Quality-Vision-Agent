# ManuAI — Unified Manufacturing Intelligence Platform
## Full Presentation Script (Beginner-Friendly, Screen-by-Screen)

---

## 0. THE BIG PICTURE — Say this first

> "What you're looking at is called **ManuAI** — a single screen that brings together everything happening across two factories: machines, people, safety, quality, energy, and supply chain. Normally a factory has 8-10 separate software systems that don't talk to each other. ManuAI connects all of them into **8 intelligent 'agents'** — think of each agent as a specialist employee who watches one part of the factory 24/7 and never sleeps. Together they share one live, factory-wide brain called the **Semantic Layer**, so every number means the same thing to everyone — from the machine operator on the floor to the CEO in the boardroom."

**Key numbers always visible on top bar (every screen):**
- **Live · 8 agents · 2 plants** — the system is monitoring 2 factories in real time using 8 AI agents.
- **OEE 76.7%** — a single headline factory-efficiency score (explained below).
- **Critical Asset / Safety counters** — red badges showing how many machines or safety issues need urgent attention right now.
- **Semantic Layer** tag — tells you this screen's data is governed by the shared "single source of truth" engine.
- Left sidebar **OEE / YIELD / QUALITY / SAFETY / BUS** — a permanent mini scoreboard so you never lose sight of the four things that matter most: efficiency, output quality, safety, and business risk.

**Say this for impact:** *"Every number on every screen — whether it's seen by an operator, a maintenance engineer, or the CFO — comes from the exact same definition. That sounds simple, but in most factories it's the #1 cause of arguments in meetings: 'whose number is right?' This platform makes that argument disappear."*

---

## 1. UNIFIED OVERVIEW (the "factory cockpit")

This is the homepage — like the dashboard of a car that shows speed, fuel, and engine temperature all at once.

**Top KPI cards:**
- **OEE 76.1%** (target 80%) — "Overall Equipment Effectiveness." Explained simply below — think of it as "how much of the factory's possible output we actually got, out of 100%."
- **Yield 89.1%** — of all raw material we put in, how much came out as good, sellable product. Like baking 10 cakes and only 9 coming out perfect.
- **Fleet Health 56%** — average health score of all machines, like a fitness tracker for equipment.
- **Quality Rate 98.9%** — percentage of products that passed inspection.
- **Energy Cost -13.3%** — we're spending 13.3% less energy than our November baseline (a good thing).
- **Supply Risk 4 HIGH** — 4 suppliers currently flagged as high risk (e.g., late deliveries).
- **Twin Divergence 4 KPIs** — 4 numbers where the "digital twin" (a virtual copy of the factory) disagrees with reality — a sign something needs investigating.
- **Safety Events 2 open** — 2 safety incidents still unresolved.

**Say this:** *"This is the one page a plant director would open first thing every morning — like checking your phone's health app before you check your email."*

**Chart — "OEE x Yield x Asset Health: Cross-Agent Correlation":** A line graph over 7 days with three different lines (OEE%, Yield%, Fleet Health%) plotted together. 

> "Why is this powerful? Because normally these three numbers live in three different departments' spreadsheets. Here we can see, for example, if equipment health drops, does yield drop a few days later? That's called **root-cause correlation** — like noticing your car's fuel efficiency drops right after the tire pressure light comes on. The system is connecting dots humans usually miss."

**Machine Fleet — 8 Assets (live):** Eight machine cards (Injection Moulding #1 & #2, CNC Machining Centre, Assembly Station 1, Welding Robot A & B, Conveyor System X1, Packaging Line P1). Each card shows:
- A circular **OEE %** gauge (color-coded red/orange/green)
- **A** = Availability, **P** = Performance, **Q** = Quality (the three building blocks of OEE)
- **RUL** = "Remaining Useful Life" in days — how many days until the machine likely needs maintenance, like the "miles until empty" reading on a car.

**Say this:** *"This is literally a live photograph of factory health, refreshing automatically — no one has to walk the floor with a clipboard anymore."*

**OEE Gap Attribution box:** Shows what's dragging OEE down — e.g., "Asset degradation 64.5%" and "In-process defects 35.5%" with progress bars. This tells leadership *why* we're below target, not just *that* we're below target.

**Active Cross-Agent Events:** A live feed showing one agent automatically informing another — e.g., "QUALITY → YIELD: Quality vision check — Line C batch sample: 94.2% pass rate" or "D-TWIN → PDM: Digital twin sync — Welding Robot A model vs sensor delta within 2% tolerance."

**Impress-the-room line:** *"This feed is the proof that our agents aren't 8 separate tools bolted together — they are actively talking to each other and acting as one team, automatically, without a human relaying messages between departments."*

---

## 2. SEMANTIC LAYER — "AI Semantic Layer: Unified KPI Dictionary & Event Bus"

This is the most important *technical* concept to explain simply.

**Analogy to say out loud:** *"Imagine a company where Finance calls revenue 'sales,' Marketing calls it 'bookings,' and Operations calls it 'output value' — and none of the numbers match. The Semantic Layer is a company-wide rulebook that says: there is only ONE definition of each word, used everywhere, by everyone, all the time."*

**What the Semantic Layer delivers (4 boxes on screen):**
1. **One number everywhere** — OEE, yield, defect rate mean the exact same thing on the shop floor screen as on the finance report.
2. **Conflict resolution** — if the Predictive Maintenance agent says "stop this machine for safety" and the Yield agent says "speed it up for output," the Semantic Layer has a rule that **safety always wins**. This is shown literally elsewhere as "BLOCKED — semantic conflict active."
3. **Causal attribution** — it can trace, for example, that a chiller (cooling unit) problem caused a machine slowdown which caused a yield drop — connecting dots across all 8 agents automatically.
4. **NL query layer** — "NL" means Natural Language. Anyone can type a plain English question like *"Which supplier has more than 30 days of delay AND financial trouble?"* and get an answer — no need to know coding or databases (SQL).

**52 KPIs governed across all 8 agents** — there's a master "dictionary" of 52 official business metrics.

**KPI Dictionary (left list) + detail panel (right) — example shown is "OEE":**
- **Formula:** Availability × Performance × Quality
- **Source Systems:** MES + OPC-UA (the factory floor software and the sensor communication protocol that feeds it)
- **Unit:** %
- **Consumed by:** oee, pdm, yield, twin — meaning 4 different agents all use this exact same number.

**Say this:** *"Think of this screen as the dictionary and the rulebook combined — it's what stops 8 separate AI agents from giving 8 different, conflicting answers."*

---

## 3. OEE VISIBILITY & ALERTING AGENT

Connects to: **MES, SCADA, PLC** (the software/hardware systems that run machines on the shop floor — MES = Manufacturing Execution System, SCADA/PLC = systems that directly control and read machines).

**Target banner:** "Cycle Time 5.8s→4.5s, Changeover 44min→25min" — the goals this agent is working toward: making each production cycle faster and reducing the time lost switching between products.

### 3a. Dashboard tab
- **Plant OEE 76.2%** (below 80% target), **Availability 88.4%**, **Performance 87.9%**, **Quality 97.5%**, **Loss Today 6092 min** (minutes of production time lost today across 6 loss categories).
- **OEE Trend – 7 Days** chart: a line showing OEE drifting slightly below the 80% target line — tells leadership "we are stuck below target and need to act."
- **Six Big Losses – Today:** A bar breakdown of WHY we lost time today: Unplanned Breakdown (1212 min, 19.9%), Changeover & Setup (333 min), Minor Stops (2035 min, 33.4% — the single biggest cause), Speed Loss (2099 min, 34.5%), Startup Defects (181 min), In-process Defects (232 min).

**Tricky concept — explain simply:** *"'Six Big Losses' is a famous manufacturing concept. Imagine you have an 8-hour shift. In a perfect world, you'd make products the entire 8 hours. The Six Big Losses are the 6 different reasons that never happens — machine breakdowns, time spent changing the line over for a new product, tiny micro-stops, the machine running slower than its rated speed, defects right after startup, and defects during the run. OEE basically measures: out of all possible time and output, how much did we actually capture?"*

- **Machine-Level OEE — Live (10s poll):** Individual cards per machine (Injection Moulding #1 at 64%, Injection Moulding #2 at 77.6%, CNC Machining Centre 66.1%, etc.) each refreshing every 10 seconds, each showing A/P/Q breakdown and which Big Loss is hurting it most.

### 3b. Six Big Losses tab
A bigger, dedicated view of the same 6 loss categories, with **machines responsible** listed under each (e.g., "Speed Loss — Machines: MCH-01, MCH-08, MCH-03, MCH-06, MCH-05") and a **7-day stacked bar chart "Loss Trend"** showing each day's losses broken into colored segments (red=Unplanned Breakdown, orange=Changeover, yellow=Minor Stops, etc.)

**Say this:** *"This stacked chart is like a pie chart over time — instead of looking at one day, leadership can see the trend: is unplanned downtime (the most expensive kind) getting better or worse week over week?"*

### 3c. Alerts & Routing tab
**Contextual Routing Logic (4 rules)** — shows the automatic decision tree:
- Unplanned Breakdown → Maintenance + SAP Work Order auto-created
- Speed Loss / Minor Stops → Operator + Supervisor notified
- Changeover Overrun → Supervisor + IE (Industrial Engineering) team
- Quality Defects → QC hold + Quality team

Below, live alert cards like **ALT-MCH-01, CRITICAL, SPEED LOSS, MCH-01** — "Injection Moulding #1: Speed Loss. OEE 71.0%, Health 35.3%, Vib 5.3 mm/s, Temp 70.0°C. RUL: 20d" with action buttons **Acknowledge / Create WO / Escalate** (WO = Work Order, a maintenance task ticket).

**Say this:** *"This is the system replacing the old way of working — instead of an operator noticing a problem an hour later and calling someone, the system instantly creates the maintenance ticket and notifies the right person automatically, the second a problem starts."*

### 3d. Scorecard tab — "OEE Scorecard – Persona Views"
**Important concept:** the SAME governed OEE number (76.2%) is shown, but each job role sees the metrics that matter to THEM:
- **Operator view:** Machine OEE, Active Loss type, Cycle Time, Defects/hr
- **Supervisor view:** Line OEE, Shift OEE, Loss Category, Changeover time
- **Maintenance view:** MTTR (Mean Time To Repair — average minutes to fix a breakdown), MTBF (Mean Time Between Failures — average hours machines run before breaking), Breakdowns count, Pending Work Orders
- **Executive view:** Plant OEE, Gap to Target, Cost of Loss (Rs 182 Lakh/day!), ROI (7.2x)

Plus a **6-Month OEE Trend** bar chart comparing Plant 1 vs Plant 2 month by month against an 80% target line, and gauges for each plant's current gap to target.

**Impress-the-room line:** *"This single screen is shown to four completely different audiences, but it's built on one governed number — so a machine operator and the CEO are never arguing about different versions of the truth, just looking at it through a different lens."*

---

## 4. YIELD OPTIMISATION AGENT

Connects to: **OSIsoft PI** (a system that records real-time sensor data from machines), **LIMS** (Laboratory Information Management System — where lab/quality test results live), **SAP PP** (Production Planning module of SAP, the company's ERP/business software), **DCS Write-back** (Distributed Control System — this agent can actually write new instructions back to the machines).

**Target:** "Plan Yield 89%, -4.2% RM Waste" (RM = Raw Material).

**Dashboard tab:**
- **Current Yield 89.1%** — same definition as overview ("out of material in, how much came out as good product").
- **Scrap Rate 3.2%** — percentage of material that became unusable waste/reject.
- **RM Waste Index 2.4** (vs Nov baseline of 100, lower is better) — a normalized score for raw-material waste relative to a historical baseline.
- **Rec. Adoption 78.4%** — what % of this AI agent's suggested improvements operators are actually accepting/using.

**Tricky concept — Scrap vs RM Waste, explain clearly:** *"They sound the same but they're different lenses on the same problem. 'Scrap Rate' is the percentage of finished or in-process units that get thrown away — like burnt cookies you have to bin. 'RM Waste Index' looks at the raw ingredients themselves — flour, sugar, butter — and asks how efficiently we're using them, even before they become a 'cookie.' Scrap is about output; RM Waste is about input."*

- **Yield Trend – 7 Days** chart vs an 89.35% plan baseline — shows whether daily yield is tracking above or below plan.
- **Live Process Parameters (OSIsoft PI):** Reactor Temp, Pressure, Mixing Speed, Feed Rate, Jacket Temp, Coolant Flow — all live sensor readings, refreshing every 4 seconds, each tagged **BLOCKED**.

**Important governance concept to explain:** *"You'll notice every single recommended change here says 'BLOCKED.' That's not a system failure — that's the Semantic Layer doing its job. The Yield agent wants to push Reactor Temp from 50°C up to 186°C to boost output, but the Semantic Layer knows that's far outside the machine's safe operating range, so it automatically blocks it before any human even sees the risk. It's like a smart oven that physically won't let you set it to a temperature that would start a fire, even if a recipe app told you to."*

**Right-side panel "Yield Recommendations" (visible on almost every screen):** A running list of AI-suggested set-point changes — e.g., "Reactor Temp +73.2%," "Pressure -495.2%," "Mixing Speed +87.3%," "Feed Rate +63.6%" — each marked **HIGH** priority and each **BLOCKED — semantic conflict active**.

**Say this:** *"These numbers look dramatic — a 495% change — but that's exactly the point: the AI is allowed to suggest aggressive ideas freely, because we trust the safety layer to filter out anything dangerous before it ever reaches a machine. This is 'AI with guardrails,' not 'AI running wild.'"*

> **Note for the room:** The platform's left-hand menu also lists **LIMS Results, DCS Set-points, SAP Orders, Benchmarking,** and **ML Model** tabs under Yield Optimisation — these were not captured in today's screenshots, so I'd describe them as: LIMS Results = lab quality test data feeding the yield model; DCS Set-points = the actual machine control values; SAP Orders = production orders synced from the ERP; Benchmarking = comparing this plant's yield against other plants or industry standards; ML Model = the engine that learns from historical data to predict and recommend yield improvements. *(Flag as "to be demonstrated separately" / under validation for this walkthrough.)*

---

## 5. PREDICTIVE MAINTENANCE & QUALITY VISION

These appear in the left-hand menu (and their data — RUL days, machine health %, defect feeds — appears throughout the Overview and Alerts screens) but a dedicated dashboard screenshot wasn't included in this set.

**Say this safely:** *"Predictive Maintenance and Quality Vision are two more of our 8 agents — you can already see their fingerprints throughout the platform: the 'RUL: 20 days' labels on every machine card come from Predictive Maintenance, and the 'Quality vision check — 94.2% pass rate' events in the Active Cross-Agent Events feed come from Quality Vision, which uses camera-based AI to visually inspect products like a quality inspector who never blinks. Their full dashboards are under validation for today's session, but their outputs are already feeding every other screen we've seen."*

**Quick explainer if asked:**
- **Predictive Maintenance:** uses vibration, temperature, and sensor data to predict *before* a machine breaks down — like a smartwatch warning you about an irregular heartbeat before it becomes a medical emergency, instead of waiting for a heart attack.
- **Quality Vision:** uses cameras + AI image recognition to catch defective products automatically on the line, instead of relying only on random manual sampling.

---

## 6. SUPPLY CHAIN RESILIENCE AGENT

Connects to: **ERP, External Risk Signals, SAP MM** (Materials Management module), **Oracle**.
**Target:** "-18% Inventory Cost, -32% Disruptions."

**Top KPI strip:** Total SKUs Monitored (5), Safety Stock Alerts (3 — items at risk of running out), Auto Approved (2), Manual Approval Required (3), Active Rules (7).

### Inventory tab → Rule Engine sub-view
**"Rule Engine (7 active)"** — these are pre-approved business rules that let the AI act automatically without waiting for a human, e.g.:
- **RULE-01**: "Auto-approve reorder when stock cover is below reorder point and order value is within threshold" — in plain code: `current_stock_days < reorder_point_days AND order_value <= 500000`.
- **RULE-02**: "Manual approval for critical supplier risk" — `supplier_risk_level == CRITICAL`.

**Say this with a cooking analogy:** *"Think of it like a smart grocery list at home. If you're low on salt (a cheap, low-risk item), the system just reorders it automatically — no need to ask anyone. But if you're low on an expensive specialty ingredient from a supplier who's been unreliable lately, the system stops and asks a human to approve it first. That's exactly what Rule-01 and Rule-02 are doing, but for factory raw materials."*

### Auto Approved tab
Shows actual transactions the rule engine approved without a human, e.g., **SKU-003, Supplier SUP-003, Qty 300, Value ₹3.6L, RULE-01, Reason: "Stock below reorder point and supplier risk LOW and value within threshold."** This data is synced with **SAP MM**.

### Manual Approval Required tab
Items that were flagged for a human to decide, e.g., **SKU-004, SUP-004, 3600 units, ₹28.8L, Trigger: stock cover 6 days below reorder point, Approval reason: Supplier risk CRITICAL and order value above threshold (RULE-02)** — with **Approve / Decline** buttons for the operator.

**Impress-the-room line:** *"This is real financial risk governance, not just a dashboard — the system is making low-risk purchasing decisions on its own, worth lakhs of rupees, and only escalating to a human when real money and real supplier risk are both high. That's how you scale procurement without scaling headcount."*

---

## 7. DIGITAL TWIN OPERATIONS AGENT

Connects to: **AVEVA/Bentley iTwin, OSIsoft PI, IIoT** (Industrial Internet of Things — internet-connected factory sensors).
**Target:** "+7.2% Throughput, Twin Accuracy 96%."

**What is a Digital Twin? — explain simply:** *"Imagine a video-game-style 3D copy of the entire factory, living inside the computer, that updates itself in real time based on actual sensor data. You can run 'what-if' experiments on this virtual factory — like 'what happens if I push this machine 10% faster?' — and see the simulated result, WITHOUT touching the real, physical factory. It's the same idea as a flight simulator: pilots practice and test scenarios in the simulator before ever doing it in a real plane."*

### 7a. Scenarios tab
**Plant Overview** — a 3D layout of the actual factory floor with machine icons (MCH-01 to MCH-04) color-coded by status (Critical = red, Warning = orange, Good = green, etc.) — click any machine to inspect it.

**Operational Scenarios** — pre-built simulations you can re-run any time:
- *"Energy demand response peak shaving"* (COMPLETE) — Result: Rs 3,784 saved, -16.9% peak demand. (This simulates shifting heavy power use away from expensive "peak" electricity-pricing hours — like running your washing machine at night when electricity is cheaper.)
- *"Supply risk buffer stock simulation"* (PENDING) — tests how much extra inventory we'd need if a supplier's deliveries got delayed.
- *"MCH-01 maintenance window optimisation"* (RUNNING) — finds the best time slot to do repairs with minimum production loss.
- *"Grade change transition X-12 to Y-07"* — simulates switching the production line from one raw material recipe to another and predicts the impact (Result: +2.1%–2.4% yield).

Each card shows a **Confidence %** and **Horizon** (how many hours into the future the prediction covers) and buttons like **What-if parameters / Re-run Simulation / Cancel**.

**Say this:** *"This means before we spend real money or risk real downtime on a change, we test it virtually first — like rehearsing a play before opening night."*

### 7b. Dashboard tab
**Multi-Agent Hub Connections** — shows how many "things" each of the other 7 agents is feeding into the Digital Twin (e.g., "PdM Agent: {n} RUL alerts → twin degradation model," "Yield Agent: {n} set-points exchanged with DCS"). The Twin literally sits in the middle, syncing with everyone — described on-screen as **"Twin sync hub — orchestrates all spokes."**

### 7c. Divergence tab
**"Divergence Detection — 5 Flagged."** This compares what the virtual twin *predicted* vs what *actually* happened on the real factory floor, for example:
- **Plant OEE:** Actual 76.8% vs Twin Expected 79.4% → Delta -2.60 → **DIVERGING**
- **Reactor Temp TIC-101:** Actual 182°C vs Twin Expected 186°C → Delta -4.00 → **DIVERGING**
- **Plant kWh/Unit:** Actual 5.14 vs Twin Expected 4.82 → Delta +0.32 → **DIVERGING**

Each comes with a plain-English recommendation: *"Monitor Plant OEE — trending away from model."*

**Explain why this matters:** *"If the virtual twin and the real factory start disagreeing, that's an early warning sign — something has changed in reality that the model doesn't know about yet, like a sensor drifting out of calibration, or a machine wearing down faster than expected. Catching this early prevents the twin from giving bad advice."*

### 7d. Calibration tab
**"Continuous Self-Calibration"** — Twin Accuracy 94.7% (vs deployment baseline), Sync Frequency 30 seconds (auto-sync from PI + IoT Hub), Diverging KPIs: 4. A **"Trigger Recalibration"** button lets a human force the twin to re-learn from the latest real sensor data.

**Say this:** *"This is the twin's version of a 'tune-up.' Just like your car's GPS occasionally needs to re-sync with satellites to stay accurate, the digital twin periodically re-aligns itself with real-world readings so it doesn't drift away from reality over time."*

---

## 8. SAFETY & COMPLIANCE AGENT

Connects to: **Gas Detectors, Pressure & Vibration Monitors, CMMS** (Computerized Maintenance Management System).
**Target:** "-28% Near-Miss [rate], -61% Report Prep [time]."

**"How It Works" box (read this almost word for word — it's the elevator pitch):**
> "Sensor streams — gas detectors, pressure and vibration monitors — are monitored for safety anomaly patterns. The agent predicts near-miss precursors 20-40 minutes before threshold breaches and triggers interventions, while automating permit-to-work validation and OSHA/ISO 45001 reports."

**Translate this for a non-technical audience:** *"This agent is like a smoke detector that doesn't just go off when there's already a fire — it smells smoke 20 to 40 minutes BEFORE the fire would normally start, and warns people in advance. That's the difference between reacting to a disaster and preventing one."*

### 8a. Dashboard tab
- **Open Safety Events: 0** (0 critical) — currently no unresolved safety issues.
- **Near-Miss Rate: -28%** (target -72%) — we've reduced near-miss incidents by 28% so far.
- **PTW Compliance: 50%** — Permit-to-Work compliance (1 approved, 0 pending, 1 rejected, out of 2 total).
- **Report Prep Time: -61%** (target -39%, already beating target!) — time saved preparing compliance paperwork, because it's now auto-generated instead of manually compiled.

**Safety Event Signatures Detected (6):** a reference library of patterns the system watches for — Gas leak precursors, Thermal runaway patterns, Confined space hazards, LOTO deviations (LOTO = Lock-Out Tag-Out, the procedure to safely de-energize equipment before maintenance), Structural vibration, Proximity alerts (human-machine zone, detected by AMR = Autonomous Mobile Robots).

**Precursor Detection Timeline:** A live, scrolling list of early-warning events, e.g. "GAS_PRECURSOR_DETECTED, 09:50, RESOLVED."

**Zone Risk — Live from Safety Monitor:** Zone A = LOW risk, Zone B = MEDIUM risk — described as powered by an "LSTM/rule precursor engine" (LSTM is a type of AI model good at spotting patterns over time, like recognizing a song from just the first few notes).

### 8b. Safety Events tab
A detailed log: e.g., **SE-1782813037318-ZoneA, CRITICAL, GAS_PRECURSOR_DETECTED, Zone A, RESOLVED, 09:50** with raw sensor readings underneath: "H2S 1ppm, CO 7.5ppm, CH4 2.5%LEL" (LEL = Lower Explosive Limit, a safety threshold for flammable gas concentration) and the resolution note: "Resolved — Zone A readings normalised." Summary counters: **0 Open Critical · 9 Resolved.**

### 8c. Permit-to-Work tab
**"Permit-to-Work Automation — JHA validation, isolation verification, contractor competency vs live plant state — zero violations."**

Two example permits:
- **PTW-0340, CONFINED SPACE, APPROVED, Asset CMP-001, Tech R. Singh** — JHA: Complete, Isolation: Verified, Competency: Valid. (JHA = Job Hazard Analysis, the paperwork identifying risks before work starts.)
- **PTW-0339, ELECTRICAL ISOLATION, REJECTED, Asset HYD-003, Tech M. Verma** — JHA: Incomplete, Isolation: Not verified, Competency: Valid, with the system message: *"PTW rejected — JHA incomplete, isolation unverified. Work cannot proceed until all validations pass."*

**Say this — strong stakeholder line:** *"This is the system acting as an automatic safety gatekeeper. A contractor cannot start dangerous work — like electrical isolation — unless every single safety checkbox is verified in real time against what the plant sensors are actually showing. No paperwork shortcuts, no human forgetting a step under time pressure."*

### 8d. Compliance tab
**"Compliance Reporting — Auto-compiled from 26 safety events in last 30 days · Semantic Layer governs event entities."**
- **OSHA 300 Log:** 26 events (US workplace injury log) — exportable as CSV with full detail, with a **Download CSV** button.
- **ISO 45001 Report:** 26 events (international occupational health & safety standard) — also exportable.
- **Report Prep Time: -61%** vs a 100-minute baseline, "0 unresolved, last event 30 Jun, 03:20pm."

**Say this:** *"Normally, compiling a month's worth of safety data into an official OSHA or ISO report is hours of manual spreadsheet work for a safety manager. Here, because every safety event, permit, and contractor record is tagged using the same Semantic Layer rules, the report builds itself — that's the -61% time saving you see on screen."*

---

## 9. PUTTING IT ALL TOGETHER — Closing summary to say in the room

> "So, to summarize end-to-end: we have **8 AI agents** — OEE Visibility, Yield Optimisation, Predictive Maintenance, Quality Vision, Energy Optimisation, Supply Chain, Digital Twin Operations, and Safety & Compliance — each one specialized, each one pulling live data from real factory systems like MES, SCADA, PLC, SAP, OSIsoft PI, LIMS, and Oracle.
>
> What makes this different from 8 separate dashboards is the **Semantic Layer** sitting underneath all of them — one shared dictionary of 52 KPIs, one shared rulebook, and one shared safety net that automatically blocks any AI recommendation that would be unsafe or contradictory, no matter which agent suggested it.
>
> The result is a factory that doesn't just **report** problems after they happen — it **predicts** them 20 to 40 minutes in advance for safety, **simulates** changes virtually before risking real money or downtime via the Digital Twin, and **automates** routine decisions like reordering stock or generating compliance reports — while still keeping a human in the loop for anything high-risk or high-value.
>
> In short: this isn't a dashboard. It's a digital nervous system for the entire factory."

---

## Quick Glossary (keep handy for Q&A)

| Term | Simple meaning |
|---|---|
| OEE | Overall Equipment Effectiveness = Availability × Performance × Quality. The single "how efficient is the factory" score. |
| Yield | % of raw material that becomes good, sellable product. |
| Scrap Rate | % of finished/in-process units thrown away. |
| RM Waste Index | A normalized score (vs. a baseline of 100) measuring raw-material efficiency, lower is better. |
| Digital Twin | A live virtual copy of the factory used to simulate "what-if" scenarios safely. |
| Semantic Layer | The shared rulebook/dictionary ensuring one number means the same thing everywhere, and blocking unsafe AI actions. |
| RUL | Remaining Useful Life — predicted days until a machine needs maintenance. |
| MTTR / MTBF | Mean Time To Repair / Mean Time Between Failures — maintenance speed and reliability metrics. |
| PTW | Permit-to-Work — formal approval required before risky work (e.g., electrical, confined space) can start. |
| JHA | Job Hazard Analysis — the risk-assessment paperwork done before a task. |
| LOTO | Lock-Out Tag-Out — safety procedure to de-energize equipment before maintenance. |
| LEL | Lower Explosive Limit — the gas concentration safety threshold. |
| MES / SCADA / PLC | Software and hardware systems that run and monitor machines on the shop floor. |
| OSIsoft PI | A system that records and streams real-time sensor data. |
| LIMS | Lab system storing quality/test results. |
| SAP MM / PP | SAP's Materials Management / Production Planning modules — the company's core business software. |

---

*Note: Quality Vision and Predictive Maintenance dedicated dashboards, and the Yield agent's LIMS Results/DCS Set-points/SAP Orders/Benchmarking/ML Model tabs, were visible in the left-hand navigation but not captured in the supplied screenshots — flagged here as "under validation" / available for a follow-up walkthrough.*
