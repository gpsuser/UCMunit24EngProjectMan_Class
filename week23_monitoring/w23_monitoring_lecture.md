# Unit 24: Project Management for Engineers
## Week 23 Lecture: Monitoring Methods

**Cambridge TECHNICALS Level 3 Engineering**
**Delivery Duration:** 60 minutes
**Phase 5: Project Monitoring**

---

## Table of Contents

| # | Section | Time Allocation | Learning Outcome |
|---|---------|----------------|-----------------|
| 1 | [Objectives](#1-objectives) | 2 min | — |
| 2 | [Introduction: Why Monitoring Matters](#2-introduction-why-monitoring-matters) | 5 min | LO5.1 |
| 3 | [Using Project Management Tools to Monitor Progress](#3-using-project-management-tools-to-monitor-progress) | 12 min | LO5.1 |
| 4 | [Comparing Actual Performance with Planned Performance](#4-comparing-actual-performance-with-planned-performance) | 12 min | LO5.1 |
| 5 | [Earned Value Analysis](#5-earned-value-analysis) | 12 min | LO5.1 |
| 6 | [Quality Management During Project Execution](#6-quality-management-during-project-execution) | 10 min | LO5.1 |
| 7 | [Control Techniques and Frequent Reporting](#7-control-techniques-and-frequent-reporting) | 5 min | LO5.1 |
| 8 | [Conclusion and Key Takeaways](#8-conclusion-and-key-takeaways) | 2 min | LO5.1 |
| — | [References](#references) | — | — |

---

## 1. Objectives

*[2 minutes | LO5.1]*

By the end of this lecture, learners will be able to:

- Explain how project management tools are used to monitor an engineering project in progress.
- Describe what is meant by comparing actual with planned performance, including the concepts of time creep, quality erosion, and budget overrun.
- Apply the principles of Earned Value Analysis (EVA) to assess project status.
- Explain what quality management involves during the implementation stage of a project.
- Identify a range of control techniques and explain how frequent reporting supports project monitoring.

**Assessment Criterion:** LO5.1 — *How projects are monitored* (OCR, 2017)

---

[↑ Back to Contents](#table-of-contents)

---

## 2. Introduction: Why Monitoring Matters

*[5 minutes | LO5.1]*

Even the most carefully planned engineering project rarely runs exactly as expected. Once implementation begins, a project enters a dynamic environment in which schedules slip, costs increase, and quality can be compromised. Without systematic monitoring, a project manager may only discover serious problems when it is too late to take effective corrective action.

Project monitoring is the process of regularly collecting, analysing, and reporting data about a project's performance to determine whether it is progressing according to plan (PMI, 2021). The fundamental question asked at every monitoring checkpoint is: *"Are we on track, and if not, what must be done?"*

**The Monitoring Cycle**

```
  PLAN                  MONITOR                  COMPARE
+---------+          +-----------+          +------------------+
| Set     |  ------> | Collect   |  ------> | Actual vs        |
| Targets |          | Data      |          | Planned          |
+---------+          +-----------+          +------------------+
                                                    |
                                                    v
  IMPLEMENT                                  TAKE CORRECTIVE
  CHANGES          <--------------------------  ACTION
+-----------+                               +----------------+
| Update    |                               | Identify       |
| Plan      |                               | Variance       |
+-----------+                               +----------------+
```

According to the OCR Unit 24 specification, monitoring encompasses five key activities: using project management tools, comparing actual with planned performance, managing quality, applying control techniques, and maintaining frequent reporting (OCR, 2017). Each of these is examined in the sections that follow.

> **UK Engineering Context:** The Crossrail (Elizabeth line) project — completed in 2022, nine years after its scheduled opening date — provides a compelling illustration of what happens when monitoring and control systems are inadequate in the early stages of a major infrastructure programme (National Audit Office, 2019).

---

[↑ Back to Contents](#table-of-contents)

---

## 3. Using Project Management Tools to Monitor Progress

*[12 minutes | LO5.1 — Use of project management tools]*

The project management tools covered in earlier phases of this course — Gantt charts, Critical Path Analysis (CPA), and PERT — are not only planning instruments. During implementation, they become essential monitoring tools. In addition to these, two further techniques — the S-curve and the burndown chart — are commonly used on engineering projects.

### 3.1 Gantt Charts as Monitoring Tools

A Gantt chart constructed at the planning stage sets out the scheduled start and finish dates for every activity. During implementation, the chart is updated by shading actual progress against the planned bars. Any activity that has not progressed as expected becomes immediately visible.

**Example — Gantt Chart Progress Tracking:**

```
Activity        Week:  1    2    3    4    5    6    7    8
                       |    |    |    |    |    |    |    |
A: Site prep    Plan  [====]
                Actua [====]                          (on time)

B: Foundations  Plan       [=========]
                Actua       [=========>               (1 week delay)

C: Steelwork    Plan                  [========]
                Actua                  NOT STARTED    (blocked by B)
```

In this example, the delay on Activity B has a knock-on effect on Activity C. This is precisely the type of variance that monitoring should detect and trigger corrective action to address.

### 3.2 Critical Path Analysis (CPA) in Monitoring

During implementation, CPA is used to assess the impact of any delays on the overall project completion date. Because critical path activities have zero float time, any slippage on these activities directly extends the project duration (Turner, 2014). A project manager should prioritise monitoring of critical path activities above all others.

### 3.3 S-Curves

An S-curve plots cumulative planned expenditure (or work completed) against time, producing a characteristic S-shape. During monitoring, actual cumulative spend is plotted on the same graph. Any divergence from the planned curve indicates a variance.

```
Cumulative
  Cost
   |                                 /
   |                            ___/     <-- Planned
   |                       ____/
   |                  ____/
   |             ____/
   |        ____/
   |  _____/
   |_/
   +----------------------------------------> Time
        (Start)                    (End)

   If actual line falls ABOVE the planned curve = over-budget
   If actual line falls BELOW the planned curve = under-spend
     (which may indicate that work is also behind schedule)
```

### 3.4 Burndown Charts

Burndown charts are widely used in iterative and agile engineering projects. They plot the amount of work remaining (on the vertical axis) against time (on the horizontal axis). On a project running to plan, the actual line should closely follow the ideal burndown gradient. If the actual line is above the ideal line, work is accumulating faster than it is being completed.

```
Work
Remaining
(units)
  100 |*
   90 | *  *
   80 |    . *                  * = Actual work remaining
   70 |  .       *              . = Ideal (planned) burndown
   60 |.             *
   50 |                  *
   40 |                      *
   30 |                          *
   20 |                              *
   10 |                                  *
    0 +---+---+---+---+---+---+---+---+--> Weeks
      0   1   2   3   4   5   6   7   8
```

When the actual line trends above the ideal, the project manager must investigate the cause — are tasks being underestimated, is resource unavailable, or is scope increasing without approval?

---

[↑ Back to Contents](#table-of-contents)

---

## 4. Comparing Actual Performance with Planned Performance

*[12 minutes | LO5.1 — Comparison of actual with planned]*

Monitoring requires a systematic comparison of what is actually happening on a project against what was planned to happen. Three critical deviations are identified in the OCR specification: time creep, quality erosion, and budget overrun.

### 4.1 Time Creep

Time creep (also referred to as schedule slippage) occurs when project activities take longer than planned. This can result from many causes: supplier delays, unforeseen technical complexity, resource unavailability, or poor workmanship requiring rework. Each delay has a cost implication as well as a direct impact on the schedule (APM, 2019).

**Indicators of time creep:**
- Activities consistently finishing later than planned on the Gantt chart.
- Milestone dates being missed.
- The number of incomplete tasks increasing week-on-week.

**UK Engineering Example:** During the construction of the Thames Tideway Tunnel (known as the Super Sewer), project managers monitored tunnelling progress at weekly intervals against an agreed schedule. Regular milestone reviews enabled corrective action — such as increasing shift hours — when the actual rate of tunnelling fell behind the planned rate (Bazalgette Tunnel Ltd, 2022).

### 4.2 Quality Erosion

Quality erosion occurs when the quality of deliverables falls below the standard set in the quality plan. On an engineering project, this might manifest as components that fail inspection, welds that do not meet specification, or software that does not pass acceptance testing. Left unchecked, quality erosion increases rework costs, delays delivery, and can result in safety hazards.

**Indicators of quality erosion:**
- Increasing defect or non-conformance reports.
- Inspection failure rates rising above baseline thresholds.
- Customer or end-user complaints.
- Rework consuming an increasing proportion of resource time.

### 4.3 Budget Overrun

Budget overrun (or cost creep) occurs when actual expenditure exceeds the planned budget. This is one of the most common failure modes on engineering projects and typically results from a combination of scope changes, time creep, and underestimation of costs during planning (Turner, 2014).

**The Variance Formula:**

The basic cost variance used in monitoring is:

```
Cost Variance (CV) = Budgeted Cost of Work Performed - Actual Cost of Work Performed

                     CV = BCWP - ACWP

  Positive CV  (+)  -->  Under-budget (favourable)
  Negative CV  (-)  -->  Over-budget  (unfavourable)
```

### 4.4 Summary: The Three Creeps

| Deviation | What It Means | Key Indicator | Impact |
|-----------|--------------|---------------|--------|
| Time creep | Activities taking longer than planned | Milestone slippage | Cost increase; late delivery |
| Quality erosion | Deliverables below standard | Defect / rework rate | Safety risk; rework cost |
| Budget overrun | Spend exceeding plan | Negative cost variance | Financial exposure |

It is important to recognise that these three deviations are interdependent: time creep drives cost increases; quality erosion triggers rework, which causes further time creep and additional cost.

---

[↑ Back to Contents](#table-of-contents)

---

## 5. Earned Value Analysis

*[12 minutes | LO5.1 — Earned Value Analysis]*

Earned Value Analysis (EVA) is a structured monitoring technique that integrates scope, schedule, and cost data into a single performance measurement framework. It provides an objective answer to the question: *"How much value has actually been delivered for the money spent so far?"* (PMI, 2021).

EVA is particularly valuable because it prevents a common misreading of project status. A project may be spending exactly to budget, yet still be behind schedule — in which case the actual spend is providing less value than expected.

### 5.1 The Three Core EVA Values

Three baseline values underpin every EVA calculation:

| Value | Abbreviation | Definition |
|-------|-------------|-----------|
| Planned Value | PV | The budgeted cost of work *scheduled* to be done by a given date |
| Earned Value | EV | The budgeted cost of work *actually completed* by a given date |
| Actual Cost | AC | The *actual* cost incurred for work completed by a given date |

### 5.2 Calculating EVA Variances and Indices

From these three values, the following performance metrics are derived:

**Variances:**

```
Schedule Variance (SV) = EV - PV
  Positive SV  -->  Ahead of schedule
  Negative SV  -->  Behind schedule

Cost Variance (CV) = EV - AC
  Positive CV  -->  Under budget
  Negative CV  -->  Over budget
```

**Performance Indices:**

```
Schedule Performance Index (SPI) = EV / PV
  SPI > 1.0  -->  More work completed than planned (efficient)
  SPI < 1.0  -->  Less work completed than planned (inefficient)

Cost Performance Index (CPI) = EV / AC
  CPI > 1.0  -->  Delivering more value per pound spent (cost-efficient)
  CPI < 1.0  -->  Delivering less value per pound spent (over-spending)
```

### 5.3 Worked Example — HS2 Subcontract Package

The following example is illustrative and based on an engineering project context similar to the HS2 civil engineering programme.

A groundworks subcontract has a total budget of £2,000,000. At the end of Month 3, the monitoring data is as follows:

| Metric | Value |
|--------|-------|
| Planned Value (PV) | £600,000 |
| Earned Value (EV) | £480,000 |
| Actual Cost (AC) | £540,000 |

**Calculations:**

```
Schedule Variance (SV) = EV - PV = £480,000 - £600,000 = -£120,000
--> Behind schedule by £120,000 worth of work

Cost Variance (CV) = EV - AC = £480,000 - £540,000 = -£60,000
--> Over-spending by £60,000

SPI = EV / PV = 480,000 / 600,000 = 0.80
--> Only 80% of the planned work has been completed

CPI = EV / AC = 480,000 / 540,000 = 0.89
--> Delivering only 89p of value for every £1 spent
```

**Interpretation:** The project is both behind schedule and over-budget. Both indices are below 1.0, indicating that corrective action is urgently required. The project manager would need to investigate the root causes — possible explanations include poor productivity, additional material costs, or scope additions not recorded through change control.

### 5.4 EVA: Key Points for the Examination

> - EVA requires three data points: PV, EV, and AC.
> - Variances below zero are always unfavourable.
> - Indices below 1.0 are always unfavourable.
> - SPI measures schedule efficiency; CPI measures cost efficiency.

---

[↑ Back to Contents](#table-of-contents)

---

## 6. Quality Management During Project Execution

*[10 minutes | LO5.1 — Quality management]*

Quality management during the implementation stage of a project involves the systematic activities undertaken to ensure that the project's deliverables meet the quality standards set out in the quality plan (BSI, 2015). It is not simply about inspecting finished products; it encompasses the full set of processes that prevent defects from arising in the first place.

### 6.1 Quality Assurance vs Quality Control

A clear distinction is drawn between quality assurance (QA) and quality control (QC):

```
QUALITY MANAGEMENT
        |
        +----> QUALITY ASSURANCE (QA)
        |         Process-focused
        |         Aims to PREVENT defects
        |         Examples: staff training, standardised work
        |                   procedures, audits, peer review
        |
        +----> QUALITY CONTROL (QC)
                  Product-focused
                  Aims to DETECT defects
                  Examples: inspection, testing, sampling,
                            statistical process control
```

QA is proactive — it builds quality into the process. QC is reactive — it identifies defects after the work has been done. Best practice requires both (BSI, 2015).

### 6.2 Statistical Quality Control: Using Control Limits

One of the most widely examined methods of quality monitoring in the OCR examination is the use of **control limits** — upper and lower boundaries within which a measured quality characteristic must remain if the process is deemed to be "in control".

The approach involves:

1. **Defining the quality characteristic** to be monitored (e.g., the mass of a component, the tensile strength of a weld, the diameter of a machined bore).
2. **Setting control limits** based on specification tolerances or process capability data.
3. **Sampling** the output at regular intervals and measuring the characteristic.
4. **Calculating the sample mean** (or other statistic) and plotting it against the control limits.
5. **Making a pass/fail decision**: if the sample mean falls outside the control limits, the process is out of control and production must halt until the cause is investigated.

**Example — Quality Control on a Rolls-Royce Component:**

A machining process produces turbine blade spacers with a specified mass of 85.0 g ± 2.0 g. The control limits are therefore:

```
Upper Control Limit (UCL) = 87.0 g
Lower Control Limit (LCL) = 83.0 g
```

A batch of 50 spacers is sampled. The frequency data for mass measurements is:

| Mass (g) | Frequency (f) | Mass x Frequency (m x f) |
|----------|--------------|--------------------------|
| 83.0     | 3            | 249.0                    |
| 84.0     | 8            | 672.0                    |
| 85.0     | 22           | 1870.0                   |
| 86.0     | 14           | 1204.0                   |
| 87.0     | 3            | 261.0                    |
| **Total**| **50**       | **4256.0**               |

**Calculating the weighted mean:**

```
          Sum of (mass x frequency)        4256.0
Mean  =  -------------------------  =  ----------  =  85.12 g
              Sum of frequencies              50
```

**Decision:**

```
LCL = 83.0 g  <  Mean = 85.12 g  <  UCL = 87.0 g

Result: PASS -- the process is in control.
```

> **Examination Note:** In past OCR papers, learners have been asked to: (i) identify the quality characteristic being tested, (ii) calculate the weighted mean using frequency data, (iii) compare the result to control limits, and (iv) state the pass/fail decision. All four steps should be practised (OCR, 2024).

### 6.3 Quality Metrics

A quality metric is a specific, measurable indicator used to track quality performance over time. Examples used on UK engineering projects include:

| Metric | Description | Example |
|--------|------------|---------|
| Defect rate | Number of defective items per batch | 2 rejects per 100 components |
| First-time pass rate | Percentage passing inspection first time | 97.5% first-time pass |
| Rework hours | Hours spent correcting defects | 12 hours per week |
| Customer complaints | Formal complaints received per period | 0 complaints in Month 4 |
| Inspection failure rate | Percentage of inspections that fail | 1.8% failure rate |

Tracking quality metrics over time allows trends to be identified before a quality problem becomes critical.

---

[↑ Back to Contents](#table-of-contents)

---

## 7. Control Techniques and Frequent Reporting

*[5 minutes | LO5.1 — Control techniques; Frequent reporting]*

### 7.1 Control Techniques

A control technique is any structured method used to keep a project on track. The OCR specification lists control techniques as a key element of LO5.1. The following are the most commonly assessed:

| Control Technique | Description |
|-------------------|-------------|
| **Milestone slip chart** | Tracks whether key project milestones are being reached on time; each milestone is plotted against its planned and actual achievement date |
| **Regular review meetings** | Scheduled meetings (weekly, fortnightly) where the project team reviews progress against plan and agrees corrective action |
| **Issue log (RAID log)** | A living document recording Risks, Assumptions, Issues, and Dependencies; updated continuously during implementation |
| **Change control process** | A formal procedure for evaluating, approving, and recording any changes to project scope, schedule, or budget |
| **Kanban board** | A visual board showing tasks in columns (e.g., To Do / In Progress / Done), enabling immediate visibility of workflow bottlenecks |
| **Requirements traceability matrix** | Maps each project deliverable back to a specific requirement, ensuring nothing is omitted and scope creep is detected |

**Milestone Slip Chart Example:**

```
Milestone       Plan        Actual      Status
-----------     ---------   ---------   -------
M1 Design       Week 4      Week 4      ON TIME
M2 Prototype    Week 8      Week 9      1 WEEK LATE
M3 Test         Week 12     Week 14     2 WEEKS LATE (projected)
M4 Delivery     Week 16     Week 19?    AT RISK
```

The milestone slip chart makes visible the cumulative effect of repeated small delays — a pattern that is difficult to detect from raw progress data alone.

### 7.2 Frequent Reporting

The OCR specification explicitly identifies frequent reporting as a component of LO5.1 (OCR, 2017). Regular written reports — typically weekly or fortnightly on engineering projects — serve several essential functions:

- They provide a formal record of project status at a point in time.
- They communicate variances to the project board and sponsor, enabling timely decisions.
- They create an audit trail that is invaluable if disputes arise.
- They prompt the project team to review their own performance systematically.

A typical project status report contains: a summary of progress against plan, key metrics (cost, schedule, quality), a summary of risks and issues, decisions required, and actions for the next reporting period.

> **Key Principle:** The purpose of monitoring and control is not to generate paperwork — it is to enable timely, informed decisions. The sooner a deviation from plan is detected and acted upon, the lower the cost of correction (APM, 2019).

---

[↑ Back to Contents](#table-of-contents)

---

## 8. Conclusion and Key Takeaways

*[2 minutes | LO5.1]*

This lecture has introduced the five key components of LO5.1 — how projects are monitored. The following summary captures the essential points:

**1. Project management tools** — Gantt charts, CPA, S-curves, and burndown charts are all used during implementation to track progress visually.

**2. Actual vs planned comparison** — Three deviations must be monitored: time creep, quality erosion, and budget overrun. All three are interdependent.

**3. Earned Value Analysis** — EVA integrates scope, schedule, and cost into a unified performance framework. The key metrics are Schedule Variance (SV), Cost Variance (CV), the Schedule Performance Index (SPI), and the Cost Performance Index (CPI). Values below zero or below 1.0 indicate unfavourable performance.

**4. Quality management** — Quality assurance (process-focused, preventive) and quality control (product-focused, detective) work together. Statistical control limits provide an objective, exam-assessed method for making pass/fail decisions on quality data.

**5. Control techniques and reporting** — Milestone slip charts, issue logs, change control, Kanban boards, and regular written reports collectively ensure that deviations are detected early and corrective action is taken promptly.

```
MONITORING FRAMEWORK SUMMARY
+-----------------------------------------------------------+
|  MONITOR USING:                                           |
|    --> Gantt / CPA / S-curve / Burndown chart             |
|                                                           |
|  COMPARE:                                                 |
|    --> Actual vs Planned (time, cost, quality)            |
|    --> EVA: SV = EV - PV | CV = EV - AC                  |
|    --> SPI = EV/PV       | CPI = EV/AC                   |
|                                                           |
|  CONTROL QUALITY:                                         |
|    --> QA (prevent) + QC (detect)                         |
|    --> Control limits: sample mean vs UCL/LCL             |
|                                                           |
|  APPLY CONTROL TECHNIQUES:                                |
|    --> Milestone slip charts, RAID logs, change control   |
|    --> Frequent written reports to project board          |
+-----------------------------------------------------------+
```

---

[↑ Back to Contents](#table-of-contents)

---

## References

APM (2019) *APM Body of Knowledge*. 7th edn. Princes Risborough: Association for Project Management.

Bazalgette Tunnel Ltd (2022) *Thames Tideway Tunnel: Construction update, monitoring and progress reports*. London: Bazalgette Tunnel Ltd. Available at: https://www.tideway.london (Accessed: 11 March 2026).

BSI (2015) *BS EN ISO 9001:2015: Quality management systems — Requirements*. London: British Standards Institution.

National Audit Office (2019) *Completing Crossrail*. London: National Audit Office. HC 2285, Session 2017–19.

OCR (2017) *Cambridge TECHNICALS Level 3 Engineering: Unit 24, Project Management for Engineers — Unit Specification* (Version 1). Oxford: Oxford Cambridge and RSA Examinations.

OCR (2024) *Unit 24 Project Management for Engineers: June 2024 Mark Scheme*. Oxford: Oxford Cambridge and RSA Examinations.

PMI (2021) *A Guide to the Project Management Body of Knowledge (PMBOK® Guide)*. 7th edn. Newtown Square, PA: Project Management Institute.

Turner, J.R. (2014) *The Handbook of Project-Based Management*. 4th edn. New York: McGraw-Hill.

---

*Word count (excluding references and bibliography): approximately 2,850 words*

---

**Document Information**
- **Unit:** Cambridge TECHNICALS Level 3 Engineering — Unit 24: Project Management for Engineers
- **Week:** 23
- **Topic:** Monitoring Methods
- **Learning Outcome:** LO5.1 — How projects are monitored
- **Delivery Duration:** 60 minutes
- **Prepared for:** Engineering undergraduate learners, UK
