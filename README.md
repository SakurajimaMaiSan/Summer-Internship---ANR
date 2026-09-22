<div align="center">

# ⛏️ Talabira II & III OCP — Fleet Performance & Digital Mining Internship

**Performance Monitoring & Improvement in OB & Coal Operations through FMS & FUMS Data**

*Adani Natural Resources · Talabira II & III Open Cast Project, Odisha, India*

![Status](https://img.shields.io/badge/status-completed-brightgreen)
![Domain](https://img.shields.io/badge/domain-mining%20engineering-orange)
![Data](https://img.shields.io/badge/data-FMS%20%7C%20FUMS-blue)

</div>

---

## 📋 Overview

This repository contains the technical deliverables from a summer internship at **Adani Natural Resources**, focused on diagnosing and correcting systematic under-reporting of overburden (OB) volumes in the Fleet Management System (FMS), and identifying improvement opportunities across fleet availability, utilization, and fuel efficiency.

The centerpiece of the work is a **Dynamic Truck Factor (TF) Calibration Framework** — a weighted reconciliation model that closes the gap between FMS-estimated OB volume and independent survey (TOMPL) ground truth, which stood at **16.1%** against a CIL-mandated tolerance of **±2%**.

| | |
|---|---|
| **Intern** | Sushant Rathore |
| **Site Head** | Nabal Kishor Sharma, Talabira II & III CH |
| **Report Date** | July 2026 |
| **Data Sources** | Fleet Management System (FMS), Fuel Management System (FUMS) |

---

## 📁 Repository Structure

```
├── Talabira_Final_Report.docx              # Full technical report
├── final_ppt.pptx                          # Final presentation deck (18 slides)
├── TF_Calibration_Model.xlsx               # Dynamic TF calibration engine
├── 1__OB_Removal_FY_2026-27__xlsx.xlsx     # FY26-27 OB removal plan & tracking
├── Talabira_FMS_March2025_Final.xlsx       # Monthly FMS analysis — Mar 2025
├── Talabira_FMS_April2025_Final.xlsx       # Monthly FMS analysis — Apr 2025
├── Talabira_FMS_May2025_Final.xlsx         # Monthly FMS analysis — May 2025
└── Density_Experiment.docx                 # Supplementary lab experiment write-up
```

---

## 📑 Deliverables

### `Talabira_Final_Report.docx`
The final technical report. Covers mine and geology overview, current FMS structure and its limitations, availability–utilization–reliability analysis, Dynamic Trip Factor (TF) and 3D TLS reconciliation, CAN bus integration for measurement, and a roadmap toward digital mining.

### `final_ppt.pptx`
18-slide presentation summarizing the internship for a business audience — context, objectives, methodology, fleet performance and reliability assessment, production validation, Dynamic Truck Factor derivation, business impact, and key learnings.

### `TF_Calibration_Model.xlsx`
The core engineering contribution — a phased, auditable model for recalibrating the FMS truck factor against survey ground truth.

| Sheet | Purpose |
|---|---|
| `README` | Model purpose, usage guide, colour legend, core formulae |
| `Assumptions` | Editable global inputs — OEM truck factors, CIL tolerance, weighting rules |
| `Phase 1 – Monthly` | Months 1–12: weighted deviation calc, TF recalibration, Gate 1 check |
| `Phase 2 – Quarterly` | Months 13–36: quarterly deviation, annual TF update, Gate 2 check |
| `Phase 3 – Annual` | Month 37+: single annual audit, pass/fail against CIL tolerance |
| `Summary Dashboard` | Full 48-month TF evolution, error reduction, recovered production volume |

**Core formulae**

```
Deviation (ε)              = (V_survey − V_FMS) / V_FMS
Weighted avg deviation     = Σ(w · ε) / Σw
Recalibrated Truck Factor  = TF_old × (1 + ε_avg)
```

### `1__OB_Removal_FY_2026-27__xlsx.xlsx`
Forward-looking OB removal plan for FY 2026-27 — OB detail, Trip Factor tracking, and month-wise breakdowns (April, May '26).

### `Talabira_FMS_{March|April|May}2025_Final.xlsx`
Monthly FMS analysis workbooks. Each follows a consistent structure:

`Raw Data → Executive Summary → Availability & Utilization → Fuel Analysis → Idle Time Analysis → Production KPIs → Improvement Opportunities`

### `Density_Experiment.docx`
Lab write-up for bulk density determination (g/cm³) of mine-site rock and soil samples — topsoil, sandstone (white/red), carb shale, coal, clay — via the cup-displacement method.

---

## 🧭 Suggested Reading Order

1. **`Talabira_Final_Report.docx`** — full context, methodology, and findings
2. **`final_ppt.pptx`** — condensed executive summary
3. **`TF_Calibration_Model.xlsx`** — the core methodological contribution
4. **`Talabira_FMS_*_Final.xlsx`** — monthly data underpinning the report
5. **`1__OB_Removal_FY_2026-27__xlsx.xlsx`** — forward-looking OB plan
6. **`Density_Experiment.docx`** — supplementary lab work

---

<div align="center">

*Prepared as part of a B.Tech Mining Engineering internship, IIT (ISM) Dhanbad × Adani Natural Resources*

</div>
