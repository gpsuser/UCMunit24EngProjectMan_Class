# Week 12: Gantt Chart Practice – Workshop Activities

**Unit 24: Project Management for Engineers**  
**Cambridge TECHNICALS Level 3 Engineering**  
**Duration:** 30 minutes  
**Learning Outcome:** LO3.1 – How to use and interpret a Gantt chart

---

## Instructions for Students

This workshop contains **7 questions** divided into three sections:

- **Section 1 (Questions 1-2):** Past examination questions – practice under exam conditions
- **Section 2 (Questions 3-4):** Adapted examination questions – similar style, different context
- **Section 3 (Questions 5-7):** New practice questions – additional application opportunities

**Time Management:**
- Aim to spend approximately 4 minutes per question
- Show all working for calculation questions
- Use rulers and pencils for drawing/completing Gantt charts

**Helpful Hints:**
- Read all information carefully before starting
- Check whether activities have dependencies
- Remember: Slack Time = Latest Finish - Earliest Finish
- Critical activities have ZERO slack time

**Materials Needed:**
- Pencil and ruler
- Calculator (optional – most questions are non-calculator)
- Eraser

---

## Section 1: Past Examination Questions

### Question 1 (Based on Jan24 Q2(b)(i)) | 6 marks | LO3.1

**Scenario:** HD Tyre Ltd is implementing a carbon reduction project at its headquarters. The project comprises four phases:

| Phase | Description | Duration | Depends on |
|-------|-------------|----------|------------|
| A | Conduct energy audit | 3 months | - |
| B | Install LED lighting | 4 months | Phase A |
| C | Upgrade HVAC system | 10 months | Phase B |
| D | Final commissioning | 1 month | Phase C |

**(a)** Complete the Gantt chart below to show **all four phases** of the project. The chart for Phase A has been drawn for you.

```
Month:    0    2    4    6    8    10   12   14   16   18
          |    |    |    |    |    |    |    |    |    |
Phase A   [===]

Phase B   

Phase C   

Phase D   

```

**Mark Scheme:**
- 2 marks for Phase B (correct start point and duration)
- 2 marks for Phase C (correct start point and duration)
- 2 marks for Phase D (correct start point and duration)

**Total: 6 marks**

---

### Question 2 (Based on Jun23 Q3(c)(ii)) | 2 marks | LO3.1

**Scenario:** An engineering project has the following activity information:

| Activity | Duration (weeks) | Earliest Finish (EF) | Latest Finish (LF) |
|----------|------------------|---------------------|-------------------|
| A | 4 | 4 | 4 |
| B | 3 | 7 | 10 |
| C | 6 | 10 | 10 |
| D | 2 | 12 | 12 |

**Statement:** "Activity C is a critical activity."

**Required:**

**(a)** State whether you **agree** or **disagree** with this statement. (1 mark)

**(b)** Explain your answer with reference to the data provided. (1 mark)

**Total: 2 marks**

---

## Section 2: Adapted Examination Questions

### Question 3 (Adapted from Jan23 Q3(a)(i)) | 3 marks | LO3.1

**Scenario:** A manufacturing project has been planned with the following activities:

| Activity | Description | Duration (weeks) | Depends on |
|----------|-------------|------------------|------------|
| P | Design product | 5 | - |
| Q | Order materials | 3 | P |
| R | Set up production line | 4 | P |
| S | Trial production run | 2 | Q, R |
| T | Full production | 6 | S |

The partially completed Gantt chart below shows some of the activities:

```
Week:     0    2    4    6    8    10   12   14   16   18   20
          |    |    |    |    |    |    |    |    |    |    |
P         [=====]
Q              [===]
R              
S                        [==]
T                            [======]

Legend: [===] = Activity time    ■■■ = Slack time
```

**Required:**

**(a)** Complete the bar for Activity R on the chart above. (1 mark)

**(b)** Activity Q has slack time. Show this slack time on the chart using the ■■■ symbol. (1 mark)

**(c)** Draw a dependency arrow from Activity Q to Activity S. (1 mark)

**Total: 3 marks**

---

### Question 4 (Adapted from Jun24 Q3(a)) | 6 marks | LO3.1

**Scenario:** A project manager is using a Gantt chart to plan a laboratory refurbishment project. The chart shows various activities including equipment installation, safety testing, and staff training.

