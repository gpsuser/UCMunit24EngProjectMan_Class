# Week 13: Critical Path Analysis (CPA) - Slide Deck

## Cambridge TECHNICALS Level 3 Engineering
### Unit 24: Project Management for Engineers

---

<!-- _footer: '2' -->

# Table of Contents

| Section | Topic | Time | LO |
|---------|-------|------|-----|
| 1 | Introduction | 5 min | LO3.2 |
| 2 | What is CPA and Why Use It? | 6 min | LO3.2 |
| 3 | Network Diagram Fundamentals | 10 min | LO3.2 |
| 4 | Earliest Start Times (EST) | 10 min | LO3.2 |
| 5 | Latest Finish Times (LFT) | 10 min | LO3.2 |
| 6 | Float Time & Critical Path | 8 min | LO3.2 |
| 7 | Advantages & Applications | 6 min | LO3.2 |
| 8 | Conclusion | 5 min | LO3.2 |

---

<!-- _footer: '3' -->

# Learning Outcomes

**Aligned to:** Learning Outcome 3.2 - How to use a critical path analysis

By the end of this lecture, you will understand:
- The purpose and benefits of Critical Path Analysis in engineering projects
- How to construct and interpret critical path network diagrams
- How to calculate Earliest Start Times (EST) and Latest Finish Times (LFT)
- How to determine float time for activities
- How to identify the critical path and its significance
- The advantages of using CPA for project management

---

<!-- _footer: '4' -->

# Objectives

This session will enable you to:

1. Explain the purpose of CPA in engineering project management
2. Construct critical path network diagrams using standard notation
3. Calculate EST using the forward pass method
4. Calculate LFT using the backward pass method
5. Determine float time for individual activities
6. Identify the critical path within a project network
7. Evaluate the usefulness of CPA for managing engineering projects

---

<!-- _footer: '5' -->

# Introduction

**Critical Path Analysis (CPA)** is one of the most powerful project management tools available to engineers.

**Historical context:**
- Developed in the 1950s by DuPont and Remington Rand
- Designed for managing complex industrial projects
- Now an industry standard across construction, manufacturing, aerospace, and technology sectors

**Why it matters:**
Engineering projects involve numerous interdependent activities. CPA provides a systematic method for analysing these dependencies and identifying which activities directly impact project duration.

---

<!-- _footer: '6' -->

# What is CPA?

**Definition:**
Critical Path Analysis is a project management technique that identifies the sequence of activities that determines the minimum project duration.

**The "Critical Path":**
The longest path through the network of project activities, where any delay directly extends the overall project completion time.

**Key principle:**
Not all project activities are equally important for determining project duration – some have flexibility (float time), while others are critical.

---

<!-- _footer: '7' -->

# Key Components of CPA

**1. Network diagram**
Visual representation showing all project activities and dependencies

**2. Activity duration**
Time required to complete each task

**3. Dependencies**
Relationships between activities (which must be completed before others)

**4. Critical path**
Sequence of activities with zero float time

**5. Float time**
Amount of delay an activity can tolerate without affecting project duration

---

<!-- _footer: '8' -->

# Why Use CPA?

**Planning benefits:**
- Identifies logical sequence of activities before work begins
- Highlights dependencies that constrain scheduling
- Determines realistic minimum project duration

**Monitoring benefits:**
- Focuses attention on critical activities
- Identifies activities with scheduling flexibility
- Enables proactive risk management

**Resource management benefits:**
- Guides resource allocation to critical activities
- Identifies opportunities to redeploy resources
- Supports schedule compression decisions

---

<!-- _footer: '9' -->

# Network Diagram Fundamentals

**Activity-on-Node (AON) Notation:**
We use Activity-on-Node format where:
- Activities are represented as boxes (nodes)
- Arrows show dependencies between activities
- This is the most common format in modern project management software

**Key concept:**
Arrows connecting activities show precedence relationships. An arrow from Activity A to Activity B means B cannot start until A is completed.

---

<!-- _footer: '10' -->

# Standard Node Structure

```
┌─────────────────────────────────┐
│   Activity Description/Letter   │
├──────────┬──────────┬───────────┤
│   EST    │ Duration │    LFT    │
│ (Start)  │  (Days)  │  (Finish) │
└──────────┴──────────┴───────────┘
```

**Each node contains three key pieces of information:**

- **EST (Earliest Start Time):** Earliest time an activity can begin
- **Duration:** Time required to complete the activity
- **LFT (Latest Finish Time):** Latest time an activity can finish without delaying the project

---

