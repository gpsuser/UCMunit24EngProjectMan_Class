# Week 13: Critical Path Analysis (CPA)

## Cambridge TECHNICALS Level 3 Engineering
### Unit 24: Project Management for Engineers

**Lecture Duration:** 55 minutes  
**Workshop Duration:** 30 minutes  
**Break:** 5 minutes

---

## Table of Contents

| Section | Topic | Time | Learning Outcome |
|---------|-------|------|------------------|
| 1 | Introduction and objectives | 5 min | LO3.2 |
| 2 | What is CPA and why use it? | 6 min | LO3.2 |
| 3 | Network diagram fundamentals | 10 min | LO3.2 |
| 4 | Earliest Start Times (EST) - Forward pass | 10 min | LO3.2 |
| 5 | Latest Finish Times (LFT) - Backward pass | 10 min | LO3.2 |
| 6 | Float time and critical path identification | 8 min | LO3.2 |
| 7 | Advantages and practical applications | 5 min | LO3.2 |
| 8 | Conclusion and summary | 1 min | LO3.2 |
| | **BREAK** | **5 min** | |
| 9 | Workshop activities | 30 min | LO3.2 |

---

## Learning Objectives

By the end of this lecture, learners will be able to:

1. Explain the purpose and benefits of Critical Path Analysis (CPA) in engineering project management
2. Construct and interpret critical path network diagrams using standard notation
3. Calculate Earliest Start Times (EST) using the forward pass method
4. Calculate Latest Finish Times (LFT) using the backward pass method
5. Determine float time for individual activities within a project network
6. Identify the critical path and explain its significance for project duration
7. Analyse the impact of delays and adjustments on project completion times
8. Evaluate the usefulness of CPA for managing engineering projects

**Aligned to:** Learning Outcome 3.2 - How to use a critical path analysis

---

## 1. Introduction (5 minutes)

### Context

Critical Path Analysis (CPA), also known as Critical Path Method (CPM), is one of the most powerful project management tools available to engineers. Originally developed in the 1950s by DuPont and Remington Rand for managing complex industrial projects, CPA has become an industry standard across construction, manufacturing, aerospace, and technology sectors (Meredith and Mantel, 2012).

### Why CPA Matters in Engineering

Engineering projects typically involve numerous interdependent activities. Consider a bridge construction project: foundation work must be completed before pier construction, which must precede deck installation. CPA provides a systematic method for analysing these dependencies, identifying which activities directly impact project duration, and optimising resource allocation (Burke, 2013).

### Week 13 in Context

This session builds on Week 11-12 (Gantt Charts) by introducing more sophisticated scheduling analysis. Next week (Week 14), learners will extend CPA skills to calculate float time and manage resource constraints. Week 15 will introduce PERT (Program Evaluation and Review Technique), which incorporates uncertainty into CPA calculations.

---

## 2. What is CPA and Why Use It? (6 minutes)

### Definition

**Critical Path Analysis** is a project management technique that identifies the sequence of activities that determines the minimum project duration. The "critical path" is the longest path through the network of project activities, where any delay directly extends the overall project completion time (Lock, 2014).

### Key Components

CPA consists of several interconnected elements:

1. **Network diagram:** A visual representation showing all project activities and their dependencies
2. **Activity duration:** The time required to complete each task
3. **Dependencies:** The relationships between activities (which must be completed before others can start)
4. **Critical path:** The sequence of activities with zero float time
5. **Float time:** The amount of delay an activity can tolerate without affecting project duration

### Why Use CPA?

Engineering projects benefit from CPA in multiple ways:

**Planning benefits:**
- Identifies the logical sequence of activities before work begins
- Highlights dependencies that constrain scheduling flexibility
- Determines realistic minimum project duration (Kerzner, 2017)

**Monitoring benefits:**
- Focuses attention on critical activities that directly impact completion
- Identifies activities with scheduling flexibility (float time)
- Enables proactive risk management by highlighting vulnerable points

**Resource management benefits:**
- Guides resource allocation to critical activities
- Identifies opportunities to redeploy resources from non-critical activities
- Supports schedule compression decisions

### Real-World Example: Crossrail Project

The £18.9 billion Crossrail project (now Elizabeth Line) utilised CPA extensively to coordinate thousands of interdependent activities across 42km of new tunnels and 10 new stations. CPA enabled project managers to identify that tunnel boring machine progress was on the critical path, requiring priority focus, while station fit-out activities had float time allowing more flexible scheduling (National Audit Office, 2014).

---

## 3. Network Diagram Fundamentals (10 minutes)

### Activity-on-Node (AON) Notation

This course uses Activity-on-Node notation, where activities are represented as boxes (nodes) connected by arrows showing dependencies. This is the most common format in modern project management software (PMI, 2017).

