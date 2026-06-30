# ManuAI Platform — COMPLETE Exhaustive Walkthrough
## Every screen, every tab, every KPI, every chart, every button explained

---

## HOW TO USE THIS DOCUMENT
This covers all 28 screenshots in full detail, agent by agent, tab by tab. Nothing is skipped — every number, every card, every chart axis, every alert line, every button is explained in plain language with the business reason behind it.

---

# AGENT 0: UNIFIED OVERVIEW

### Top global header (present on every screen of the platform)
- **ManuAI logo + "Unified Manufacturing Intelligence Platform"** — the product name.
- **Live · 8 agents · 2 plants** (green dot) — confirms the system is live, watching 2 factories using 8 specialist AI agents.
- **Topic pills:** OEE, Yield, PdM+Parts, Quality, Energy, Supply, Twin, Safety, Semantic — quick-jump tags representing each of the 8 agents plus the Semantic Layer.
- **Plant selector:** "All Plants / Plant 1 / Plant 2" — lets you view combined or individual factory data.
- **Critical Asset counter** (red) — e.g. "1 CRITICAL ASSET" or "3 CRITICAL ASSETS" — live count of machines in a dangerous/urgent state.
- **Safety counter** (red) — e.g. "2 SAFETY" — open safety events needing attention.
- **OEE badge** — e.g. "OEE 76.7%" — same headline number repeated so it's always visible no matter which agent screen you're on.
- **SEMANTIC LAYER badge** (teal) — confirms this screen's numbers are governed by the shared rulebook.
- **Left sidebar permanent scorecard:** OEE %, YIELD %, QUALITY %, SAFETY (open count), BUS (business — "critical" count) — four numbers an executive should always be able to see no matter where they click.
- **Right-hand panel (Insights / Unified AI tabs):**
  - **"SEMANTIC LAYER ACTIVE"** box: total actions blocked today (e.g. "10 actions blocked · 8 agents · Plant 1") and a breakdown like "2 pdm · 8 yield" — how many unsafe AI suggestions were auto-blocked, split by which agent proposed them.
  - **"YIELD RECOMMENDATIONS"** list with a count badge (4 or 6) — running list of AI-suggested parameter changes, each tagged HIGH priority, showing the suggested change (e.g. "Reactor Temp 49.9 → 186 °C"), and a red "Semantic Layer block active" tag if stopped for safety.

### Unified Overview — Main KPI Row (8 cards)
1. **OEE 76.1%** (target 80%) — Overall Equipment Effectiveness, the single "how efficiently is the factory running" score (Availability × Performance × Quality).
2. **Yield 89.1%** (+0.1% vs baseline) — % of raw material that became good, sellable product, and the trend vs a historical baseline.
3. **Fleet Health 56%** (3 critical assets) — average health score across all 8 machines; how many are in a critical/risky state right now.
4. **Quality Rate 98.9%** (avg all lines) — average pass rate across every production line.
5. **Energy Cost -13.3%** (vs Nov baseline) — how much more/less energy we're spending vs a November reference month.
6. **Supply Risk 4 HIGH** (shortfall alerts) — suppliers currently flagged as high risk of late or short delivery.
7. **Twin Divergence 4 KPIs** (vs digital twin) — metrics where the virtual "digital twin" model disagrees with what's actually happening on the floor.
8. **Safety Events 2 open** (2 critical · 1 PTW pending) — open safety incidents, how many are critical, and how many Permit-to-Work approvals are stuck.

### Chart: "OEE x Yield x Asset Health — Cross-Agent Correlation" (tagged SEMANTIC LAYER)
- Line chart from 23 June to 30 June 2026.
- **Left Y-axis (65 to 92):** OEE % and Yield % scale.
- **Right Y-axis (45 to 56):** Fleet Health % scale.
- **Three colored lines:** OEE % (teal/blue), Yield % (purple dashed), Fleet Health % (orange dashed).
- A horizontal dashed **"Target"** line marking the 80% OEE goal.
- Caption: "Semantic Layer: Digital twin sync — Welding Robot A model vs sensor delta within 2% tolerance" — proof this chart is actively cross-checked against the digital twin.
- **Say this:** *"You can literally watch on this one chart whether a dip in machine health a few days ago is what's now dragging OEE and Yield down — that's cause and effect, visualized."*

### Machine Fleet — 8 Assets (live) — "OEE Agent + PdM Agent shared universe"
Eight cards, one per machine: machine name + code, a circular **OEE %** gauge (red <70%, orange 70-85%, green >85%), **A** (Availability %), **P** (Performance %), **Q** (Quality %), and **RUL** (Remaining Useful Life, in days).