**Required:**

Explain **one advantage** to the project manager of identifying each of the following on a Gantt chart:

**(a)** Concurrent activities (activities that can be performed simultaneously) (2 marks)

**(b)** Critical activities (activities with zero slack time) (2 marks)

**(c)** Activities with slack time (2 marks)

**Helpful Hint:** For full marks, explain the benefit specifically to project management decision-making, not just what the term means.

**Total: 6 marks**

---

## Section 3: New Practice Questions

### Question 5 | 4 marks | LO3.1

**Scenario:** A civil engineering firm is planning a bridge inspection project. The project comprises the following activities:

| Activity | Description | Duration (days) | Earliest Finish | Latest Finish |
|----------|-------------|-----------------|----------------|---------------|
| A | Site access setup | 2 | 2 | 2 |
| B | Visual inspection | 3 | 5 | 6 |
| C | Structural testing | 5 | 10 | 10 |
| D | Report writing | 3 | 13 | 13 |

**Required:**

**(a)** Calculate the slack time for Activity B. Show your working. (2 marks)

**(b)** Identify which activities are on the critical path. (1 mark)

**(c)** The project manager wants to reduce the overall project duration by 2 days. Explain why reducing the duration of Activity B would **not** achieve this objective. (1 mark)

**Helpful Hint:** Think about the relationship between slack time and the critical path.

**Total: 4 marks**

---

### Question 6 | 5 marks | LO3.1

**Scenario:** An automotive component manufacturer is planning a production line upgrade. The original Gantt chart showed that Activities K, L, M, and N would complete in 14 weeks. However, Activity M has been delayed by 3 weeks due to supplier issues.

**Original activity data:**

| Activity | Duration (weeks) | Slack Time |
|----------|------------------|------------|
| K | 4 | 0 |
| L | 5 | 2 |
| M | 6 | 0 |
| N | 3 | 0 |

Critical Path: K → M → N (total 13 weeks)  
Activity L runs concurrent with K and M

**Required:**

**(a)** Calculate the new project completion time following the 3-week delay to Activity M. Show your working. (2 marks)

**(b)** Explain whether the delay to Activity M will affect Activity L. (2 marks)

**(c)** State **one** action the project manager could take to reduce the impact of this delay. (1 mark)

**Total: 5 marks**

---

### Question 7 | 6 marks | LO3.1

**Scenario:** A pharmaceutical company is developing a new drug manufacturing process. The project includes regulatory approval, equipment installation, and staff training. The project manager has identified the following situation:

```
Month:    0    2    4    6    8    10   12   14   16
          |    |    |    |    |    |    |    |    |
Activity X   [====]                                 (4 months, critical)
Activity Y        [=====]                           (5 months, critical)
Activity Z             [=]■■■■                      (1 month + 4 months slack)
Activity W                     [=======]            (7 months, critical)

Key: [===] = Planned activity time    ■■■ = Slack time
```

The company has just received notice that regulatory approval (Activity Y) will now take **9 months** instead of the planned 5 months – a delay of 4 months.

**Required:**

**(a)** Calculate the new project completion time. Show your working. (2 marks)

**(b)** The project manager proposes to **fast-track** the project by starting Activity W immediately when Activity Y starts, rather than waiting for Activity Y to finish. 

Explain **one advantage** and **one disadvantage** of this fast-tracking approach. (4 marks)

**Helpful Hint:** Fast-tracking means performing activities in parallel that were originally planned in sequence. Consider both the time benefits and the risks.

**Total: 6 marks**

---

## Summary of Questions

| Question | Marks | Topic | Source |
|----------|-------|-------|--------|
| Q1 | 6 | Complete Gantt chart with dependencies | Past exam (Jan24) |
| Q2 | 2 | Identify critical activities | Past exam (Jun23) |
| Q3 | 3 | Complete Gantt chart, show slack | Adapted |
| Q4 | 6 | Explain advantages of Gantt features | Adapted |
| Q5 | 4 | Calculate slack, identify critical path | New |
| Q6 | 5 | Calculate delay impact | New |
| Q7 | 6 | Fast-tracking analysis | New |
| **Total** | **32 marks** | | |

---

## Technical Glossary

