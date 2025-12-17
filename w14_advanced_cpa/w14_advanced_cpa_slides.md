# Week 14: Advanced Critical Path Analysis & Float Time

**Cambridge TECHNICALS Level 3 Engineering**  
Unit 24: Project Management for Engineers

---

<!-- _footer: 'Slide 2' -->

## Table of Contents

| Section | Time | LO |
|---------|------|-----|
| Introduction & Recap | 5 min | LO3.2 |
| Float Time: Definitions & Calculations | 12 min | LO3.2 |
| Types of Float & Implications | 10 min | LO3.2 |
| Advanced Critical Path Identification | 10 min | LO3.2 |
| Multiple Critical Paths | 8 min | LO3.2 |
| Schedule Compression Techniques | 10 min | LO3.2 |
| Conclusion & Exam Relevance | 5 min | LO3.2 |

---

<!-- _footer: 'Slide 3' -->

## Learning Outcomes

By the end of this session, you will be able to:

1. Calculate total float, free float and independent float for activities in a project network
2. Identify and explain the implications of multiple critical paths in complex engineering projects
3. Analyse the impact of delays and resource constraints on project completion time
4. Apply schedule compression techniques (crashing and fast-tracking) to optimise project delivery
5. Evaluate the usefulness and limitations of advanced critical path analysis
6. Make informed decisions about resource allocation using float time analysis

---

<!-- _footer: 'Slide 4' -->

## Objectives

This session builds on Week 13's CPA fundamentals to explore:

- **Advanced float time concepts** for better resource management
- **Multiple critical path scenarios** and their risks
- **Schedule compression strategies** for project recovery
- **Real-world applications** in major UK engineering projects

Understanding these advanced concepts is essential for managing complex engineering projects effectively.

---

<!-- _footer: 'Slide 5' -->

## Introduction

### Why Advanced CPA Matters

Major engineering projects like Crossrail demonstrate the critical importance of understanding float time and schedule management:

- **Crossrail**: 3 years delayed, £4 billion over budget
- Understanding which activities have flexibility (float) is crucial
- Effective schedule compression can save projects from catastrophic delays

Advanced CPA techniques enable **proactive project management** rather than reactive firefighting.

---

<!-- _footer: 'Slide 6' -->

## Quick Recap: CPA Fundamentals

```
Activity Network Notation:
┌─────────────┐  Duration
│  Activity   │
│    Label    │
├──────┬──────┤
│ EST  │ LFT  │
└──────┴──────┘

EST = Earliest Start Time
LFT = Latest Finish Time
```

**Critical Path**: Sequence of activities with zero float that determines minimum project duration

**Critical Activity**: Any activity on the critical path where EST = LFT

---

<!-- _footer: 'Slide 7' -->

## Float Time: What is It? (1/3)

**Float time** (or slack time) represents the amount of time an activity can be delayed without affecting:
- Subsequent activities, OR
- The overall project completion date

Float indicates **scheduling flexibility** and helps prioritise resource allocation.

Activities with **zero float** are critical and require intensive monitoring.

---

<!-- _footer: 'Slide 8' -->

## Float Time: Types (2/3)

### Total Float (TF)
Maximum time an activity can be delayed without delaying project completion

**Formula:**
```
Total Float = LFT - EST - Duration
```

### Free Float (FF)
Time an activity can be delayed without delaying the earliest start of any immediately following activity

**Formula:**
```
Free Float = Min EST of successors - (EST + Duration)
```

---

<!-- _footer: 'Slide 9' -->

## Float Time: Calculation Example (3/3)

**Thames Tideway Tunnel Project Example:**

Activity G: "Install primary sewage interception system"
- Duration: 8 weeks
- EST: Week 12
- LFT: Week 24

```
Total Float = 24 - 12 - 8 = 4 weeks
```

**Interpretation**: Activity G can start as late as Week 16 without delaying the project.

---

<!-- _footer: 'Slide 10' -->

## Interpreting Float Time

| Float Value | Interpretation | Management Implication |
|-------------|----------------|------------------------|
| 0 weeks | Critical activity | Must be monitored closely; any delay impacts project |
| 1-2 weeks | Near-critical | Monitor regularly; minimal flexibility |
| 3-5 weeks | Moderate float | Some flexibility; can absorb minor delays |
| >5 weeks | High float | Low monitoring priority; significant flexibility |

**Key principle**: Float belongs to the **project**, not individual activities.

---

<!-- _footer: 'Slide 11' -->

## Total Float vs Free Float: Practical Implications

**Heathrow Terminal 5 Baggage System Example:**