| Machine | OEE | A | P | Q | RUL |
|---|---|---|---|---|---|
| Injection Moulding #1 (MCH-01) | 35.5% | 88.1% | 83.5% | 96.6% | 20d |
| Injection Moulding #2 (MCH-02) | 65.7% | 94.4% | 91.5% | 98.4% | 75d |
| CNC Machining Centre (MCH-03) | 51.7% | 78.7% | 82.3% | 96.5% | 102d |
| Assembly Station 1 (MCH-04) | 79.1% | 95.8% | 94% | 99% | 101d |
| Welding Robot A (MCH-05) | 49.7% | 91.2% | 86.1% | 97.3% | 30d |
| Welding Robot B (MCH-06) | 23.2% | 71.8% | 80.6% | 96.9% | 49d |
| Conveyor System X1 (MCH-07) | 86.3% | 97.2% | 94.9% | 98.3% | 136d |
| Packaging Line P1 (MCH-08) | 56% | 89.5% | 90.2% | 97.6% | 49d |

**Say this:** *"Welding Robot B has the lowest OEE on the floor at 23.2% and only 49 days of useful life left — that's exactly the kind of machine a plant manager should look at first thing tomorrow."*

### OEE Gap Attribution box (tagged SEMANTIC)
- Subtitle: "Cross-agent root cause via Semantic Layer."
- **Asset degradation: 64.5%** (progress bar) — % of the OEE gap explained by machines wearing down.
- **In-process defects: 35.5%** (progress bar) — % of the gap explained by quality problems during the run.
- Tells leadership exactly which of two root causes to fix first, not just "OEE is low."

### Active Cross-Agent Events box ("Semantic Layer event bus")
Live list of agents passing info to each other automatically:
- **QUALITY → YIELD:** "Quality vision check — Line C batch sample: 94.2% pass rate"
- **QUALITY → YIELD:** "Quality vision check — Line A batch sample: 94.4% pass rate"
- **D-TWIN → PDM:** "Digital twin sync — Welding Robot A model vs sensor delta within 2% tolerance"
- **D-TWIN → PDM:** "Digital twin sync — Injection Moulding #1 model vs sensor delta..."

**Say this:** *"This is proof the agents are a team, not 8 separate apps — one agent's finding automatically becomes another agent's input, with no human relay required."*

---

# AGENT 1: AI SEMANTIC LAYER (the shared brain underneath everything)

- Title: **"AI Semantic Layer – Unified KPI Dictionary & Event Bus."**
- Subtitle: **"52 KPIs governed across all 8 agents"** — total size of the shared metrics rulebook.
- Buttons: **"Reload CSV"** (refresh the KPI dictionary from its source file) and **"ALL 8 AGENTS"** (filter/view toggle).

### "What the Semantic Layer delivers" — 4 explainer boxes
1. **One number everywhere:** "OEE, yield, defect rate identical for shop floor, finance and executive — across all plants."
2. **Conflict resolution:** "PdM fault blocks Yield recs. Safety precursor pauses hot-work PTW. Cross-agent safety net." (Predictive Maintenance's safety warning overrides Yield's "go faster" suggestion; a gas precursor automatically pauses hot-work permits.)
3. **Causal attribution:** "Traces CHP-002 chiller to MCH-01 speed loss to OEE to yield drop across 8 agents." (Example: a cooling-unit problem caused a machine slowdown, which dropped OEE, which dropped yield — all connected automatically.)
4. **NL query layer:** "Which supplier has >30d lead drift AND financial distress? Answered in plain English, no SQL." (Anyone can ask a plain question instead of writing database code.)

### KPI Dictionary (left list, scrollable) — example entries:
OEE (oee+pdm+yield+twin, %), Availability (oee, %), Performance (oee, %), Quality Rate (oee+quality, %), Loss Today (oee, min), Defect Rate (quality+oee, %).

### Detail panel (right) — shown for "OEE":
- **Formula:** Availability × Performance × Quality
- **Source Systems:** MES + OPC-UA
- **Unit:** %
- **Consumed by:** oee, pdm, yield, twin (4 different agents pull this exact same number rather than calculating their own).

**Say this:** *"This page is the rulebook and dictionary combined — it's literally why the OEE number on the operator's screen matches the one in the CEO's report, to the decimal point."*

---

# AGENT 2: OEE VISIBILITY & ALERTING AGENT

Connected systems: **MES, SCADA, PLC**. Target: **"Cycle Time 5.8s→4.5s, Changeover 44min→25min."**

## Tab 1: Dashboard

**Top KPI row (5 cards):**
- **Plant OEE: 76.2%** (▼ below target 80%)
- **Availability: 88.4%** (▼ -0.6% wk) — % of scheduled time the machine actually ran.
- **Performance: 87.9%** (▼ -0.4% wk) — how close to rated speed it ran while operating.
- **Quality: 97.5%** (▲ +0% wk) — % of units that passed inspection first time.
- **Loss Today: 6092 min** — total minutes of potential production lost today across all six loss types.