### Standard Node Structure

```
┌─────────────────────────────────┐
│   Activity Description/Letter   │
├──────────┬──────────┬───────────┤
│   EST    │ Duration │    LFT    │
│  (Start) │  (Days)  │  (Finish) │
└──────────┴──────────┴───────────┘
```

Each node contains three key pieces of information:

- **EST (Earliest Start Time):** The earliest time an activity can begin, considering all preceding activities
- **Duration:** The time required to complete the activity
- **LFT (Latest Finish Time):** The latest time an activity can finish without delaying the project

### Dependency Arrows

Arrows connect activities to show precedence relationships. An arrow from Activity A to Activity B indicates that B cannot start until A is completed. This is called a "finish-to-start" dependency, the most common relationship in engineering projects (Harrison and Lock, 2017).

### Example Network - Small Engineering Project

Consider a simplified product testing project:

**Activities:**
- A: Design test rig (5 days)
- B: Procure test equipment (8 days) - depends on A
- C: Manufacture prototype (6 days) - depends on A
- D: Calibrate equipment (2 days) - depends on B
- E: Conduct tests (4 days) - depends on C and D

```
         A (5)
        /     \
       /       \
    B (8)      C (6)
      |          |
    D (2)        |
      \         /
       \       /
        E (4)
```

This simple network already reveals important scheduling relationships: both the equipment path (A→B→D→E) and the prototype path (A→C→E) must be considered when determining project duration.

### Multiple Predecessors

When an activity has multiple predecessors, it cannot start until ALL of them are complete. In the example above, Activity E cannot begin until both D and C finish. This creates a merge point in the network diagram.

### Reading Network Diagrams

To interpret a network diagram effectively:

1. Start at the leftmost node(s) with no predecessors
2. Follow arrows to understand the logical sequence
3. Identify merge points where multiple activities must complete
4. Locate the rightmost node(s) that represent project completion

---

## 4. Earliest Start Times (EST) - Forward Pass (10 minutes)

### Purpose of EST Calculation

The forward pass through the network determines the earliest possible start time for each activity, working from the project start towards completion. This establishes the minimum project duration and provides the foundation for identifying the critical path (Maylor, 2010).

### Forward Pass Rules

**Rule 1:** The EST for the first activity (or activities) is zero (or the project start date).

**Rule 2:** For activities with a single predecessor:
```
EST = EST of predecessor + Duration of predecessor
```

**Rule 3:** For activities with multiple predecessors (merge points):
```
EST = Maximum of (EST + Duration) for all predecessors
```

The merge point rule is crucial: an activity cannot start until ALL its predecessors are complete, so we take the longest path to that point (APM, 2019).

### Worked Example: Product Testing Project

Let's calculate EST values for our example project. We work from left to right:

**Step 1:** Activity A (project start)
- EST(A) = 0
- Activity A completes at: 0 + 5 = Day 5

**Step 2:** Activities B and C (both depend on A)
- EST(B) = EST(A) + Duration(A) = 0 + 5 = 5
- EST(C) = EST(A) + Duration(A) = 0 + 5 = 5
- Activity B completes at: 5 + 8 = Day 13
- Activity C completes at: 5 + 6 = Day 11

**Step 3:** Activity D (depends on B)
- EST(D) = EST(B) + Duration(B) = 5 + 8 = 13
- Activity D completes at: 13 + 2 = Day 15

**Step 4:** Activity E (depends on both C and D - merge point)
- Path via C: EST(C) + Duration(C) = 5 + 6 = 11
- Path via D: EST(D) + Duration(D) = 13 + 2 = 15
- EST(E) = Maximum(11, 15) = 15 (must wait for both paths)
- Activity E completes at: 15 + 4 = Day 19

**Project duration = 19 days** (the completion of the final activity)

### Common Errors to Avoid

**Error 1:** Forgetting to add duration
- Incorrect: EST(B) = EST(A) = 0
- Correct: EST(B) = EST(A) + Duration(A) = 5

**Error 2:** Using minimum instead of maximum at merge points
- Incorrect: EST(E) = min(11, 15) = 11
- Correct: EST(E) = max(11, 15) = 15

**Error 3:** Working out of sequence
- Always calculate EST values from left to right, ensuring all predecessors are complete before calculating an activity's EST

### Practice Checkpoint

*Pause here to ensure learners understand the forward pass before proceeding to backward pass calculations.*

---

## 5. Latest Finish Times (LFT) - Backward Pass (10 minutes)

### Purpose of LFT Calculation

The backward pass determines the latest time each activity can finish without delaying the overall project. This calculation is essential for identifying which activities have scheduling flexibility and which are critical (CIOB, 2010).

