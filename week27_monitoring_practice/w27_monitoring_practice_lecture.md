# Unit 24: Project Management for Engineers
## Week 27 — Monitoring Practice
### Cambridge TECHNICALS Level 3 Engineering

---

**Week:** 27 | **Session Type:** Tutorial | **Duration:** 60 minutes  
**Learning Outcome:** LO5 — Understand how and why engineering projects are monitored  
**Date:** 22 April 2026

---

## Table of Contents

| # | Section | Time | LO Reference |
|---|---------|------|--------------|
| 1 | [Learning Objectives](#1-learning-objectives) | 2 min | LO5 |
| 2 | [Introduction: Why Monitoring Practice Matters](#2-introduction-why-monitoring-practice-matters) | 5 min | LO5.1 |
| 3 | [Status Reports: Purpose, Structure and Formats](#3-status-reports-purpose-structure-and-formats) | 12 min | LO5.1 |
| 4 | [Time, Cost and Quality Creep](#4-time-cost-and-quality-creep) | 10 min | LO5.1 / LO5.2 |
| 5 | [Variance Analysis in Practice](#5-variance-analysis-in-practice) | 15 min | LO5.1 |
| 6 | [Escalation Procedures](#6-escalation-procedures) | 8 min | LO5.1 |
| 7 | [Change Control](#7-change-control) | 6 min | LO5.1 |
| 8 | [Conclusion and Summary](#8-conclusion-and-summary) | 2 min | LO5 |
| — | [References](#references) | — | — |

---

## 1. Learning Objectives

**⏱ 2 minutes | LO5**

By the end of this session, students will be able to:

- Describe the purpose and key components of a project status report.
- Explain the concepts of time creep, cost creep and quality erosion, and identify how each manifests in engineering projects.
- Complete and interpret a variance analysis table, distinguishing between favourable and adverse variances.
- Describe a structured escalation procedure and explain when it should be triggered.
- Outline a change control process and explain why it is essential for maintaining project integrity.

> **Exam note:** Variance analysis (LO5.1) has appeared as a structured data question in multiple OCR examination series. Ensure confidence in calculating percentage variances and labelling them correctly as adverse or favourable.

[↑ Return to Table of Contents](#table-of-contents)

---

## 2. Introduction: Why Monitoring Practice Matters

**⏱ 5 minutes | LO5.1**

Monitoring is the structured activity of comparing actual project performance against the plan in order to detect deviation, trigger corrective action, and maintain control (Association for Project Management, 2019). It is not a passive activity: effective project managers actively interrogate data, communicate findings and make decisions throughout the project lifecycle.

In engineering contexts, the consequences of poor monitoring are well documented. The National Audit Office (2020) review of HS2 Phase One cited inadequate cost and schedule tracking as a primary contributor to the project's substantial budget overruns. Similarly, the Independent review of the Edinburgh Trams project (Hardie, 2011) identified the absence of a robust change control and escalation framework as a key systemic failure.

Monitoring encompasses three interconnected activities:

```
  PLAN  ──────>  MONITOR  ──────>  CONTROL
  (Baseline)     (Compare)         (Correct)
      ^                                 |
      |_________________________________|
             Continuous feedback loop
```

This session consolidates the monitoring tools and techniques introduced in Weeks 23 to 26, focusing on their practical application: writing reports, identifying creep, conducting variance analysis, escalating issues and managing change.

[↑ Return to Table of Contents](#table-of-contents)

---

## 3. Status Reports: Purpose, Structure and Formats

**⏱ 12 minutes | LO5.1**

### 3.1 Purpose of the Status Report

A project status report is a formal, periodic communication that informs stakeholders of project progress relative to the approved baseline (Project Management Institute, 2021). Its primary functions are to:

- Provide an objective, time-stamped record of project health.
- Enable decision-makers to take corrective action before issues become crises.
- Create an audit trail that supports post-project review and lessons learned.
- Maintain stakeholder confidence through transparent communication.

The APM Body of Knowledge (Association for Project Management, 2019, p.104) states that "regular reporting creates the discipline of regular review," emphasising that the act of preparing a report is itself a monitoring control.

### 3.2 Key Components of a Status Report

A well-structured engineering project status report typically contains the following elements:

| Component | Description | Example |
|-----------|-------------|---------|
| **Report header** | Project name, report date, reporting period, author | "HS2 Euston Station — Week 52 Status Report" |
| **Executive summary** | RAG status and one-paragraph overview | Overall status: AMBER |
| **Schedule performance** | Planned vs actual progress; milestones due/achieved | 3 of 5 planned milestones achieved |
| **Cost performance** | Budget spend vs planned spend; forecast at completion | £4.2m spent vs £3.8m planned |
| **Quality performance** | Defect rates, inspection outcomes, non-conformances | 12 open NCRs; 3 critical |
| **Risks and issues** | Active risks, newly identified issues, mitigations | Risk R-14 escalated to project board |
| **Actions and decisions required** | Items requiring stakeholder input | Approve revised procurement schedule |
| **Forecast** | Projected completion date and cost | Forecast £0.4m over budget at completion |

### 3.3 RAG Status Indicators

The RAG (Red, Amber, Green) system provides an immediate visual summary of project health across the three control dimensions — time, cost and quality (Turner, 2014):

```
  GREEN  = On track; no significant variance from baseline
  AMBER  = At risk; variance detected; corrective action underway or planned
  RED    = Off track; significant variance; escalation required
```

> **Example:** On the Thames Tideway Tunnel project, Tideway used a monthly RAG dashboard distributed to the project board. When the Chambers Wharf shaft drilling encountered unexpected ground conditions, the schedule indicator moved to RED, triggering an immediate escalation meeting and a contract variation process (Tideway, 2022).

### 3.4 Reporting Frequency and Format

Reporting frequency should be proportional to project risk and complexity (Project Management Institute, 2021). Common formats include:

- **Weekly** status reports during high-risk implementation phases.
- **Monthly** reports for programme-level summaries to senior stakeholders.
- **Exception reports** triggered by a significant adverse event, regardless of the reporting cycle.

[↑ Return to Table of Contents](#table-of-contents)

---

## 4. Time, Cost and Quality Creep

**⏱ 10 minutes | LO5.1 / LO5.2**

### 4.1 Definitions

Creep refers to the gradual, often unnoticed, accumulation of deviations from the approved project baseline. Because each individual deviation appears small at the time, creep can persist undetected until it has produced a significant overall variance (Kerzner, 2017).

**Time creep** occurs when activities consistently take slightly longer than planned, causing the overall project schedule to extend incrementally. Each delay may be trivial in isolation, but compounded across many activities it can push a project significantly beyond its completion date.

**Cost creep** occurs when expenditure consistently exceeds the budgeted figures for individual work packages. Small overspends on materials, labour, or subcontractors accumulate into a substantial budget overrun.

**Quality erosion** (sometimes called quality creep) occurs when quality standards are progressively relaxed, often under schedule or cost pressure. Non-conformances are accepted, inspection steps are skipped or reduced, and the specification is quietly diluted.

### 4.2 Causes and Indicators

```
  CAUSE                        INDICATOR IN MONITORING DATA
  ─────────────────────────────────────────────────────────
  Optimistic initial estimates  Consistent small adverse variances
  Scope additions               Budget spend rising faster than progress
  Poor time management          Activities always finishing 1-2 days late
  Inadequate quality gates      Rising non-conformance report count
  Stakeholder-driven changes    Frequent minor scope amendments
```

### 4.3 Engineering Example: HS2 Phase One

The National Audit Office (2020) reported that HS2 Phase One costs rose from an estimated £37.5 billion (2019 prices) at sanction to over £44 billion, with schedule slipping by over three years. The review identified that many individual work packages were delivered slightly over budget and slightly late, with no effective mechanism to aggregate these trends and trigger early corrective action — a textbook instance of time and cost creep operating simultaneously.

### 4.4 Preventing Creep

Prevention relies on the same principle: frequent, granular monitoring against a robust baseline. Turner (2014, p.298) argues that "the discipline of regular comparison prevents the normalisation of deviation." Key controls include:

- Setting clearly defined tolerances (e.g., ±5% cost, ±2 days schedule) at work-package level.
- Reviewing trends across multiple reporting periods, not just the most recent.
- Requiring explicit approval for any variation, however small (change control — see Section 7).

[↑ Return to Table of Contents](#table-of-contents)

---

## 5. Variance Analysis in Practice

**⏱ 15 minutes | LO5.1**

### 5.1 What Is Variance Analysis?

Variance analysis is the systematic comparison of planned (baseline) values against actual values, in order to quantify the magnitude and direction of any deviation (Association for Project Management, 2019). It is one of the most directly assessed techniques in the OCR Unit 24 examination.

A variance is calculated as:

```
  Variance = Actual Value − Planned Value
```

The variance is then expressed as a percentage of the planned value:

```
  Percentage Variance (%) = ((Actual − Planned) / Planned) × 100
```

- A **favourable variance** occurs when the actual outcome is better than planned (e.g., cost lower than budget, or quality defects fewer than forecast).
- An **adverse variance** occurs when the actual outcome is worse than planned (e.g., cost higher than budget, schedule delayed).

> **Important:** In the examination, students are expected both to calculate the variance and to correctly label it as **adverse** or **favourable**. Omitting the label loses marks.

### 5.2 Worked Example: Variance Analysis Table

A civil engineering contractor is monitoring the installation of drainage systems across four sites on a road-widening project. The table below shows planned and actual completion percentages at the end of Week 8.

| Site | Planned Completion (%) | Actual Completion (%) | Variance (%) | Adverse / Favourable |
|------|----------------------|-----------------------|--------------|----------------------|
| A | 80 | 75 | −5 | **Adverse** |
| B | 60 | 65 | +5 | **Favourable** |
| C | 90 | 90 | 0 | **On target** |
| D | 70 | 58 | −12 | **Adverse** |

**Worked calculation for Site D:**

```
  Variance       = 58 − 70 = −12 percentage points
  % Variance     = (−12 / 70) × 100 = −17.1%
  Classification = Adverse (actual is below planned)
```

Site D requires immediate attention. An adverse variance of 17.1% at Week 8 means the site is significantly behind schedule. The project manager should investigate the cause, assess the impact on the overall project completion date, and determine whether corrective action is feasible within the remaining float.

### 5.3 Cost Variance Example

The same project has the following cost data at Week 8:

| Work Package | Budgeted Cost (£k) | Actual Cost (£k) | Variance (£k) | Adverse / Favourable |
|---|---|---|---|---|
| Drainage — Site A | 120 | 132 | +12 | **Adverse** |
| Drainage — Site B | 80 | 76 | −4 | **Favourable** |
| Drainage — Site D | 105 | 118 | +13 | **Adverse** |
| **Total** | **305** | **326** | **+21** | **Adverse** |

The overall cost variance of +£21k adverse, combined with the schedule delay at Site D, suggests a systemic problem requiring investigation and corrective action.

### 5.4 Reading Trends Across Reporting Periods

A single period's variance may be attributable to a one-off event. Sustained adverse variances across multiple reporting periods indicate a systemic problem. The project manager should plot the cumulative variance over time:

```
  Week:      1    2    3    4    5    6    7    8
  Variance: −1%  −2%  −3%  −3%  −6%  −9%  −11% −17%
             |                             |
             Small           Growing concern — escalation threshold crossed
```

This trend view is more informative than any single data point and is a key principle in earned value analysis (Kerzner, 2017).

[↑ Return to Table of Contents](#table-of-contents)

---

## 6. Escalation Procedures

**⏱ 8 minutes | LO5.1**

### 6.1 What Is Escalation?

Escalation is the formal process by which a project manager refers an issue, risk or decision upwards through the project governance structure when it exceeds their delegated authority or tolerance thresholds (Association for Project Management, 2019). It is a control mechanism, not an admission of failure — it ensures that the appropriate level of authority is engaged at the appropriate time.

The key principle is that **escalation should be timely**: waiting until a problem has become critical before escalating eliminates the decision space available to senior stakeholders (Turner, 2014).

### 6.2 Escalation Thresholds

Escalation is typically triggered when:

- A variance exceeds the agreed tolerance (e.g., cost overrun >10% of work-package budget).
- A critical-path activity is delayed beyond a defined number of days.
- A risk moves from an acceptable to an unacceptable level on the risk matrix.
- A decision is required that is outside the project manager's delegated financial authority.
- An issue cannot be resolved within the project team's resources or timescales.

### 6.3 A Structured Escalation Pathway

```
  LEVEL 1 — Project Team
      Issue identified and logged in the issue register
      Team-level resolution attempted within [defined period, e.g. 3 days]
           |
           | Not resolved / exceeds team authority
           v
  LEVEL 2 — Project Manager
      Formal issue report raised; corrective action assessed
      PM resolution within delegated authority and tolerance
           |
           | Exceeds PM authority or tolerance threshold
           v
  LEVEL 3 — Project Board / Steering Committee
      Exception report submitted; board meeting convened
      Board authorises corrective action / change request
           |
           | Strategic decision required / programme-level impact
           v
  LEVEL 4 — Project Sponsor / Executive
      Strategic direction sought; resource allocation authorised
```

### 6.4 The Exception Report

An exception report is a specific document prepared when a project is forecast to exceed its agreed tolerances. It is distinct from a standard status report in that it focuses exclusively on the deviation, its cause, its likely impact, and the options available for recovery (Association for Project Management, 2019). A typical exception report contains:

- A clear statement of the deviation and its cause.
- Impact on time, cost and quality baselines.
- Options available, with pros and cons for each.
- A recommended course of action.
- Decisions required from the project board.

> **Example:** During construction of the Elizabeth Line, a delayed delivery of specialist tunnel segments at Whitechapel triggered an exception report to the Crossrail project board. The board authorised a contract variation and a revised programme baseline, demonstrating the escalation pathway functioning correctly (Wolstenholme, 2011).

[↑ Return to Table of Contents](#table-of-contents)

---

## 7. Change Control

**⏱ 6 minutes | LO5.1**

### 7.1 Why Change Control Is Essential

Change is inevitable in engineering projects. Stakeholder requirements evolve, technical solutions prove impractical, and external conditions alter. Without a structured process for managing change, each modification — however well-intentioned — can unpredictably alter the cost, schedule and quality baseline, making it impossible to maintain effective control (Kerzner, 2017).

Change control is the process by which all proposed modifications to the approved project baseline are formally evaluated, approved or rejected, and implemented in a controlled manner (Project Management Institute, 2021). It protects the integrity of the baseline and ensures that the impact of every change is understood before it is implemented.

### 7.2 The Change Control Process

```
  1. CHANGE REQUEST RAISED
     Formal change request form submitted by any stakeholder
     Describes: what, why, urgency, originator
          |
          v
  2. IMPACT ASSESSMENT
     Project manager assesses impact on time, cost, quality, risk and scope
     Assessment documented and costed
          |
          v
  3. REVIEW AND DECISION
     Change control board (CCB) or project board reviews assessment
     Decision: Approve / Reject / Defer / Approve with conditions
          |
          v
  4. IMPLEMENTATION (if approved)
     Project plan, schedule and budget updated
     Team notified; issue log updated
          |
          v
  5. CLOSE-OUT
     Change request closed and archived
     Baseline formally updated; new baseline communicated
```

### 7.3 The Change Log

All change requests — whether approved, rejected or deferred — must be recorded in a change log. This provides an auditable history of every modification to the project baseline, which is essential for post-project review and dispute resolution.

| Change Ref | Description | Raised By | Date | Impact Assessment | Decision | Status |
|---|---|---|---|---|---|---|
| CR-001 | Additional drainage inspection pit — Site D | Client engineer | 14 Apr | +£8k, +3 days | Approved | Implemented |
| CR-002 | Substitute pipe specification | Procurement | 18 Apr | Negligible cost; quality risk HIGH | Rejected | Closed |
| CR-003 | Extend programme by 2 weeks | PM | 21 Apr | +£15k; schedule +14 days | Pending Board | Open |

### 7.4 Scope Creep vs Managed Change

The distinction between **scope creep** and **managed change** is important. Scope creep occurs when changes are implemented informally, without going through the change control process, typically because they appear trivial at the time. Over time, these informal changes accumulate and undermine the baseline. Managed change, by contrast, is any modification — regardless of size — that has been formally assessed and approved. All changes, however small, must pass through the change control process.

[↑ Return to Table of Contents](#table-of-contents)

---

## 8. Conclusion and Summary

**⏱ 2 minutes | LO5**

This session has consolidated the core monitoring and control competencies required of an engineering project manager. The key points are:

- **Status reports** provide a structured, periodic record of project health across time, cost and quality dimensions. The RAG system offers an immediate visual summary for stakeholders.
- **Time, cost and quality creep** are gradual deviations that, if undetected, can compound into significant overruns. Regular monitoring against the baseline, with clearly defined tolerances, is the primary defence.
- **Variance analysis** quantifies the magnitude and direction of deviation from the plan. Each variance must be calculated, expressed as a percentage, and classified as adverse or favourable.
- **Escalation procedures** ensure that issues reaching or exceeding tolerance thresholds are referred promptly to the appropriate level of authority, preserving decision space for senior stakeholders.
- **Change control** protects the integrity of the project baseline by ensuring that every modification — regardless of apparent size — is formally assessed, decided upon, and documented before implementation.

Together, these practices embody the monitoring and control discipline that characterises professional engineering project management. As the APM Body of Knowledge (Association for Project Management, 2019, p.102) observes, "effective control is not about preventing change — it is about managing it."

[↑ Return to Table of Contents](#table-of-contents)

---

## References

Association for Project Management (2019) *APM Body of Knowledge*. 7th edn. Princes Risborough: Association for Project Management.

Hardie, R. (2011) *Edinburgh Trams Inquiry: Preliminary Report*. Edinburgh: Scottish Government.

Kerzner, H. (2017) *Project Management: A Systems Approach to Planning, Scheduling and Controlling*. 12th edn. Hoboken, NJ: John Wiley & Sons.

National Audit Office (2020) *HS2 Phase One: A Review of Early Progress*. London: NAO. Available at: https://www.nao.org.uk/reports/hs2-phase-one (Accessed: 15 April 2026).

OCR (2017) *Cambridge Technicals Level 3 Engineering: Unit 24 Project Management for Engineers (T/615/1558)*. Cambridge: OCR.

Project Management Institute (2021) *A Guide to the Project Management Body of Knowledge (PMBOK® Guide)*. 7th edn. Newtown Square, PA: Project Management Institute.

Tideway (2022) *Tideway Annual Report and Accounts 2021/22*. London: Bazalgette Tunnel Limited.

Turner, J.R. (2014) *The Handbook of Project-Based Management*. 4th edn. New York: McGraw-Hill.

Wolstenholme, A. (2011) *Never Waste a Good Crisis: A Review of Progress Since Rethinking Construction and Thoughts for Our Future*. London: Constructing Excellence.

---

*Word count: approximately 2,850 words (excluding references, bibliography, tables and diagrams)*