**Chart: "OEE Trend – 7 Days" (vs 80% target)** — line chart 06-24 to 06-30, Y-axis 65–71%, line hovering well below the dashed 80% target all week. *"We've been stuck 4-5 points under target for a full week — a pattern, not a one-off bad day."*

**"Six Big Losses – Today" mini-list:** Unplanned Breakdown 1212min (19.9%), Changeover & Setup 333min (5.5%), Minor Stops 2035min (33.4%), Speed Loss 2099min (34.5%), Startup Defects 181min (3%), In-process Defects 232min (3.8%) — each with a progress bar.

**"Machine-Level OEE – Live (10s poll)" grid** — "Drill down Plant > Line > Machine · All Plants." LINE filter: All/A/B/C/D.

| Machine | OEE | A | P | Q | Today's biggest loss |
|---|---|---|---|---|---|
| Injection Moulding #1 (MCH-01) | 64% | 83.4% | 81.5% | 94.2% | Speed Loss, 888min |
| Injection Moulding #2 (MCH-02) | 77.6% | 92.6% | 88.9% | 94.3% | Minor Stops, 863min |
| CNC Machining Centre (MCH-03) | 66.1% | 83.5% | 82.6% | 95.8% | Unplanned Breakdown, 732min |
| Assembly Station 1 (MCH-04) | 81.4% | 94.2% | 91.8% | 94.1% | Changeover & Setup, 393min |
| Welding Robot A (MCH-05) | 70.1% | 88.6% | 83.6% | 94.6% | Minor Stops, 1207min |
| Welding Robot B (MCH-06) | 64.7% | 82.1% | 83.8% | 94% | Unplanned Breakdown, 729min |
| Conveyor System X1 (MCH-07) | 84% | 95% | 94.1% | 94% | Startup Defects, 230min |
| Packaging Line P1 (MCH-08) | 72.2% | 86.9% | 87.8% | 94.6% | Speed Loss, 1050min |

**Note:** these OEE figures differ slightly from the Unified Overview's machine table — flag honestly: *"the two views show a slightly different live snapshot — likely a refresh-timing difference, under validation."*

## Tab 2: Six Big Losses (full dedicated view)
Six cards (red=worst, orange=moderate, green=minor) with minutes, event count, % of today, and responsible machines:
1. **Unplanned Breakdown:** 1212min · 2 events · 19.9% · MCH-03, MCH-06
2. **Changeover & Setup:** 333min · 1 event · 5.5% · MCH-04
3. **Minor Stops:** 2035min · 5 events · 33.4% · MCH-02, MCH-05, MCH-04, MCH-07, MCH-08
4. **Speed Loss:** 2099min · 5 events · 34.5% · MCH-01, MCH-08, MCH-03, MCH-06, MCH-05
5. **Startup Defects:** 181min · 1 event · 3% · MCH-07
6. **In-process Defects:** 232min · 6 events · 3.8% · MCH-06, MCH-08, MCH-03, MCH-02, MCH-07, MCH-04

**Chart: "Loss Trend – 7 Days"** — "Day-on-day loss minutes since OEE agent deployment." Stacked bar chart 06-24 to 06-30, Y-axis 0–14000 min, each bar split into 6 colored segments (legend: red=Unplanned Breakdown, orange=Changeover & Setup, yellow=Minor Stops, dark orange=Speed Loss, green=Startup Defects, teal=In-process Defects). *"Notice today's bar (06-30) is much shorter than the rest of the week — losses are trending down, though we'd want more days to confirm it's a real trend."*

## Tab 3: Alerts & Routing
**"Contextual Routing Logic (4 rules)":**
1. Unplanned Breakdown → Maintenance + SAP Work Order auto-created
2. Speed Loss / Minor Stops → Operator + Supervisor notified
3. Changeover Overrun → Supervisor + IE team (Industrial Engineering)
4. Quality Defects → QC hold + Quality team

**Live Alert Cards:**
- **ALT-MCH-01, CRITICAL, SPEED LOSS, MCH-01, 10:50am** — "Injection Moulding #1: Speed Loss. OEE 71.0%, Health 35.3%, Vib 5.3 mm/s, Temp 70.0°C. RUL: 20d." → Maintenance + SAP WO auto-created. Buttons: **Acknowledge / Create WO / Escalate**.
- **ALT-MCH-06, CRITICAL, SPEED LOSS, MCH-06, 10:50am** — "Welding Robot B: Speed Loss. OEE 56.0%, Health 22.4%, Vib 3.8 mm/s, Temp 63.0°C. RUL: 49d." Same routing/buttons.
- **ALT-MCH-03, WARNING, SPEED LOSS, MCH-03, 10:50am** (lower severity, partially visible).