### Backward Pass Rules

**Rule 1:** The LFT for the final activity equals its earliest finish time (the project duration we calculated in the forward pass).

**Rule 2:** For activities with a single successor:
```
LFT = LFT of successor - Duration of successor
```

**Rule 3:** For activities with multiple successors (split points):
```
LFT = Minimum of (LFT - Duration) for all successors
```

At split points, we take the minimum because delaying an activity affects all its successors; we must finish early enough to accommodate the most constraining successor (Burke, 2013).

### Worked Example: Product Testing Project (Backward Pass)

Now we work backwards from right to left through our network:

**Step 1:** Activity E (project end)
- Earliest finish = 19 days (from forward pass)
- LFT(E) = 19

**Step 2:** Activities D and C (both predecessors of E)

For Activity D:
- LFT(D) = LFT(E) - Duration(E) = 19 - 4 = 15

For Activity C:
- LFT(C) = LFT(E) - Duration(E) = 19 - 4 = 15

**Step 3:** Activity B (predecessor of D)
- LFT(B) = LFT(D) - Duration(D) = 15 - 2 = 13

**Step 4:** Activity A (predecessor of both B and C - split point)
- Path via B: LFT(B) - Duration(B) = 13 - 8 = 5
- Path via C: LFT(C) - Duration(C) = 15 - 6 = 9
- LFT(A) = Minimum(5, 9) = 5 (must finish early enough for both paths)

### Completed Network Diagram

```
     A: EST=0, LFT=5 (Duration: 5 days)
           /                    \
          /                      \
  B: EST=5, LFT=13         C: EST=5, LFT=15
     (Duration: 8)             (Duration: 6)
          |                           |
  D: EST=13, LFT=15                  |
     (Duration: 2)                   |
          \                          /
           \                        /
              E: EST=15, LFT=19
                (Duration: 4)
```

### Verification Check

For every activity, the relationship must hold:
```
EST + Duration ≤ LFT
```

If this inequality is violated, there's a calculation error. In our example:
- Activity A: 0 + 5 = 5 ≤ 5 ✓
- Activity B: 5 + 8 = 13 ≤ 13 ✓
- Activity C: 5 + 6 = 11 ≤ 15 ✓
- Activity D: 13 + 2 = 15 ≤ 15 ✓
- Activity E: 15 + 4 = 19 ≤ 19 ✓

---

## 6. Float Time and Critical Path Identification (8 minutes)

### What is Float Time?

**Float time** (also called slack time) represents the amount of time an activity can be delayed without affecting the overall project completion date. It provides scheduling flexibility for resource allocation and risk management (Kerzner, 2017).

### Calculating Float Time

```
Float = LFT - (EST + Duration)
```

Alternatively:
```
Float = (LFT - Duration) - EST
```

Both formulas are equivalent and yield the same result.

### Float Time in Our Example

**Activity A:**
Float = 5 - (0 + 5) = 0 days

**Activity B:**
Float = 13 - (5 + 8) = 0 days

**Activity C:**
Float = 15 - (5 + 6) = 4 days

**Activity D:**
Float = 15 - (13 + 2) = 0 days

**Activity E:**
Float = 19 - (15 + 4) = 0 days

### Identifying the Critical Path

The **critical path** consists of all activities with zero float time. These activities directly determine project duration; any delay in a critical activity extends the project (Lock, 2014).

In our example:
**Critical Path: A → B → D → E** (total duration: 5 + 8 + 2 + 4 = 19 days)

Activity C is not on the critical path. It has 4 days of float, meaning it could be delayed by up to 4 days without affecting the project completion date of Day 19.

### Multiple Critical Paths

Complex projects may have multiple critical paths. For example, if Activity C had a duration of 10 days instead of 6 days, both paths (A→B→D→E and A→C→E) would be critical, with zero float on all activities.

### Significance of the Critical Path

Understanding the critical path is essential for project managers because:

1. **Focus resources:** Critical activities deserve priority attention and resources
2. **Risk management:** Risks to critical activities pose direct threats to completion
3. **Schedule compression:** Reducing project duration requires speeding up critical activities
4. **Progress monitoring:** Critical activities require more frequent monitoring
5. **Stakeholder communication:** The critical path explains why the project requires its stated duration

### Real-World Application: Thames Tideway Tunnel

The £4.9 billion Thames Tideway Tunnel super-sewer project used CPA to manage interdependencies across 25km of tunnel construction. Tunnelling activities were on the critical path, requiring 24-hour operations and continuous monitoring, while some shaft construction activities had float time, allowing for more flexible scheduling and resource allocation (Thames Tideway Tunnel, 2016).

---

## 7. Advantages and Practical Applications (5 minutes)

### Advantages of Critical Path Analysis

