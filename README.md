# From Compliance Metrics to Business Decisions  
### A Risk-Based Data Governance Dashboard for Executive Action

This repository contains the end-to-end design and implementation of a **data governance analytics dashboard** built as part of **The FP20 Analytics Challenge 34**.

The goal of the project was simple—but rarely achieved:

> **Transform data governance metrics into a decision framework leadership can actually act on.**

Using **5500 governance audit records**, this project reframes compliance from percentages and control counts into **financial risk, root causes, and prioritized remediation actions**.

---

##  Problem Statement

Most data governance dashboards fail at the executive level.

They answer:
- *What is our compliance rate?*
- *How many audits failed?*

But they don’t answer:
- **How exposed are we?**
- **Why are we exposed?**
- **What should we fix first?**

This project addresses that gap by translating governance performance into **regulatory risk exposure (€)** and **investment-driven prioritization**.

---

##  Project Objectives

- Quantify **regulatory and compliance risk in financial terms**
- Identify **structural drivers of non-compliance**
- Enable **risk-based prioritization of governance investments**
- Reposition data governance as a **strategic risk management function**

---

##  Solution Overview: The Three-Act Dashboard Framework

### **Act 1 — Establish the Baseline: How Exposed Are We?**

The first dashboard page answers the board-level question.

Key KPIs:
- **€843.82M** estimated regulatory fine exposure  
- **28.7%** non-compliance rate (↓ 13.8% YoY)
- **42.94** average compliance risk score (↓ 12.2% YoY)

Outcome:  
Compliance conversations shift from *technical controls* to **business risk and financial exposure**.

---

### **Act 2 — Break the Aggregate: Why Are We Exposed?**

Averages hide structure. This section decomposes risk into its root causes:

#### 1. **Governance Maturity Drives Risk**
- Each maturity level increase materially reduces average risk
- Largest drop occurs when moving out of Levels 1–2

#### 2. **Missing Controls Amplify Regulatory Exposure**
- Domains lacking ownership, classification, or retention controls show higher non-compliance
- GDPR relevance compounds weak governance

#### 3. **Retention Policies Quietly Inflate Risk**
- Longer retention periods significantly increase compliance risk
- Risk is driven by *duration*, not just access or quality

Outcome:  
Maturity models and control frameworks become **quantifiable risk levers**, not abstract best practices.

---

### **Act 3 — Prioritize Action: What Do We Fix First?**

This is where governance becomes **capital allocation**.

By plotting:
- **Average compliance risk**
- **Against remediation cost**

Clear investment signals emerge:
-  High-risk, low-cost domains → **Immediate action**
-  High-cost, low-impact initiatives → **Deprioritize**
-  Governance investments should be **sequenced**, not evenly distributed

---
## 📊 Live Dashboard

[![Power BI Dashboard Preview](screenshots/dashboard_overview.png)]
(Live Report](https://app.powerbi.com/view?r=eyJrIjoiMjc5NzMzOTctY2ZkYS00MWI2LWE0MmYtZTY0ODA0N2ZhNmFkIiwidCI6ImRiMjMwNmZkLWFmMjUtNGUyOS05Y2NiLWJmMjg2YWY2MjFjMCJ9))


---

##  Key Regulatory Insight: The GDPR Concentration Problem

Audit findings revealed:

- **62%** of all findings are GDPR-related
- **56.1%** of GDPR risk is concentrated in **HR**
- Poor data quality bands show **2× non-compliance rates**

**Strategic takeaway:**  
Improving governance maturity and data quality in **HR and IT** delivers the highest risk reduction per euro invested.

---

##  Technical Stack

- **Power BI** – Dashboard design & storytelling
- **DAX** – Risk scoring, financial exposure modeling
- **Data modeling** – Star schema optimized for analytics
- **Statistical analysis** – Trend, correlation, and segmentation analysis

---

##  Repository Structure

```text
├── data/
│   └── source_datasets.csv
├── models/
│   └── risk_scoring_logic.md
├── powerbi/
│   └── governance_dashboard.pbix
├── screenshots/
│   └── dashboard_pages.png
└── README.md