*"Vib" = vibration, often the earliest physical sign a machine is about to fail. "Health %" is a combined score from vibration, temperature and other sensors, calculated by Predictive Maintenance.*

## Tab 4: Scorecard — "OEE Scorecard – Persona Views"
Subtitle: **"Single governed OEE definition for all roles."** Toggle: Operator / Supervisor / Maintenance / Executive — same 76.2% OEE, different lens per role.

- **Operator:** Machine OEE 76.2%, Active Loss: Speed Loss, Cycle Time 4.8s, Defects/hr 14.1
- **Supervisor:** Line OEE 76.2%, Shift OEE 78.5%, Loss Category: Speed Loss, Changeover 31min
- **Maintenance:** MTTR 49.5min (avg time to fix a breakdown), MTBF 6hrs (avg run-time before next failure), Breakdowns 2, Pending WOs 3
- **Executive:** Plant OEE 76.2%, Gap to Target -3.8%, Cost of Loss Rs 182 L/day, ROI 7.2x

**Shared chart (all 4 views): "6-Month OEE Trend"** (target 80% governed) — bar chart Jan–Jun, two bars/month (Plant 1 blue, Plant 2 teal), Y-axis 61–76. Below: gauge cards — **Plant 1: 76.2% OEE, gap -3.8%**, **Plant 2: 75.7% OEE, gap -4.3%**.

**Say this — strong line:** *"An operator, a supervisor, a maintenance engineer, and the plant's executive are all looking at the exact same governed 76.2% OEE number — they just each see the 4 metrics most relevant to their job. That's the Semantic Layer in action, not a slogan."*

---

# AGENT 3: YIELD OPTIMISATION AGENT

Connected systems: **OSIsoft PI, LIMS, SAP PP, DCS Write-back.** Target: **"Plan Yield 89%, -4.2% RM Waste."**

## Tab: Dashboard
**Top KPI row:**
- **Current Yield: 89.1%** (▲ +/-0.3% vs baseline)
- **Scrap Rate: 3.2%** — % of material/output thrown away as waste.
- **RM Waste Index: 2.4** (vs Nov baseline = 100, lower is better) — normalized raw-material efficiency score.
- **Rec. Adoption: 78.4%** — % of this agent's AI recommendations operators actually accepted and used.

**Chart: "Yield Trend – 7 Days"** (vs 89.35% plan baseline) — line chart 06-24 to 06-30, Y-axis 82.3–91.4%, dips mid-week then recovers above baseline by 06-30.

**"Live Process Parameters (OSIsoft PI)"** — "4s refresh · Semantic Layer blocks unsafe recs" — tag "6 BLOCKED": Reactor Temp 50°C, Pressure 50.2 bar, Mixing Speed 50 RPM, Feed Rate 50 kg/hr, Jacket Temp 49.8°C, Coolant Flow 49.8 (units cut off on scroll) — all tagged **BLOCKED**.

**Right panel: "YIELD RECOMMENDATIONS"** (badge 4-6) — each card: parameter, HIGH tag, suggested % change, current→suggested value, red **"Semantic Layer block active"** tag:
- **Reactor Temp +73.0–73.2%** — ~50 → 186°C — BLOCKED
- **Pressure -492.9% to -497.6%** — ~50 → 8.4 bar — BLOCKED
- **Mixing Speed +87.3–87.4%** — ~50 → 395 RPM — BLOCKED
- **Feed Rate +63.6–63.9%** — BLOCKED

**Explain the BLOCKED pattern:** *"Every recommendation is blocked — that's the system working as designed. The Yield AI wants to push reactor temperature from 50°C to 186°C because mathematically that boosts output, but the Semantic Layer knows that's outside the equipment's safe range, so it vetoes it automatically — like a car's parking sensor stopping you before you reverse into a wall, even if your foot is still on the accelerator."*

> The Yield agent's menu also lists **LIMS Results, DCS Set-points, SAP Orders, Benchmarking, ML Model** tabs — not captured in these screenshots, flagged as "to be demonstrated separately." Quick meaning if asked: LIMS Results = lab test data; DCS Set-points = actual live machine control values; SAP Orders = production orders synced from ERP; Benchmarking = comparing this plant vs others/industry; ML Model = the predictive engine behind the recommendations.

---

# AGENT 4: SUPPLY CHAIN RESILIENCE AGENT

Connected systems: **ERP, External Risk Signals, SAP MM, Oracle.** Target: **"-18% Inventory Cost, -32% Disruptions."** Nav tabs: Dashboard, Risk Monitor, Demand Forecast, **Inventory** (captured in detail).

