# Week 12: Gantt Chart Practice

**Unit 24: Project Management for Engineers**  
**Cambridge TECHNICALS Level 3 Engineering**  
**Lecture Duration:** 55 minutes  
**Workshop Duration:** 30 minutes (following 5-minute break)  
**Learning Outcome:** LO3.1 – How to use and interpret a Gantt chart

---

## Table of Contents

| Section/Topic | Time Allocation | Learning Outcome | Page |
|--------------|----------------|------------------|------|
| Introduction & Objectives | 5 minutes | LO3.1 | 2 |
| Slack Time Analysis | 15 minutes | LO3.1 | 3 |
| Critical Activities Identification | 15 minutes | LO3.1 | 5 |
| Delays and Adjustments | 10 minutes | LO3.1 | 7 |
| Resource Levelling & Schedule Compression | 5 minutes | LO3.1 | 9 |
| Software Tools for Gantt Charts | 3 minutes | LO3.1 | 10 |
| Conclusion & Summary | 2 minutes | LO3.1 | 11 |

---

## Learning Objectives

By the end of this session, learners will be able to:

1. **Calculate and interpret slack time** (float time) for non-critical activities on a Gantt chart
2. **Identify critical activities** and explain their significance for project delivery
3. **Analyse the impact of delays** on project completion time and recommend appropriate adjustments
4. **Apply resource levelling techniques** to resolve scheduling conflicts
5. **Evaluate schedule compression strategies** including fast-tracking and crashing
6. **Use software tools** to create and modify Gantt charts efficiently

---

## Introduction (5 minutes) | LO3.1

### Context and Importance

Following on from Week 11's introduction to Gantt chart fundamentals, this week focuses on **practical application** of Gantt charts in real engineering project scenarios. Gantt charts are the most widely used project scheduling tool in the engineering industry, with research showing that approximately 80% of project managers use them regularly (Project Management Institute, 2021). However, creating a basic chart is only the first step; effective project management requires the ability to **analyse, interpret, and adjust** Gantt charts throughout the project lifecycle.

This session addresses three critical competencies that distinguish competent project managers from novices:

1. **Understanding slack time** – knowing which activities have flexibility in their scheduling
2. **Identifying critical activities** – recognising which tasks directly impact project completion
3. **Managing changes** – adjusting schedules when delays occur or opportunities for acceleration arise

These skills are directly assessed in external examinations and are essential for professional practice in engineering project management.

### Real-World Application

Consider the construction of the Elizabeth Line (Crossrail) in London, one of Europe's largest infrastructure projects. The project involved over 10,000 activities coordinated across 40 construction sites. Project managers used sophisticated Gantt charts to identify that the fitting-out of stations was on the critical path, whilst utilities diversions had significant slack time. This understanding enabled them to prioritise resources effectively and manage the inevitable delays that occurred (National Audit Office, 2018).

---

## Slack Time Analysis (15 minutes) | LO3.1

### Definition and Significance

**Slack time** (also called **float time** or **total float**) is the amount of time an activity can be delayed without affecting the project completion date. It represents scheduling flexibility and is calculated as:

```
Slack Time = Latest Finish Time - Earliest Finish Time
            OR
Slack Time = Latest Start Time - Earliest Start Time
```

### Types of Slack

1. **Total Float** – delay possible without affecting project completion
2. **Free Float** – delay possible without affecting the next activity's start time

For practical project management purposes, total float is most commonly used and simply referred to as "slack time".

### Calculating Slack Time from Gantt Charts

Gantt charts provide visual representation of slack time through the gap between an activity bar and the next dependent activity. Consider this example:

```
Activity Table:
┌──────────────┬──────────────────┬──────────┬─────────────────┐
│ Activity     │ Duration (weeks) │ Depends  │ Earliest Start  │
│              │                  │ on       │ (ES)            │
├──────────────┼──────────────────┼──────────┼─────────────────┤
│ A: Design    │ 4                │ -        │ Week 0          │
│ B: Procure   │ 3                │ A        │ Week 4          │
│ C: Test      │ 2                │ A        │ Week 4          │
│ D: Assemble  │ 5                │ B, C     │ Week 7          │
└──────────────┴──────────────────┴──────────┴─────────────────┘

Gantt Chart:
Week:    0    2    4    6    8    10   12
         |    |    |    |    |    |    |
A        [====]
B             [===]
C             [==][■■]  (2 weeks slack shown as ■■)
D                  [=====]
```

**Analysis:**
- Activity A: No slack (on critical path)
- Activity B: No slack (on critical path)
- Activity C: 2 weeks slack (can finish by Week 6 but D doesn't need it until Week 7)
- Activity D: No slack (on critical path)

### Practical Implications of Slack Time

Understanding slack time enables project managers to:

1. **Prioritise resources** – allocate key personnel to critical activities first
2. **Manage multiple projects** – assign staff with slack time activities to other projects temporarily
3. **Accept delays strategically** – permit delays on non-critical activities when necessary
4. **Negotiate schedules** – offer realistic delivery dates for component parts

### Case Study: Heathrow Terminal 5

During the construction of Heathrow Terminal 5, the project management team identified that certain airside works had 12 weeks of slack time, whilst the structural steelwork had zero slack. This enabled them to redeploy specialist steel erectors from the delayed airside works to accelerate the critical steelwork, keeping the project on schedule (BAA, 2008).

### Common Student Errors

❌ **Incorrect:** "Slack time means the activity is unimportant"  
✅ **Correct:** Slack time indicates scheduling flexibility, not importance

❌ **Incorrect:** "Activities with slack can be delayed indefinitely"  
✅ **Correct:** Slack time is finite; excessive delays consume slack and can make activities critical

### Practice Example

Calculate the slack time for each activity:

```
┌──────────┬──────────┬─────────┬────────────┬──────────────┐
│ Activity │ Duration │ Depends │ Earliest   │ Latest       │
│          │ (days)   │ on      │ Finish (EF)│ Finish (LF)  │
├──────────┼──────────┼─────────┼────────────┼──────────────┤
│ X        │ 5        │ -       │ Day 5      │ Day 5        │
│ Y        │ 3        │ X       │ Day 8      │ Day 10       │
│ Z        │ 4        │ X       │ Day 9      │ Day 9        │
└──────────┴──────────┴─────────┴────────────┴──────────────┘
```

**Solution:**
- Activity X: Slack = 5 - 5 = **0 days** (critical)
- Activity Y: Slack = 10 - 8 = **2 days**
- Activity Z: Slack = 9 - 9 = **0 days** (critical)

---

## Critical Activities Identification (15 minutes) | LO3.1

### Definition of Critical Activities

A **critical activity** is any task that, if delayed, will cause the entire project to be delayed. Critical activities form the **critical path** – the longest sequence of dependent activities through the project network.

### Characteristics of Critical Activities

1. **Zero slack time** – no scheduling flexibility
2. **Direct impact** – delays immediately affect project completion
3. **Highest priority** – require closest monitoring and fastest issue resolution
4. **Resource priority** – should receive best resources and management attention

### Identifying Critical Activities on Gantt Charts

On a Gantt chart, critical activities can be identified by:

1. **No gaps** before the next dependent activity
2. **Continuous chain** from project start to finish
3. **Longest path** through the network when dependencies are considered

### Visual Example

```
Week:    0    2    4    6    8    10   12   14
         |    |    |    |    |    |    |    |
A        [====]                               CRITICAL
B             [=======]                       CRITICAL
C                  [===]■■                    (slack shown)
D                     [======]                CRITICAL
E                             [====]          CRITICAL
F                                  [===]■     (slack shown)

Critical Path: A → B → D → E (Total: 14 weeks)
```

### Multiple Critical Paths

In complex projects, multiple critical paths may exist. This situation requires particular vigilance because a delay in **any** of the critical paths will delay the project. For example:

```
Week:    0    2    4    6    8    10
         |    |    |    |    |    |
Path 1:
A        [====]                    CRITICAL
B             [======]             CRITICAL

Path 2:
C        [=======]                 CRITICAL
D                [====]            CRITICAL
```

Both Path 1 (A→B) and Path 2 (C→D) take 10 weeks. A delay in activities A, B, C, or D will delay the project.

### Management Implications

Research by Turner and Müller (2003) demonstrates that projects with clearly identified critical paths are 40% more likely to complete on time than those without such analysis. Critical activity identification enables:

1. **Risk Management** – develop contingency plans for critical activities
2. **Resource Allocation** – assign most experienced team members to critical tasks
3. **Stakeholder Communication** – explain why certain activities require priority
4. **Progress Monitoring** – establish tighter monitoring intervals for critical activities
5. **Change Management** – resist scope changes that affect critical activities

### Critical Activities in Engineering Projects

| Project Type | Common Critical Activities | Typical Non-Critical Activities |
|-------------|---------------------------|--------------------------------|
| **Manufacturing** | Process equipment installation, commissioning, regulatory approval | Office refurbishment, staff training, documentation |
| **Construction** | Foundation work, structural frame, building envelope | Interior finishes, landscaping, ancillary buildings |
| **Product Development** | Prototype testing, tooling manufacture, regulatory certification | Marketing materials, user manual, packaging design |
| **IT Implementation** | Data migration, system integration testing, user acceptance | Report customisation, training material development |

### Case Study: Thames Tideway Tunnel

The £4.2 billion Thames Tideway Tunnel project identified tunnel boring as the critical activity, representing 7 years of the 9-year project schedule. The project team:

- Acquired custom-designed tunnel boring machines 18 months ahead of schedule
- Established 24/7 operations with triple-shift working
- Created dedicated risk mitigation protocols specifically for tunnelling operations
- Set up real-time monitoring systems to detect issues immediately

These measures ensured the critical tunnelling work remained on schedule despite encountering unexpected ground conditions (Tideway, 2020).

### Practice Identification

Which activities are critical?

```
┌──────────┬──────────┬─────────┬────────────┬──────────────┐
│ Activity │ Duration │ Depends │ Earliest   │ Latest       │
│          │ (months) │ on      │ Finish (EF)│ Finish (LF)  │
├──────────┼──────────┼─────────┼────────────┼──────────────┤
│ P        │ 3        │ -       │ 3          │ 3            │
│ Q        │ 2        │ P       │ 5          │ 7            │
│ R        │ 4        │ P       │ 7          │ 7            │
│ S        │ 3        │ Q, R    │ 10         │ 10           │
└──────────┴──────────┴─────────┴────────────┴──────────────┘
```

**Solution:**  
Critical activities are **P, R, and S** (all have zero slack: EF = LF)  
Non-critical activity is **Q** (slack = 7 - 5 = 2 months)  
**Critical Path:** P → R → S (total 10 months)

---

## Delays and Adjustments (10 minutes) | LO3.1

### Impact of Delays

When activities are delayed, the impact depends on whether the delayed activity is on the critical path:

1. **Critical Activity Delayed** → Project completion is delayed by the same amount
2. **Non-Critical Activity Delayed** → No impact if delay is within slack time; project delay if slack is exceeded

### Calculating Delay Impact

**Scenario:** A 3-week delay occurs. What is the impact?

```
BEFORE DELAY:
Week:    0    2    4    6    8    10   12
         |    |    |    |    |    |    |
A        [====]                          CRITICAL
B             [======]                   CRITICAL (delayed by 3 weeks)
C                   [====]               CRITICAL

Project completion: Week 12

AFTER 3-WEEK DELAY TO ACTIVITY B:
Week:    0    2    4    6    8    10   12   14   15
         |    |    |    |    |    |    |    |    |
A        [====]                          
B             [=========]                (now 9 weeks due to delay)
C                        [====]          

Project completion: Week 15 (delay of 3 weeks)
```

**Analysis:** Because Activity B was on the critical path, the 3-week delay causes a 3-week project delay. This demonstrates the **one-to-one relationship** between critical path delays and project delays.

### Adjustment Strategies

When delays occur, project managers have several options:

#### 1. Accept the Delay
Appropriate when:
- Stakeholder agreement can be obtained
- Contractual penalties are less than cost of acceleration
- Delay is on a non-critical activity with sufficient slack

#### 2. Fast-Tracking
**Definition:** Performing activities in parallel that were originally planned in sequence

**Example:**
```
ORIGINAL SEQUENCE:
Week:    0    2    4    6    8    10
         |    |    |    |    |    |
Design   [=======]
Build              [=======]

FAST-TRACKED:
Week:    0    2    4    6    8    10
         |    |    |    |    |    |
Design   [=======]
Build         [=======]  (Started 2 weeks early)
```

**Advantages:**
- Reduces overall project duration
- No additional resources required

**Disadvantages:**
- Increased risk (building starts before design complete)
- Potential rework costs
- Requires careful coordination

**Engineering Example:** On the Airbus A380 development project, systems integration testing began before software coding was complete, saving 6 months but resulting in significant rework when interface issues were discovered (Shenhar and Dvir, 2007).

#### 3. Crashing
**Definition:** Adding resources to reduce activity duration

**Example:**
```
NORMAL:
Activity X: 4 weeks with 2 staff = 8 person-weeks

CRASHED:
Activity X: 2 weeks with 4 staff = 8 person-weeks
```

**Advantages:**
- Proven method to reduce duration
- Controllable approach
- Can be applied selectively

**Disadvantages:**
- Increased cost (overtime, additional personnel)
- Diminishing returns (doubling staff rarely halves duration)
- Potential quality impacts from rushed work

**Cost Implications:**
Normal cost: £2,000/week × 4 weeks = £8,000  
Crashed cost: £2,800/week × 2 weeks = £5,600 + £3,000 mobilisation = £8,600  
**Crash cost premium:** £600 (7.5% increase)

#### 4. Resource Reallocation
Transfer resources from activities with slack to critical activities

**Example:**
```
Week:    0    2    4    6    8    10   12
         |    |    |    |    |    |    |
A        [====]■■                        (has slack)
B             [========]                  (critical - needs help)

REALLOCATION:
- Move 1 person from A to B
- B duration reduced from 8 to 6 weeks
- A extends from 4 to 5 weeks (but still within slack)
```

### Decision Framework for Delay Management

```
                    Is delayed activity
                    on critical path?
                          |
                  +-------+-------+
                  |               |
                 YES             NO
                  |               |
                  V               V
          Calculate delay    Check slack time
          impact on            remaining
          project                  |
                |            +-----+-----+
                |            |           |
                V        Sufficient   Insufficient
        Evaluate options:   slack       slack
        1. Fast-track           |           |
        2. Crash activity       V           V
        3. Extend deadline  No action   Apply crash
        4. Reduce scope     required    or fast-track
```

### Case Study: Rolls-Royce Trent XWB Engine

During development of the Trent XWB engine for the Airbus A350, high-pressure compressor testing revealed a 12-week delay on the critical path. Rolls-Royce's response:

- **Fast-tracked** low-pressure turbine assembly (started 4 weeks early)
- **Crashed** fan blade manufacturing (moved from single to double shift)
- **Reallocated** design engineers from non-critical acoustic testing to critical aerodynamic modifications

These combined strategies reduced the overall project delay from 12 weeks to 3 weeks, at a cost premium of approximately 8% (Rolls-Royce, 2013).

### Common Errors in Delay Management

❌ **Error:** Applying crash techniques to non-critical activities  
✅ **Correct:** Only crash critical activities (crashing non-critical activities wastes money)

❌ **Error:** Assuming all activities can be crashed equally  
✅ **Correct:** Some activities have practical limits (e.g., concrete curing cannot be rushed)

❌ **Error:** Failing to update the Gantt chart after adjustments  
✅ **Correct:** Always revise the chart to reflect new plan and communicate changes

---

## Resource Levelling and Schedule Compression (5 minutes) | LO3.1

### Resource Levelling

**Resource levelling** is the process of resolving resource over-allocation by adjusting activity start dates (within available slack) to create a more even distribution of resource demand.

### The Resource Over-Allocation Problem

```
Week:         1    2    3    4    5    6
Personnel     
Required:     
              
Project A:    3    3    -    -    -    -
Project B:    -    4    4    -    -    -
Project C:    2    2    2    2    -    -
              ─────────────────────────
TOTAL:        5    9    6    2    0    0   (Week 2: Over-allocated!)
Available:    6    6    6    6    6    6
```

**Problem:** Week 2 requires 9 people but only 6 available.

### Levelling Solution

Delay Project C (which has slack) by one week:

```
Week:         1    2    3    4    5    6
Personnel     
Required:     
              
Project A:    3    3    -    -    -    -
Project B:    -    4    4    -    -    -
Project C:    -    2    2    2    2    -  (delayed 1 week)
              ─────────────────────────
TOTAL:        3    9    6    2    2    0   
REVISED:      3    5    6    2    2    0   (all within capacity)
Available:    6    6    6    6    6    6
```

### Schedule Compression Summary

| Technique | How It Works | Cost Impact | Risk Impact | Best Used When |
|-----------|--------------|-------------|-------------|----------------|
| **Fast-tracking** | Parallel activities | Low | High | Activities have natural overlap potential |
| **Crashing** | Add resources | High | Medium | Deadline is firm, budget available |
| **Resource levelling** | Adjust timing | None | Low | Resource constraints exist |
| **Scope reduction** | Remove deliverables | None | Low | Stakeholders accept reduced scope |

### Engineering Applications

**Manufacturing:** During production ramp-up at a automotive plant, resource levelling ensured assembly line workers were not over-allocated whilst maintaining production targets (Meredith and Mantel, 2017).

**Construction:** On the Shard building in London, resource levelling of specialist glazing crews across 72 floors prevented bottlenecks and demobilisation costs (Sellar Property Group, 2012).

**Software:** Agile development teams use "sprint planning" which is essentially resource levelling across 2-week cycles (Schwaber and Sutherland, 2020).

---

## Software Tools for Gantt Charts (3 minutes) | LO3.1

### Industry-Standard Software

Whilst this unit focuses on manual Gantt chart construction (essential for examinations), professional project managers use software tools to manage complex schedules efficiently:

#### Microsoft Project
- **Market leader** (~45% of professional PM software users)
- Automatic critical path calculation
- Resource levelling algorithms
- Integration with Microsoft Office suite
- **Typical cost:** £500-£1,000 per licence

#### Primavera P6
- **Preferred for large engineering projects** (oil & gas, construction, infrastructure)
- Handles 100,000+ activities
- Advanced resource management
- **Used on:** Crossrail, Hinkley Point C, HS2
- **Typical cost:** £2,000-£3,000 per licence

#### Open-Source Alternatives
- **ProjectLibre** – free, similar to Microsoft Project
- **GanttProject** – lightweight, education-friendly
- **OpenProj** – community-supported

### Key Software Features

1. **Automatic calculation** of earliest/latest times and slack
2. **Resource histograms** showing over-allocation
3. **What-if scenario** modelling for delay analysis
4. **Progress tracking** with percentage complete indicators
5. **Report generation** for stakeholder communication

### Limitations of Software

❌ Software cannot replace project management judgement  
❌ "Garbage in, garbage out" – poor activity definition yields poor schedules  
❌ Over-reliance on software can reduce understanding of fundamentals  
✅ Software is a tool to implement decisions, not make them

### Examination Context

In the external examination, you will be expected to:
- Read and interpret Gantt charts manually
- Calculate slack time and identify critical activities without software
- Explain the principles that software automates

**Why manual skills matter:** Research by Thomas and Mengel (2008) shows that project managers who understand manual calculation techniques make better decisions when using software than those who rely solely on automated outputs.

---

## Conclusion and Summary (2 minutes) | LO3.1

### Key Learning Points

This session has equipped you with three essential Gantt chart skills:

1. **Slack Time Analysis**
   - Calculate slack time as LF - EF or LS - ES
   - Understand that slack provides scheduling flexibility
   - Recognise that slack can be consumed by delays

2. **Critical Activity Identification**
   - Critical activities have zero slack
   - Critical path is the longest path through the network
   - Delays to critical activities directly delay the project

3. **Delay Management**
   - Fast-tracking reduces duration by parallelising activities
   - Crashing reduces duration by adding resources
   - Only crash critical activities (crashing non-critical activities wastes resources)

### Practical Application

These skills enable you to:
- **Prioritise** limited resources effectively
- **Communicate** project status accurately to stakeholders
- **Respond** to delays strategically rather than reactively
- **Optimise** schedules to meet deadlines within budget constraints

### Preview of Next Week

**Week 13: Critical Path Analysis (CPA)** will extend these concepts by introducing network diagrams as an alternative representation method. You will learn to:
- Construct critical path network diagrams
- Calculate Earliest Start Times (EST) and Latest Finish Times (LFT) using forward and backward pass techniques
- Determine float time mathematically rather than visually

### Assessment Reminder

The external examination will assess your ability to:
- Complete partially-drawn Gantt charts accurately
- Calculate the impact of delays on project completion
- Identify critical activities and explain their significance
- Recommend appropriate schedule adjustments

**Revision tip:** Practice with past examination questions – Gantt chart questions typically worth 5-8 marks and test both calculation and interpretation skills.

---

## References

BAA (2008) *Heathrow Terminal 5: Project Management Success Factors*. London: British Airports Authority.

Meredith, J.R. and Mantel, S.J. (2017) *Project Management: A Managerial Approach*. 10th edn. Hoboken, NJ: Wiley.

National Audit Office (2018) *Crossrail: Progress Review*. HC 1965. London: NAO.

Project Management Institute (2021) *Pulse of the Profession 2021*. Newtown Square, PA: PMI.

Rolls-Royce (2013) *Trent XWB: Programme Management Case Study*. Derby: Rolls-Royce plc.

Schwaber, K. and Sutherland, J. (2020) *The Scrum Guide*. Available at: https://scrumguides.org (Accessed: 15 November 2024).

Sellar Property Group (2012) *The Shard: Construction Management*. London: Sellar Property Group.

Shenhar, A.J. and Dvir, D. (2007) *Reinventing Project Management: The Diamond Approach to Successful Growth and Innovation*. Boston, MA: Harvard Business School Press.

Thomas, J. and Mengel, T. (2008) 'Preparing project managers to deal with complexity – Advanced project management education', *International Journal of Project Management*, 26(3), pp. 304-315.

Tideway (2020) *Thames Tideway Tunnel: Programme Report*. London: Tideway Ltd.

Turner, J.R. and Müller, R. (2003) 'On the nature of the project as a temporary organization', *International Journal of Project Management*, 21(1), pp. 1-8.

---

## Glossary of Key Terms

**Concurrent Activities** – Activities that can be performed simultaneously

**Crashing** – Adding resources to reduce activity duration (at increased cost)

**Critical Activity** – An activity with zero slack time; delays directly impact project completion

**Critical Path** – The longest sequence of dependent activities through a project network; determines minimum project duration

**Dependent Activity** – An activity that cannot start until one or more predecessor activities are complete

**Fast-Tracking** – Performing activities in parallel that were originally planned in sequence

**Float Time** – See Slack Time

**Gantt Chart** – A bar chart that illustrates a project schedule, showing start and finish dates of activities

**Resource Levelling** – Adjusting activity start dates (within available slack) to resolve resource over-allocation

**Slack Time** – The amount of time an activity can be delayed without delaying the project; calculated as LF - EF

**Total Float** – See Slack Time

---