**Planning advantages:**
- Provides a logical framework for sequencing project activities
- Identifies all dependencies before project execution begins
- Establishes realistic project duration based on activity relationships
- Creates a baseline schedule against which progress can be measured

**Monitoring advantages:**
- Focuses management attention on activities that directly impact completion
- Enables early identification of delays that threaten project objectives
- Distinguishes between critical delays (affecting project) and non-critical delays
- Supports data-driven decisions about corrective actions

**Resource management advantages:**
- Guides prioritisation of resource allocation to critical activities
- Identifies opportunities to shift resources from activities with float
- Reveals opportunities for concurrent activity execution
- Supports schedule compression through targeted interventions

**Communication advantages:**
- Provides a visual representation understandable to all stakeholders
- Justifies project duration with logical dependency analysis
- Explains why certain activities cannot be accelerated without additional resources
- Creates a common language for discussing schedule issues (APM, 2019)

### Limitations to Consider

While CPA is powerful, project managers should be aware of its limitations:

1. **Assumes fixed durations:** CPA treats activity durations as known constants, which may not reflect reality (addressed by PERT in Week 15)
2. **Doesn't consider resource constraints:** CPA assumes unlimited resources; actual projects face resource limitations
3. **Static analysis:** CPA provides a snapshot; regular updates are needed as projects progress
4. **Complexity:** Very large projects may have thousands of activities, making CPA unwieldy without software support (Meredith and Mantel, 2012)

### Software Tools

Modern project management software automates CPA calculations:
- **Microsoft Project:** Industry standard for construction and engineering
- **Primavera P6:** Preferred for large-scale infrastructure projects
- **ASTA Powerproject:** Popular in UK construction industry
- **Online tools:** Monday.com, Asana, TeamGantt offer simpler interfaces

However, understanding manual calculations ensures project managers can verify software outputs and troubleshoot problems (Harrison and Lock, 2017).

### When to Use CPA

CPA is most valuable for projects with:
- Multiple interdependent activities
- Clear activity definitions and durations
- Fixed scope (changes require network recalculation)
- Multiple potential critical paths requiring analysis
- Stakeholder need for schedule justification

---

## 8. Conclusion and Summary (1 minute)

### Key Takeaways

1. **CPA identifies the critical path:** The sequence of activities that determines minimum project duration
2. **Forward pass calculates EST:** Working left to right, using maximum at merge points
3. **Backward pass calculates LFT:** Working right to left, using minimum at split points
4. **Float time = LFT - (EST + Duration):** Indicates scheduling flexibility
5. **Zero float activities are critical:** Any delay extends the project
6. **CPA supports better decisions:** Enables proactive project management and resource optimisation

### Looking Ahead

- **Week 14:** Advanced CPA techniques including complex network analysis, resource levelling, and schedule compression methods (crashing and fast-tracking)
- **Week 15:** PERT technique for handling uncertainty in activity duration estimates
- **Week 16:** Integration of Gantt charts, CPA, and PERT for comprehensive project planning


---

## References

Association for Project Management (APM) (2019) *APM Body of Knowledge*. 7th edn. Buckinghamshire: Association for Project Management.

Burke, R. (2013) *Project Management: Planning and Control Techniques*. 5th edn. Chichester: John Wiley & Sons.

Chartered Institute of Building (CIOB) (2010) *Guide to Good Practice in the Management of Time in Complex Projects*. Oxford: Wiley-Blackwell.

Harrison, F. and Lock, D. (2017) *Advanced Project Management: A Structured Approach*. 5th edn. Abingdon: Routledge.

Kerzner, H. (2017) *Project Management: A Systems Approach to Planning, Scheduling, and Controlling*. 12th edn. Hoboken, NJ: John Wiley & Sons.

Lock, D. (2014) *Project Management*. 10th edn. Farnborough: Gower Publishing.

Maylor, H. (2010) *Project Management*. 4th edn. Harlow: Pearson Education.

Meredith, J.R. and Mantel, S.J. (2012) *Project Management: A Managerial Approach*. 8th edn. Hoboken, NJ: John Wiley & Sons.

National Audit Office (2014) *Crossrail*. London: National Audit Office. Available at: https://www.nao.org.uk/reports/crossrail/ (Accessed: 8 December 2024).

Project Management Institute (PMI) (2017) *A Guide to the Project Management Body of Knowledge (PMBOK Guide)*. 6th edn. Newtown Square, PA: Project Management Institute.

Thames Tideway Tunnel (2016) *Development Consent Order Application*. London: Thames Water. Available at: https://www.tideway.london (Accessed: 8 December 2024).

---

## Word Count

**Lecture content (excluding table of contents, references, title pages):** 3,247 words

---