## Tab: Inventory
**Top KPI row:**
- **Total SKUs Monitored: 5** (across all plants) — SKU = Stock Keeping Unit, a unique inventory item code.
- **Safety Stock Alerts: 3** (adjustment needed) — items at risk of falling below the safe minimum stock level.
- **Auto Approved: 2** (rule-engine approved) — reorders approved automatically.
- **Manual Approval Required: 3** (awaiting operator) — reorders waiting for a human decision.
- **Active Rules: 7** (governance enabled) — total automated business rules currently live.

**Filter toggles:** Safety Stock Alerts (3) / Manual Approval Required (3) / Auto Approved (2) / Rule Engine (7).

**Sub-view: "Rule Engine (7 active)"** — "Governance rules deciding auto vs manual approval" (SEMANTIC LAYER tag, "+ New Rule" button):
- **RULE-01: "Auto-approve below reorder point under threshold"** (INVENTORY, AUTO APPROVAL, ALL PLANTS) — used 42x, last 2026-06-24. Logic: `current_stock_days < reorder_point_days AND order_value <= 500000`. Meaning: if stock is low AND the order is cheap enough, approve automatically.
- **RULE-02: "Manual approval for critical supplier risk"** (SUPPLIER RISK, MANUAL APPROVAL, ALL PLANTS) — used 9x, last 2026-06-22. Logic: `supplier_risk_level == CRITICAL`. Meaning: if the supplier is CRITICAL risk, a human must approve regardless of order size.
- Each rule has a **Disable** button.

**Sub-view: "Auto Approved Orders (2)"** (SAP MM tag, date-range filter). Columns: SKU | Supplier | Qty | Value | Rule/SAP | Reason.
- **SKU-003 (P1), SUP-003, Qty 300, ₹3.6L, RULE-01, "PR Created"** — "Stock below reorder point and supplier risk LOW and value within threshold." (PR = Purchase Requisition.)
- **SKU-005 (P2), SUP-005, Qty 8, ₹0.7L, RULE-01, "Completed"** — same reasoning.

**Sub-view: "Manual Approval Required (3)"** — "Reorders routed to operator before SAP MM PR" (GOVERNANCE tag, date filter):
- **SKU-004, SUP-004 (P2), AI AGENT, Qty 3600, ₹28.8L** — Trigger: "Stock cover 6d below reorder point 14d." Reason: "Supplier risk CRITICAL and order value above threshold (RULE-02)." Buttons: **Approve / Decline**.
- **SKU-001, SUP-001 (P1), AI AGENT, Qty 18, ₹15.1L** — Trigger: "Stock cover 8d below reorder point 15d." Reason: "Order value exceeds threshold and lead-time drift 18d (RULE-03)." Buttons: **Approve / Decline**. (References RULE-03, not shown in the Rule Engine list shown — flagged "under validation.")

**Say this — strong line:** *"This isn't just a dashboard showing problems — it's a system making real purchasing decisions worth lakhs of rupees on its own, and only stopping to ask a human when both the money AND the supplier risk are high. That frees up a procurement team's time for the decisions that actually need human judgment."*

---

# AGENT 5: DIGITAL TWIN OPERATIONS AGENT

Connected systems: **AVEVA/Bentley iTwin, OSIsoft PI, IIoT.** Target: **"+7.2% Throughput, Twin Accuracy 96%."**

**Digital Twin analogy:** *"Picture a video-game-style 3D replica of the factory living inside a computer, constantly fed real sensor data so it mirrors the real plant. You can run 'what-if' tests on this virtual copy — like a flight simulator for pilots — without touching or risking the real machines."*