<!-- _footer: '11' -->

# Example Network Structure

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

---

<!-- _footer: '12' -->

# Multiple Predecessors

**Important rule:**
When an activity has multiple predecessors, it **cannot start until ALL of them are complete**.

In our example:
- Activity E cannot begin until both D and C finish
- This creates a **merge point** in the network diagram

**Reading network diagrams:**
1. Start at the leftmost node(s) with no predecessors
2. Follow arrows to understand logical sequence
3. Identify merge points where multiple activities must complete
4. Locate rightmost node(s) representing project completion

---

<!-- _footer: '13' -->

# Earliest Start Times (EST) - Forward Pass

**Purpose:**
The forward pass determines the earliest possible start time for each activity, working from project start towards completion.

**Three key rules:**

**Rule 1:** EST for the first activity = 0 (or project start date)

**Rule 2:** For activities with a single predecessor:
```
EST = EST of predecessor + Duration of predecessor
```

**Rule 3:** For activities with multiple predecessors (merge points):
```
EST = Maximum of (EST + Duration) for all predecessors
```

---

<!-- _footer: '14' -->

# Forward Pass Example

Working left to right through our network:

**Step 1:** Activity A (project start)
- EST(A) = 0
- Completes at: 0 + 5 = Day 5

**Step 2:** Activities B and C (both depend on A)
- EST(B) = 0 + 5 = 5 (completes Day 13)
- EST(C) = 0 + 5 = 5 (completes Day 11)

**Step 3:** Activity D (depends on B)
- EST(D) = 5 + 8 = 13 (completes Day 15)

---

<!-- _footer: '15' -->

# Forward Pass Example (continued)

**Step 4:** Activity E (depends on both C and D - merge point)

Must wait for both paths:
- Path via C: 5 + 6 = 11
- Path via D: 13 + 2 = 15
- **EST(E) = Maximum(11, 15) = 15**
- Completes at: 15 + 4 = Day 19

**Project duration = 19 days**

**Key principle at merge points:**
Always use the **maximum** value because we must wait for ALL predecessors to complete.

---

<!-- _footer: '16' -->

# Common Forward Pass Errors

**Error 1: Forgetting to add duration**
- ❌ Incorrect: EST(B) = EST(A) = 0
- ✅ Correct: EST(B) = EST(A) + Duration(A) = 5

**Error 2: Using minimum instead of maximum at merge points**
- ❌ Incorrect: EST(E) = min(11, 15) = 11
- ✅ Correct: EST(E) = max(11, 15) = 15

**Error 3: Working out of sequence**
- ✅ Always calculate EST values from left to right
- ✅ Ensure all predecessors are complete before calculating an activity's EST

---

<!-- _footer: '17' -->

# Latest Finish Times (LFT) - Backward Pass

**Purpose:**
The backward pass determines the latest time each activity can finish without delaying the overall project.

**Three key rules:**

**Rule 1:** LFT for the final activity = project duration (from forward pass)

**Rule 2:** For activities with a single successor:
```
LFT = LFT of successor - Duration of successor
```

**Rule 3:** For activities with multiple successors (split points):
```
LFT = Minimum of (LFT - Duration) for all successors
```

---

<!-- _footer: '18' -->

# Backward Pass Example

Working backwards from right to left:

**Step 1:** Activity E (project end)
- LFT(E) = 19 (from forward pass)

**Step 2:** Activities D and C (predecessors of E)
- LFT(D) = 19 - 4 = 15
- LFT(C) = 19 - 4 = 15

**Step 3:** Activity B (predecessor of D)
- LFT(B) = 15 - 2 = 13

---

<!-- _footer: '19' -->

# Backward Pass Example (continued)

**Step 4:** Activity A (predecessor of both B and C - split point)

Must finish early enough for both paths:
- Path via B: 13 - 8 = 5
- Path via C: 15 - 6 = 9
- **LFT(A) = Minimum(5, 9) = 5**

**Key principle at split points:**
Always use the **minimum** value because delaying an activity affects ALL its successors.

**Verification check:**
For every activity: EST + Duration ≤ LFT
If violated, there's a calculation error.

---

<!-- _footer: '20' -->

# Float Time (Slack Time)

**Definition:**
Float time represents the amount of time an activity can be delayed without affecting overall project completion.

**Calculation formula:**
```
Float = LFT - (EST + Duration)
```

**Alternative formula:**
```
Float = (LFT - Duration) - EST
```

Both formulas yield the same result.

---

<!-- _footer: '21' -->

# Calculating Float Time - Example

For our product testing project:

| Activity | EST | Duration | LFT | Float |
|----------|-----|----------|-----|-------|
| A | 0 | 5 | 5 | 0 days |
| B | 5 | 8 | 13 | 0 days |
| C | 5 | 6 | 15 | 4 days |
| D | 13 | 2 | 15 | 0 days |
| E | 15 | 4 | 19 | 0 days |

**Activity C** has 4 days of float – it could be delayed by up to 4 days without affecting project completion.

---

<!-- _footer: '22' -->

# Identifying the Critical Path

**The Critical Path consists of all activities with zero float time.**

**In our example:**
Critical Path: **A → B → D → E**

Total duration: 5 + 8 + 2 + 4 = 19 days

**Key principle:**
Any delay in a critical activity extends the overall project duration.

**Note:** Complex projects may have multiple critical paths if several paths have the same maximum duration.

---

<!-- _footer: '23' -->

# Significance of the Critical Path

Understanding the critical path is essential because:

**1. Resource focus**
Critical activities deserve priority attention and resources

**2. Risk management**
Risks to critical activities pose direct threats to completion

**3. Schedule compression**
Reducing project duration requires speeding up critical activities

**4. Progress monitoring**
Critical activities require more frequent monitoring

**5. Stakeholder communication**
The critical path explains why the project requires its stated duration

---

<!-- _footer: '24' -->

# Real-World Example: Crossrail

**The £18.9 billion Crossrail project** (now Elizabeth Line) utilised CPA extensively:

- Coordinated thousands of interdependent activities
- 42km of new tunnels and 10 new stations
- Tunnel boring machine progress was on the critical path
- Required 24-hour operations and continuous monitoring
- Station fit-out activities had float time
- Allowed more flexible scheduling for non-critical work

CPA enabled project managers to prioritise resources effectively and focus attention where it mattered most.

---

<!-- _footer: '25' -->

# Advantages of CPA

**Planning advantages:**
- Logical framework for sequencing activities
- Identifies all dependencies before execution
- Establishes realistic project duration
- Creates baseline schedule for progress measurement

**Monitoring advantages:**
- Focuses management attention on critical activities
- Enables early identification of delays
- Distinguishes critical vs non-critical delays
- Supports data-driven corrective actions

---

<!-- _footer: '26' -->

# Advantages of CPA (continued)

**Resource management advantages:**
- Guides prioritisation of resource allocation
- Identifies opportunities to shift resources
- Reveals opportunities for concurrent activity execution
- Supports schedule compression

**Communication advantages:**
- Provides visual representation for all stakeholders
- Justifies project duration with logical analysis
- Explains constraints and dependencies
- Creates common language for schedule discussions

---

<!-- _footer: '27' -->

# Limitations of CPA

**Project managers should be aware:**

**1. Assumes fixed durations**
CPA treats activity durations as known constants (addressed by PERT technique)

**2. Doesn't consider resource constraints**
CPA assumes unlimited resources; actual projects face limitations

**3. Static analysis**
CPA provides a snapshot; regular updates needed as projects progress

**4. Complexity**
Very large projects may have thousands of activities, requiring software support

---

<!-- _footer: '28' -->

# When to Use CPA

CPA is most valuable for projects with:

- Multiple interdependent activities
- Clear activity definitions and durations
- Fixed scope (changes require network recalculation)
- Multiple potential critical paths requiring analysis
- Stakeholder need for schedule justification

**Software tools:**
- Microsoft Project
- Primavera P6
- ASTA Powerproject
- Online tools: Monday.com, Asana, TeamGantt

Understanding manual calculations ensures you can verify software outputs.

---

<!-- _footer: '29' -->

# Conclusion - Key Takeaways

**1.** CPA identifies the critical path that determines minimum project duration

**2.** Forward pass calculates EST (working left to right, maximum at merge points)

**3.** Backward pass calculates LFT (working right to left, minimum at split points)

**4.** Float time = LFT - (EST + Duration), indicating scheduling flexibility

**5.** Zero float activities are critical – any delay extends the project

**6.** CPA supports better decisions through proactive project management

---

<!-- _footer: '30' -->

# Summary

Critical Path Analysis is a powerful tool that enables engineering project managers to:

- Understand activity dependencies and sequencing
- Identify which activities directly impact project duration
- Focus resources and attention where they matter most
- Make informed decisions about schedule compression
- Communicate project constraints effectively to stakeholders

**Remember:** The critical path shows you where delays cannot be tolerated, while activities with float time provide scheduling flexibility for resource optimisation and risk management.

---