```
Activity A: Hardware (4 weeks, TF=0) → Critical
    ↓
Activity B: Software (3 weeks, TF=2, FF=0)
    ↓
Activity C: Testing (2 weeks, TF=2, FF=2)
    ↓
Activity D: Training (2 weeks, TF=0) → Critical
```

**Key insight**: Activity B has total float but zero free float
- Delaying B won't affect overall completion
- BUT it will delay Activity C's start
- Requires coordination between teams

---

<!-- _footer: 'Slide 12' -->

## Negative Float

**Occurs when**: Imposed deadlines create situations where LFT < EST + Duration

**Example:**
```
Activity imposed deadline: Week 20
EST + Duration: Week 22
Negative Float: 20 - 22 = -2 weeks
```

**Causes**: External constraints, regulatory deadlines, resource windows

**Implications**: 
- Project is already late before it starts
- Requires schedule compression
- Risk of quality compromises

---

<!-- _footer: 'Slide 13' -->

## Float Ownership & Consumption

**Critical principle**: Float belongs to the **project**, not individual activities.

**Challenge**: If Activity B's manager uses all 2 weeks of float, Activity C loses its scheduling flexibility even though C had float.

**Best practices**:
- Centralized float management by project manager
- Float consumption must be approved
- Regular monitoring of float usage
- Document all float consumption decisions

---

<!-- _footer: 'Slide 14' -->

## Near-Critical Paths

**Definition**: Activity paths with very low float (typically 1-3 weeks) that could easily become critical if minor delays occur.

**Identification**: Calculate total float for all paths; identify paths with float < 5% of project duration.

**Risk management strategies**:
- Apply contingency buffers to near-critical activities
- Pre-allocate premium resources
- Develop fast-track options
- Monitor as closely as critical paths

---

<!-- _footer: 'Slide 15' -->

## Critical Path Drag

**Critical Path Drag**: The amount of time an activity adds to the project duration.

**Formula:**
```
Drag = Minimum of (Activity Duration, Total Float of parallel paths)
```

**Example:**
```
Critical Activity E: Duration 6 weeks
Parallel non-critical path has TF = 2 weeks
Drag = Min(6, 2) = 2 weeks
```

**Application**: Identifies which critical activities, if reduced, would have greatest impact on shortening project duration.

---

<!-- _footer: 'Slide 16' -->

## Multiple Critical Paths: When They Occur

Multiple critical paths occur when two or more paths have:
- Identical duration
- Zero float
- All activities with EST = LFT

**Example Network:**
```
        Path A: 14 weeks (Critical)
Start ──┬──→ Activities A-B-C-D ──→ End
        │   
        └──→ Activities E-F-G-H ──→
        Path B: 14 weeks (Critical)
```

Both paths are critical with zero float.

---

<!-- _footer: 'Slide 17' -->

## Implications of Multiple Critical Paths

**Increased Risk**:
- Risk probability multiplies, not adds
- Path A: 10% delay risk + Path B: 10% delay risk
- Project delay risk ≈ 19%
- Formula: 1 - (0.9 × 0.9) = 0.19

**Resource Challenges**:
- Cannot reallocate resources between critical paths
- Both require premium resources simultaneously
- Increased costs and scheduling complexity

**Monitoring Burden**:
- Must track all critical paths simultaneously
- Greater coordination overhead

---

<!-- _footer: 'Slide 18' -->

## Real-World Example: Crossrail Project

Crossrail experienced multiple critical paths during fit-out phase:

```
Path 1: Station construction → Track installation → Signalling
Path 2: Station construction → Platform screen doors → Testing  
Path 3: Rolling stock delivery → Driver training → Safety certification
```

All three paths became critical in 2018-2019, contributing to the three-year delay.

**Lessons learned**: Early identification, enhanced risk mitigation, close coordination between parallel work streams.

---

<!-- _footer: 'Slide 19' -->

## Managing Multiple Critical Paths

**Strategy 1: Critical Chain Method**
- Add buffer activities before merge points
- Pool contingency at merge points

**Strategy 2: Path Convergence Analysis**
- Identify where multiple paths merge
- Apply additional resources at convergence points

**Strategy 3: Risk Prioritisation**
- Assess delay probability for each path
- Focus intensive management on highest-risk path
- Develop independent contingency plans

---

<!-- _footer: 'Slide 20' -->

## Schedule Compression: Crashing (1/2)

**Definition**: Reducing activity duration by adding resources (at increased cost).

**When to apply**:
- Project has negative float (already late)
- Contractual penalties exceed crashing cost
- Market window closing
- Regulatory deadline cannot be moved

**Process**:
1. Identify crashable critical activities
2. Calculate cost per time unit saved
3. Select activity with lowest cost/time ratio
4. Recalculate critical path (may change!)
5. Repeat if needed

---