**Concurrent Activities** – Activities that can be performed at the same time (simultaneously)

**Critical Activity** – An activity with zero slack time; any delay will cause project delay

**Critical Path** – The sequence of critical activities from project start to finish; the longest path through the network

**Dependency** – A logical relationship where one activity must finish before another can start

**Duration** – The length of time required to complete an activity

**Fast-tracking** – Starting activities in parallel that were originally planned in sequence, to reduce overall project time

**Gantt Chart** – A horizontal bar chart showing activities on a timeline, with bars representing activity duration

**Slack Time** (also called Float Time or Total Float) – The amount of time an activity can be delayed without delaying the project; calculated as Latest Finish - Earliest Finish

**Predecessor Activity** – An activity that must be completed before another activity can start

**Successor Activity** – An activity that cannot start until a predecessor activity is complete

---

## Helpful Examination Tips

### Time Management
- Read the entire question before starting
- For multi-mark questions, allocate approximately 1-1.5 minutes per mark
- If stuck, move on and return later

### Common Mistakes to Avoid

❌ **Mistake 1:** Forgetting to check dependencies before drawing activities  
✅ **Solution:** Always read the "Depends on" column carefully

❌ **Mistake 2:** Confusing slack time with activity duration  
✅ **Solution:** Slack time is the *gap* between finish and next activity start

❌ **Mistake 3:** Stating "critical activities are important"  
✅ **Solution:** Critical activities are those with *zero slack*; all activities are important

❌ **Mistake 4:** Calculating slack as EF - Duration  
✅ **Solution:** Slack = LF - EF or Slack = LS - ES

❌ **Mistake 5:** Drawing activity bars without using a ruler  
✅ **Solution:** Use a ruler for neat, accurate charts that are easy to mark

### Answering Explanation Questions

For questions asking you to "explain":

**Poor answer:** "Critical activities have no slack."  
(This defines rather than explains)

**Good answer:** "Identifying critical activities allows the project manager to prioritise resources towards activities that directly affect project completion, ensuring the project finishes on time."  
(This explains the practical benefit)

### Calculation Questions

Always show your working:

**Poor presentation:**
Answer: 3 weeks

**Good presentation:**
Slack Time = Latest Finish - Earliest Finish  
Slack Time = 8 - 5  
Slack Time = **3 weeks**

Even if your final answer is incorrect, you can earn partial marks for correct method.

---

## Learning Outcomes Checklist

After completing these workshop questions, you should be able to:

- [ ] Complete a Gantt chart accurately showing dependent activities
- [ ] Calculate slack time using the formula: Slack = LF - EF
- [ ] Identify critical activities (those with zero slack)
- [ ] Explain the practical significance of concurrent activities
- [ ] Analyse the impact of delays on project completion time
- [ ] Evaluate schedule compression strategies (fast-tracking)
- [ ] Show slack time visually on a Gantt chart
- [ ] Draw dependency relationships between activities

If you struggle with any checklist item, review the relevant section in the lecture notes and attempt the practice questions again.

---

## Additional Practice Resources

**Past Examination Papers (available from your tutor):**
- January 2022, Question 3(a)
- January 2023, Questions 3(a)(i) and 3(a)(ii)
- June 2023, Questions 3(b), 3(c)(i), 3(c)(ii), 3(c)(iii)
- January 2024, Question 2(b)(i)
- June 2024, Question 3(a)

**Recommended Review:**
- Week 11 lecture notes (Gantt Charts Fundamentals)
- Unit specification, LO3.1 assessment criteria
- Practice calculating slack time for 10 different activities

**Online Resources:**
- OCR Cambridge TECHNICALS Engineering support materials
- ProjectLibre software (free download for Gantt chart practice)
- PMI (Project Management Institute) knowledge base

---

## Document Information

**Course:** Cambridge TECHNICALS Level 3 Engineering  
**Unit:** 24 – Project Management for Engineers  
**Week:** 12 of 32  
**Workshop Duration:** 30 minutes  
**Total Marks Available:** 32 marks  
**Learning Outcome:** LO3.1  
**Assessment Focus:** Gantt chart completion, slack time calculation, critical path identification, delay analysis

**Solutions Document:** See separate "Week12_Workshop_Solutions.md" file

---
