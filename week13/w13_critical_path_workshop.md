# Week 13: Critical Path Analysis (CPA) - Workshop Activities

## Cambridge TECHNICALS Level 3 Engineering
### Unit 24: Project Management for Engineers

**Workshop Duration:** 30 minutes  
**Total Questions:** 7  
**Learning Outcome:** LO3.2 - How to use a critical path analysis

---

## Instructions

This workshop contains three sections:

- **Section 1:** Questions from past examination papers (verbatim)
- **Section 2:** Adapted questions based on past examination papers
- **Section 3:** New questions based on lecture content

Work through all questions systematically. Show all working for calculations. Solutions will be provided in a separate document.

---

## SECTION 1: Past Examination Questions

### Question 1 (2 marks)
**Source: June 2024, Question 3(b)(i)**

Study the critical path network diagram below:

```
     ┌───────────┐
     │  START    │
     │  Node 0   │
     └─────┬─────┘
           │
     ┌─────▼─────┐
     │Activity A │
     │Duration:7 │
     └─────┬─────┘
           │
     ┌─────▼─────┐
     │Activity B │
     │Duration:5 │
     └───────────┘
```

**Additional information:**
- Activity A: Earliest Start Time (EST) = 0
- Activity B: Latest Finish Time (LFT) = 7

**(a)** State the EST for Activity A.  
[1 mark]

**(b)** State the LFT for Activity B.  
[1 mark]

---

### Question 2 (2 marks)
**Source: January 2024, Question 3(a)**

An engineering project has the following critical path network:

```
     A (5 weeks) → B (8 weeks) → C (6 weeks) → D (4 weeks)
```

All activities shown are on the critical path.

**Explain one benefit to the project manager** of identifying which activities lie on the critical path.

Your answer must relate to the management of the project.

[2 marks]

---

## SECTION 2: Adapted Questions

### Question 3 (3 marks)
**Adapted from: June 2024, Question 3(b)(ii)**

Study the network diagram below for a manufacturing project:

```
           ┌─────────────┐
           │  Activity X │
     ┌────▶│  Duration:4 │────┐
     │     └─────────────┘    │
┌────┴────┐                   ▼
│Activity │              ┌─────────────┐
│    W    │              │  Activity Z │
│Duration:│              │  Duration:3 │
│    6    │              └─────────────┘
└────┬────┘                   ▲
     │     ┌─────────────┐    │
     └────▶│  Activity Y │────┘
           │  Duration:5 │
           └─────────────┘
```

The project must be completed in 9 days.

**(a)** Calculate the EST for Activity Z assuming the project starts at Day 0.  
[1 mark]

**(b)** Identify which activities are on the critical path.  
[1 mark]

**(c)** Explain why these activities are considered critical.  
[1 mark]

---

### Question 4 (12 marks)
**Adapted from: January 2022, Question 2(c)**

Falcon Aerospace Ltd is developing a new lightweight composite material for aircraft fuselage panels. The project involves multiple interdependent activities including laboratory testing, prototype manufacturing, and regulatory approval processes.

The project manager, Sarah Chen, is considering using Critical Path Analysis (CPA) to plan and manage this project.

**Evaluate the advantages of using Critical Path Analysis** for managing this aerospace materials development project.

You should consider:
- How CPA would help with planning the project
- How CPA would support project monitoring and control
- How CPA would assist with resource allocation
- The specific challenges of aerospace project management
- Any limitations of CPA in this context

Make a justified recommendation about whether CPA is appropriate for this project.

[12 marks - Levels of Response marking]

**Level 1 (1-3 marks):** Identifies advantages of CPA  
**Level 2 (4-6 marks):** Explains how CPA advantages apply  
**Level 3 (7-9 marks):** Analyses advantages with reference to aerospace context  
**Level 4 (10-12 marks):** Evaluates CPA's suitability with justified judgement

---

## SECTION 3: New Questions

### Question 5 (6 marks)

A civil engineering firm is managing a highway bridge replacement project with the following activities:

| Activity | Description | Duration (weeks) | Immediate Predecessors |
|----------|-------------|------------------|------------------------|
| A | Site clearance and preparation | 3 | None |
| B | Foundation excavation | 4 | A |
| C | Concrete foundation pour | 2 | B |
| D | Steel framework delivery | 5 | A |
| E | Bridge pier construction | 6 | C |
| F | Steel framework installation | 4 | D, E |
| G | Deck construction | 3 | F |
| H | Road surfacing | 2 | G |

**(a)** Calculate the Earliest Start Time (EST) for each activity using the forward pass method. Show your working.  
[3 marks]

**(b)** Determine the minimum project completion time.  
[1 mark]

**(c)** Which activity or activities represent merge points in the network? Explain why merge points are significant in CPA.  
[2 marks]

---

### Question 6 (8 marks)

A renewable energy company is installing a solar farm with the following project activities:

```
Activity Network Diagram:

      A(2)
     /    \
    /      \
  B(5)     C(4)
    |       |
    |       |
  D(3)     E(6)
    \      /
     \    /
      F(2)
```

Numbers in brackets indicate duration in weeks. All dependencies are finish-to-start.

**Given information:**
- EST(A) = 0
- LFT(F) = 13 weeks

**(a)** Complete the forward pass to calculate EST for all activities. Show all working.  
[2 marks]

**(b)** Complete the backward pass to calculate LFT for all activities. Show all working.  
[2 marks]

**(c)** Calculate the float time for Activities C and E.  
[2 marks]

**(d)** State the critical path and explain what this means for project management.  
[2 marks]

---

### Question 7 (5 marks)

An automotive manufacturer is developing a new electric vehicle battery system. The project network analysis reveals the following:

**Original Plan:**
- Critical Path: A → B → C → D → E
- Project Duration: 24 months
- Activity D (prototype testing) is on the critical path with duration of 6 months

**Scenario:** Activity D encounters problems and will now take 9 months instead of 6 months.

**(a)** Calculate the new project duration.  
[1 mark]

**(b)** Explain the impact of this delay on:
   - (i) The project completion date  
   [1 mark]
   
   - (ii) Activities with float time in the original network  
   [2 marks]

**(c)** As the project manager, recommend one action to mitigate the impact of this delay. Justify your recommendation.  
[1 mark]

---

## Time Management Guidance

**Suggested time allocation:**

- **Section 1** (Questions 1-2): 6 minutes
- **Section 2** (Questions 3-4): 10 minutes  
- **Section 3** (Questions 5-7): 14 minutes

Remember to show all working for calculations and refer to the specific context when answering evaluation questions.

---

## Assessment Criteria

These workshop questions align with the following Unit 24 assessment criteria:

**LO3.2 - How to use a critical path analysis:**
- Critical path network diagrams
- Earliest Start Times (EST)
- Latest Finish Times (LFT)
- Float time for an activity
- The identification of a project's critical path
- Minimum completion time
- Delays and adjustments
- Usefulness and importance of critical path analysis for project management

---

*Cambridge TECHNICALS Level 3 Engineering*  
*Unit 24: Project Management for Engineers*  
*Week 13 Workshop Activities*  
*December 2024*