<!-- _footer: 'Slide 21' -->

## Schedule Compression: Crashing (2/2)

**Thames Tideway Tunnel Example:**

```
Activity: "Excavate main tunnel section"
- Normal duration: 24 weeks, Cost: £45M
- Crash duration: 18 weeks, Cost: £54M

Cost slope = (£54M - £45M) / (24-18) = £1.5M per week
```

**Decision**: Crash if contractual penalty or opportunity cost > £1.5M per week

**Limitations**: Only works on critical path; diminishing returns; may compromise quality

---

<!-- _footer: 'Slide 22' -->

## Schedule Compression: Fast-Tracking (1/2)

**Definition**: Performing activities in parallel that would normally be done in sequence.

**Example:**
```
Traditional: Design 100% → Procurement → Construction

Fast-tracked: Design 60% → Procurement starts
              Design 100% → Construction (based on 60% design)
```

**Advantages**:
- No additional cost (unlike crashing)
- Can significantly reduce project duration
- Maintains activity durations

---

<!-- _footer: 'Slide 23' -->

## Schedule Compression: Fast-Tracking (2/2)

**Risks and challenges**:
- Increased rework if early work needs changes
- Higher coordination complexity
- Potential quality issues
- Communication overhead increases

**Heathrow Terminal 5 Example:**
- Fast-tracked M&E installation during architectural works
- Benefits: 6-month schedule reduction
- Challenges: 12% rework rate due to design changes

---

<!-- _footer: 'Slide 24' -->

## Schedule Compression Decision Matrix

| Technique | When to Use | Cost Impact | Risk Impact | Quality Impact |
|-----------|-------------|-------------|-------------|----------------|
| **Crashing** | Late project, high penalties | High (++) | Low (+) | Medium (+) |
| **Fast-Tracking** | Early phase, design flexibility | Low (+) | High (++) | High (++) |
| **Combined** | Critical project, resources available | Very High (+++) | Very High (+++) | High (++) |

**Key consideration**: Combined approach multiplies risks and requires intensive management oversight.

---

<!-- _footer: 'Slide 25' -->

## Conclusion: Key Takeaways

1. **Float time** provides scheduling flexibility but must be managed as a project resource

2. **Multiple critical paths** increase project risk and management complexity exponentially

3. **Schedule compression** techniques (crashing and fast-tracking) offer recovery options but at increased cost and risk

4. **Advanced CPA** enables proactive project management rather than reactive firefighting

Understanding these concepts is essential for managing complex engineering projects successfully.

---

<!-- _footer: 'Slide 26' -->

## Examination Relevance (1/2)

Recent exam papers have tested:

**Calculation Skills** (January 2024, Q3a):
- Benefits of critical path identification
- Understanding of float time and flexibility

**Analytical Skills** (June 2024, Q3b):
- Identifying EST and LFT from network diagrams
- Determining critical activities
- Explaining why activities are critical (zero float)

---

<!-- _footer: 'Slide 27' -->

## Examination Relevance (2/2)

**Evaluation Skills** (January 2022, Q2c - 12 marks):
- Evaluating advantages of CPA for specific projects
- Demonstrating understanding of float time, resource optimization
- Requires contextual application to scenarios

**Exam tips**:
- Practice calculating float time manually
- Understand **why** activities are critical, not just which
- Explain schedule compression trade-offs
- Use engineering project examples in extended answers

---

<!-- _footer: 'Slide 28' -->

## Links to Other Learning Outcomes

Advanced CPA skills support:

- **LO1.2** (Project Planning): Resource planning benefits from float analysis

- **LO2.2** (PM Skills): Decision-making and problem-solving with schedule compression

- **LO4.5** (Information Use): Using CPA data to make project decisions

- **LO5.1** (Monitoring): Comparing actual progress against planned float consumption

---

<!-- _footer: 'Slide 29' -->

## Professional Practice

In professional engineering project management:

- CPA is **mandated** in construction contracts (NEC4, FIDIC)
- Float ownership is specified in contract terms
- Schedule updates required **monthly** (minimum)
- Critical path claims form basis of delay compensation
- Advanced CPA skills are highly valued by employers

Engineers combining technical expertise with project management skills are better positioned for career success.

---

<!-- _footer: 'Slide 30' -->

## Summary

Today we covered:

✓ Float time calculations (total, free, independent)  
✓ Types of float and their implications  
✓ Advanced critical path identification techniques  
✓ Multiple critical paths and associated risks  
✓ Schedule compression techniques (crashing and fast-tracking)  

**Next steps**: Practice these techniques through workshop activities and apply them to real engineering project scenarios.

**Remember**: Advanced CPA is a powerful tool for managing complexity in engineering projects.

---