## Tab 1: Scenarios
**"Plant Overview · Plant 1"** — interactive 3D-style floor map with machine icons MCH-01–04 and status dots. **Asset Status legend:** Critical (red) · Warning (orange) · Caution (yellow/orange) · Good (green) · Gas Sensor (icon). Tooltip: "Click a machine label to view details & scenarios." When no plant chosen (All Plants), a "Select a Plant" screen appears with **Plant 1**/**Plant 2** buttons.

**"Selected Asset" panel** — placeholder "Click a machine label to inspect" until a machine is clicked.

**"Operational Scenarios"** — "Plant-wide what-if — edit inputs and the twin recomputes the outcome":
1. **[energy][COMPLETE] "Energy demand response peak shaving"** — "Peak-shaving demand response simulation across the evening tariff window." Result: **Rs 3,784 saved, -16.9% peak demand.** Buttons: What-if parameters / **Re-run Simulation**.
2. **[supply][PENDING] "Supply risk buffer stock simulation"** — "Buffer-stock sizing simulation against current supplier lead-time drift." Result: **-18d lead risk.** Buttons: What-if parameters / **Run Simulation**.
3. **[maintenance][RUNNING] "MCH-01 maintenance window optimisation"** — "Finds the shift window to repair MCH-06 with minimum OEE loss across the 72h horizon." Result: **+4.2% throughput.** Buttons: What-if parameters / **Cancel**.
4. **[grade_change][COMPLETE] "Grade change transition X-12 to Y-07"** — "Simulates raw-material transition from Compound X-12 to Y-07 across a 24h window." Result: **+2.1% yield.** Buttons: What-if parameters / **Re-run Simulation**.

*"It's like asking, 'If I switch my recipe's main ingredient, how will the cake turn out?' and getting the answer instantly from a model instead of baking 100 test cakes."*

## Tab 2: Dashboard
**"Active Scenarios"** — same 4 scenarios, each with Confidence % and Horizon:
- RUNNING: Maintenance window optimisation — +4.2% throughput, Confidence 89-91%, Horizon 72h
- COMPLETE: Grade change transition X-12 to Y-07 — +2.1-2.4% yield, Confidence 88-90%, Horizon 24h
- COMPLETE: Energy demand response peak shaving — Rs 3,784 saved, -16.9% peak demand, Confidence 88%, Horizon 48h
- PENDING: Supply risk buffer stock simulation — -18d lead risk, Confidence 74%, Horizon 168h

**"Multi-Agent Hub Connections"** — "8 agents · All Plants" (button: ALL PLANTS):
- **PDM Agent:** "{n} RUL alerts → twin degradation model"
- **YIELD Agent:** "{n} set-points exchanged with DCS"
- **ENERGY Agent:** "{n} assets feeding load schedules"
- **OEE Agent:** "{n} machines feeding OEE simulation"
- **QUALITY Agent:** "{n} defects feeding quality vision model"
- **SUPPLY Agent:** "{n} high-risk suppliers tracked"
- **SAFETY Agent:** "1 open safety events · 0 PTW pending"
- **D-TWIN (self):** "Twin sync hub — orchestrates all spokes" (the Twin is the central hub all 7 other agents plug into)

Bottom banner: *"Twin state, scenario outputs, and scheduled events published via semantic layer - every downstream agent consumes twin data with consistent entity references, eliminating cross-agent semantic drift."*

## Tab 3: Divergence
**"Divergence Detection"** — "Computed twin model vs captured readings — live PI/IoT binding activates in Phase E" — badge **"5 FLAGGED."** Each card: metric, DIVERGING tag, "live" indicator, 4 columns (ACTUAL | TWIN EXPECTED | DELTA | STATUS), plus a recommendation:
1. **Plant OEE** — Actual 76.8%, Twin Expected 79.4%, Delta -2.60, **DIVERGING** — "Monitor Plant OEE — trending away from model."
2. **Reactor Temp TIC-101** — Actual 182°C, Twin Expected 186°C, Delta -4.00, **DIVERGING** — "Monitor Reactor Temp TIC-101 — trending away from model."
3. **Plant kWh/Unit** — Actual 5.14 kWh/u, Twin Expected 4.82 kWh/u, Delta +0.32, **DIVERGING** — "Monitor Plant kWh/Unit — trending away from model."
(2 more flagged metrics exist per the "5 FLAGGED" badge, cut off by scrolling.)

*"If the twin's prediction and the real factory start disagreeing, that's an early warning that something in the real world changed that the model doesn't know yet — a sensor drifting, or equipment wearing faster than expected."*

## Tab 4: Calibration
**"Continuous Self-Calibration"** — "Re-aligns the twin's reference operating point from recent sensor feeds (full model re-fit in Phase E)" — button: **Trigger Recalibration**.
- **Twin Accuracy: 94.7%** (vs deployment baseline)
- **Sync Frequency: 30s** (Auto-sync from PI + IoT Hub)
- **Diverging KPIs: 4** (vs digital twin model)

*"Just like a car's GPS periodically re-syncs with satellites, the digital twin periodically re-tunes itself against real sensor data — this button does it on demand, on top of its normal 30-second auto-sync."*

---

# AGENT 6: SAFETY & COMPLIANCE AGENT

Connected systems: **Gas Detectors, Pressure & Vibration Monitors, CMMS.** Target: **"-28% Near-Miss, -61% Report Prep."**

## Tab 1: Dashboard
**"How It Works"** banner: *"Sensor streams - gas detectors, pressure and vibration monitors - are monitored for safety anomaly patterns. The agent predicts near-miss precursors 20-40 minutes before threshold breaches and triggers interventions, while automating permit-to-work validation and OSHA/ISO 45001 reports."*

**Top KPI row:**
- **Open Safety Events: 0** (▼ 0 critical)
- **Near-Miss Rate: -28%** (▲ target -72%) — reduced 28% so far, with a more ambitious -72% goal.
- **PTW Compliance: 50%** — "1 approved · 0 pending · 1 rejected of 2."
- **Report Prep Time: -61%** (▲ target -39%, already beating goal) — time saved auto-generating compliance reports.

**"Safety Event Signatures Detected (6)"** — "Static reference — detection signature library (config)":
1. **Gas leak precursors** — "Pressure & flow anomalies, H2S sensor"
2. **Thermal runaway patterns** — "Preceding fire risk — critical assets"
3. **Confined space hazards** — "Atmospheric indicators — confined zones"
4. **LOTO deviations** — "Procedure signals — open work orders" (LOTO = Lock-Out Tag-Out)
5. **Structural vibration** — "Near fatigue limits — high-vib assets"
6. **Proximity alerts** — "Human-machine zone — AMR" (Autonomous Mobile Robot)

**"Precursor Detection Timeline"** — "20-40 minutes before threshold breach" — live feed:
GAS_PRECURSOR_DETECTED 09:50 RESOLVED · 09:37 RESOLVED · 09:35 RESOLVED (x2 more entries at 09:35).

**"Zone Risk – Live from Safety Monitor"** — "safety-monitor service · LSTM/rule precursor engine" (SERVICE tag): **Zone A: LOW**, **Zone B: MEDIUM**.

(LSTM = AI model type good at recognizing patterns over time, used to spot a leak building up before it crosses a dangerous threshold.)

## Tab 2: Safety Events
"Precursor Detection 20-40 min Advance Warning" — badges: **0 OPEN CRITICAL · 9 RESOLVED.**
- **SE-1782813037318-ZoneA, CRITICAL, GAS_PRECURSOR_DETECTED, Zone A, RESOLVED, 09:50** — "H2S 1ppm CO 7.5ppm CH4 2.5%LEL" — "Resolved — Zone A readings normalised."
- **SE-1782812237199-ZoneA, ... 09:37** — "H2S 1ppm CO 8.9ppm CH4 2.2%LEL" — same resolution.
- **SE-1782812157186-ZoneA, ... 09:35** — "H2S 1ppm CO 8.1ppm CH4 2.3%LEL" — same resolution.
- **SE-1782812127183-ZoneA, ... 09:35** — same pattern (partially visible).

*"H2S and CO are toxic gases measured in ppm (parts per million). CH4 (methane) is measured as %LEL — % of the Lower Explosive Limit, how close it is to becoming flammable. The system caught all of these before they crossed the danger line, and confirms each returned to normal."*

## Tab 3: Permit-to-Work
**"Permit-to-Work Automation"** — "JHA validation - isolation verification - contractor competency vs live plant state - zero violations":
1. **PTW-0340, CONFINED SPACE, APPROVED, Asset CMP-001, Tech: R. Singh** — JHA: **Complete** · Isolation: **Verified** · Competency: **Valid**.
2. **PTW-0339, ELECTRICAL ISOLATION, REJECTED, Asset HYD-003, Tech: M. Verma** — JHA: **Incomplete** · Isolation: **Not verified** · Competency: **Valid** — red banner: *"PTW rejected — JHA incomplete, isolation unverified. Work cannot proceed until all validations pass."*

(JHA = Job Hazard Analysis, the risk-assessment paperwork before risky work starts.)

**Say this — strong line:** *"A contractor physically cannot get clearance for electrical isolation work unless every checkbox — paperwork AND live sensor state — agrees it's safe. No shortcuts, no human forgetting a step under time pressure."*

## Tab 4: Compliance
**"Compliance Reporting"** — "Auto-compiled from 26 safety events in last 30 days · Semantic Layer governs event entities" (LIVE tag).

**"Compliance Status — 2 frameworks":**
- **OSHA 300 Log: 26 events** — "US workplace injury log — exports as CSV with full event detail." Button: **Download CSV**.
- **ISO 45001 Report: 26 events** — "ISO 45001 occupational health & safety — exports as CSV with full event detail." Button: **Download CSV**.
- **Report Prep Time: -61%** vs 100min baseline — "0 unresolved · Last event: 30 Jun, 03:20pm."

Bottom banner: *"Safety event, permit type, compliance obligation, and contractor competency entities mapped via Semantic Layer - enabling automatic OSHA and ISO 45001 report generation with zero manual aggregation."*

**Say this:** *"A safety manager normally spends hours each month manually compiling spreadsheets for audits. Because every safety event, permit, and contractor record shares the same Semantic Layer definitions, these official reports build themselves — that's the -61% time saving."*

---

# AGENTS NOT CAPTURED IN DETAIL (flagged honestly)

The left-hand navigation also lists **Predictive Maintenance**, **Quality Vision**, and **Energy Optimisation** as full standalone agents, plus the **Yield Optimisation** sub-tabs (LIMS Results, DCS Set-points, SAP Orders, Benchmarking, ML Model) and the **Supply Chain** sub-tabs (Dashboard, Risk Monitor, Demand Forecast). None had dedicated screenshots in this set — flagged as **under validation** for a follow-up session. Their *outputs*, however, already appear feeding other screens:
- **Predictive Maintenance outputs:** the "RUL: Xd" and "Health %" figures on every machine card across Unified Overview, OEE Alerts, and the Digital Twin hub.
- **Quality Vision outputs:** the "Quality vision check — Line X batch sample: XX% pass rate" events in Active Cross-Agent Events, and Quality Rate / In-process Defects figures used elsewhere.
- **Energy Optimisation outputs:** the Energy Cost -13.3% KPI on Unified Overview, and the "Energy demand response peak shaving" scenario inside Digital Twin Ops.

**Quick explainer if asked:**
- **Predictive Maintenance** = forecasts machine failures before they happen using vibration/temperature/sensor trends — like a smartwatch flagging an irregular heartbeat before it becomes an emergency.
- **Quality Vision** = cameras + AI image recognition inspect every product visually instead of only random manual sampling — an inspector that never blinks and checks 100% of output.
- **Energy Optimisation** = shifts/reduces power usage (e.g. running heavy equipment during cheaper off-peak hours) to cut electricity cost without cutting output.

---

# CLOSING SUMMARY — say this last

> "Across all 8 agents — OEE Visibility, Yield Optimisation, Predictive Maintenance, Quality Vision, Energy Optimisation, Supply Chain Resilience, Digital Twin Operations, and Safety & Compliance — every KPI you've seen today, whether a 76.2% OEE number, a 'BLOCKED' yield recommendation, a rejected Permit-to-Work, or an auto-approved purchase order, is governed by the same Semantic Layer: one dictionary of 52 KPIs, one event bus connecting all 8 agents, and one safety net that vetoes anything risky before it reaches the real factory.
>
> The result isn't 8 dashboards bolted together — it's one factory-wide nervous system that predicts problems 20-40 minutes before they happen for safety, simulates changes virtually before risking real downtime or money via the Digital Twin, and automates routine decisions — purchase orders, compliance reports, maintenance tickets — while still keeping a human in control of anything high-risk or high-value."

---

## Full Glossary (every technical term used across all screens)

| Term | Plain meaning |
|---|---|
| OEE | Overall Equipment Effectiveness = Availability × Performance × Quality |
| Availability | % of scheduled time the machine actually ran |
| Performance | How close to rated speed the machine ran while operating |
| Quality (OEE component) | % of units that passed first-time inspection |
| Yield | % of raw material that became good, sellable output |
| Scrap Rate | % of output thrown away as waste |
| RM Waste Index | Normalized raw-material efficiency score vs a baseline of 100 |
| Rec. Adoption | % of AI suggestions operators actually accepted |
| RUL | Remaining Useful Life — predicted days until maintenance needed |
| MTTR | Mean Time To Repair |
| MTBF | Mean Time Between Failures |
| WO | Work Order — a maintenance task ticket |
| SKU | Stock Keeping Unit — a unique inventory item code |
| PR | Purchase Requisition — internal request to buy something |
| PTW | Permit-to-Work — formal approval required before risky work begins |
| JHA | Job Hazard Analysis — risk paperwork done before a task |
| LOTO | Lock-Out Tag-Out — procedure to de-energize equipment safely |
| AMR | Autonomous Mobile Robot |
| LEL | Lower Explosive Limit — gas concentration safety threshold |
| ppm | Parts per million — gas concentration unit |
| H2S / CO / CH4 | Hydrogen sulfide / carbon monoxide / methane — gases monitored for leaks |
| LSTM | An AI model type good at recognizing patterns over time |
| Digital Twin | Live virtual copy of the factory for safe "what-if" testing |
| Semantic Layer | Shared rulebook/dictionary ensuring one consistent number + safety vetoes everywhere |
| MES / SCADA / PLC | Software/hardware that runs and monitors shop-floor machines |
| OSIsoft PI | Real-time sensor data historian system |
| LIMS | Lab system storing quality/test results |
| SAP MM / PP | SAP's Materials Management / Production Planning modules |
| DCS | Distributed Control System — directly controls machine set-points |
| ERP | Enterprise Resource Planning — core business software (e.g. SAP, Oracle) |
| IIoT | Industrial Internet of Things — connected factory sensors |
| CMMS | Computerized Maintenance Management System |
| NL query | Natural Language query — plain English questions instead of code |
