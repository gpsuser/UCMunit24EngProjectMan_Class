# Week 11: Gantt Charts Fundamentals
## Cambridge TECHNICALS Level 3 Engineering
### Unit 24: Project Management for Engineers

---
<!-- _footer: 'Slide 1' -->

# Table of Contents

| Section/Topic | Time | Learning Outcome |
|---------------|------|------------------|
| Introduction | 5 min | LO3.1 |
| What is a Gantt Chart? | 10 min | LO3.1 |
| Chart Components and Structure | 10 min | LO3.1 |
| Activity Sequencing and Dependencies | 12 min | LO3.1 |
| Concurrent Activities and Duration | 8 min | LO3.1 |
| Critical Activities and Slack Time | 10 min | LO3.1 |
| Delays and Adjustments | 5 min | LO3.1 |
| Conclusion | 5 min | LO3.1 |

---
<!-- _footer: 'Slide 2' -->

# Learning Outcomes

By the end of this session, learners will be able to:

1. Define what a Gantt chart is and explain its purpose
2. Identify and describe key components and structure
3. Distinguish between sequential, concurrent, and dependent activities
4. Calculate minimum completion time for a project
5. Identify critical activities and calculate slack time
6. Interpret Gantt chart data to make project management decisions
7. Understand how delays and adjustments affect project scheduling

---
<!-- _footer: 'Slide 3' -->

# Objectives

- Understand the fundamental purpose of Gantt charts in engineering project management
- Master the interpretation of Gantt chart components
- Apply activity sequencing principles to project scheduling
- Analyse critical paths and slack time for project control
- Evaluate the impact of delays on project timelines

---
<!-- _footer: 'Slide 4' -->

# Introduction

**Why Gantt Charts Matter in Engineering**

- Essential tool for coordinating multiple activities in engineering projects
- Used in major UK projects: Crossrail, Heathrow Terminal 5, Thames Tideway Tunnel
- Foundation for advanced techniques (CPA, PERT)
- Developed by Henry Gantt in early 1900s
- Remains the global standard for project scheduling

*"Understanding this fundamental tool is essential for any engineer involved in project delivery"*

---
<!-- _footer: 'Slide 5' -->

# What is a Gantt Chart?

**Definition**

A horizontal bar chart that illustrates a project schedule, showing the start and finish dates of individual activities or tasks.

**Key Characteristic**

- Each activity represented by a bar positioned along a timeline
- Bar length corresponds to activity duration
- Visual representation of project timeline

---
<!-- _footer: 'Slide 6' -->

# Key Functions of Gantt Charts

1. **Visual representation** of project timeline
2. **Activity tracking** to monitor progress
3. **Resource allocation** planning
4. **Communication tool** for stakeholders
5. **Dependency management** showing activity relationships

---
<!-- _footer: 'Slide 7' -->

# Advantages of Gantt Charts

**Simplicity**
- Easy to understand for technical and non-technical stakeholders

**Flexibility**
- Quick updates as project circumstances change

**Clarity**
- Immediate visual insight into project status

**Planning Efficiency** - Identifies resource conflicts and scheduling issues early

**Accountability** - Clearly assigns activities to specific timeframes

---
<!-- _footer: 'Slide 8' -->

# Limitations of Gantt Charts

**Complexity Management**
- Large projects with hundreds of activities become difficult to represent

**Dependency Detail**
- Complex inter-activity relationships may not be immediately obvious

**Resource Constraints**
- Does not explicitly show resource availability or conflicts

**Critical Path Identification**
- Requires additional analysis to determine critical activities

*These limitations led to development of CPA and PERT (Weeks 13-15)*

---
<!-- _footer: 'Slide 9' -->

# Chart Components and Structure

**Essential Elements**

```
Simple Gantt Chart Structure:

Activity List     Timeline (weeks)
                  0   1   2   3   4   5   6   7   8
Activity A        [======]
Activity B            [==========]
Activity C                    [======]
Activity D                        [==========]

Legend:
[====]  = Activity duration (activity time)
[////]  = Slack time
```

---
<!-- _footer: 'Slide 10' -->

# Activity List

**Vertical Axis Components**

Activities should be:

- **Clearly labelled** with descriptive names
- **Uniquely identified** using letters or numbers
- **Appropriately sized** - not too broad or too granular
- **Measurable** with defined completion criteria

---
<!-- _footer: 'Slide 11' -->

# Timeline

**Horizontal Axis Components**

Project duration scaled appropriately:

- **Hours** - very short projects or detailed phases
- **Days** - small to medium engineering projects
- **Weeks** - medium-sized projects lasting months
- **Months** - large-scale infrastructure projects

---
<!-- _footer: 'Slide 12' -->

# Activity Bars

**Bar Positioning**

Each horizontal bar represents:

1. **Start time** - when the activity begins
2. **Duration** - how long the activity takes (bar length)
3. **Finish time** - when the activity is scheduled to complete

**Visual Conventions**
- Solid bars: actual activity duration
- Hatched/shaded bars: slack time (float)
- Dependency arrows: relationships between activities
- Milestone markers: key project events

---
<!-- _footer: 'Slide 13' -->

# Reading a Gantt Chart

**Five-Step Process**

1. Identify the activity on the vertical axis
2. Trace horizontally to determine start and finish times
3. Observe bar positioning to understand dependencies
4. Note any slack time shown through different shading
5. Calculate durations by measuring bar length against timeline

---
<!-- _footer: 'Slide 14' -->

# Activity Sequencing and Dependencies

**Three Types of Activity Relationships**

1. **Sequential (Dependent) Activities**
   - Must occur in specific order
   - "Finish-to-Start" dependency

2. **Concurrent (Parallel) Activities**
   - Can occur simultaneously
   - No dependency between them

3. **Partially Dependent Activities**
   - One can begin before predecessor completes

---
<!-- _footer: 'Slide 15' -->

# Sequential Activities Example

**Engineering Example: Automotive Component Design**

```
         0   1   2   3   4   5   6   7   8
Activity A [====]
Activity B         [======]
                   ^
            Finish-to-Start
            Dependency
```

- Activity A: Complete stress analysis (2 weeks)
- Activity B: Design component based on analysis (3 weeks)
- Total time: 5 weeks minimum
- Activity B cannot begin until Activity A finishes

---
<!-- _footer: 'Slide 16' -->

# Concurrent Activities Example

**Engineering Example: Building Construction**

```
         0   1   2   3   4   5   6   7   8
Activity C [========]
Activity D [========]
```

- Activity C: Install electrical systems (4 weeks)
- Activity D: Install plumbing systems (4 weeks)
- Both proceed simultaneously if resources available
- Total time: 4 weeks (not 8 weeks)

---
<!-- _footer: 'Slide 17' -->

# Impact on Project Duration

**Duration Calculations**

- **Sequential activities**: Durations add together
  - Example: 2 weeks + 3 weeks = 5 weeks total

- **Concurrent activities**: Only longest duration counts
  - Example: max(4 weeks, 4 weeks) = 4 weeks total

- **Partially dependent**: Overlap reduces total time

*Understanding these relationships enables schedule compression*

---
<!-- _footer: 'Slide 18' -->

# Concurrent Activities and Duration

**Benefits of Concurrency**

1. **Reduced project duration** - activities shorten critical path
2. **Resource optimisation** - different teams work separately
3. **Risk distribution** - multiple activities reduce delay impact
4. **Cost efficiency** - shorter duration reduces overhead costs

---
<!-- _footer: 'Slide 19' -->

# Duration Calculation Example

**Time Savings from Concurrency**

```
Scenario 1 - Sequential:
Foundation excavation (3 weeks) + Steel frame fabrication (4 weeks)
Total: 7 weeks

Scenario 2 - Concurrent:
Foundation excavation (3 weeks) || Steel frame fabrication (4 weeks)
Total: max(3, 4) = 4 weeks

Time saved: 3 weeks (43% reduction)
```

---
<!-- _footer: 'Slide 20' -->

# Practical Constraints on Concurrency

**Limitations to Consider**

- **Resource availability** - limited personnel, equipment, or budget
- **Physical constraints** - site access limitations or workspace conflicts
- **Technical risks** - parallel development may require rework
- **Management capacity** - overseeing multiple activities increases complexity

---
<!-- _footer: 'Slide 21' -->

# Critical Activities

**Definition**

Critical activities are those that, if delayed, will directly delay the entire project completion date.

**Characteristics**

1. **Zero slack time** - no flexibility in scheduling
2. **Sequential dependencies** - usually part of activity chain
3. **Direct impact** - any delay immediately affects completion
4. **Management priority** - require closest monitoring

---
<!-- _footer: 'Slide 22' -->

# Identifying Critical Activities

**Critical Path Example**

```
         0   1   2   3   4   5   6   7   8   9   10
Activity A [==]                              Critical
Activity B     [====]                        Critical  
Activity C     [==]////                      Non-critical
Activity D         [======]                  Critical
Activity E                 [==]              Critical

Critical Path: A → B → D → E
Minimum Completion Time: 2 + 4 + 6 + 2 = 14 weeks
```

Activity C has slack time and is not critical

---
<!-- _footer: 'Slide 23' -->

# Slack Time (Float)

**Definition**

The amount of time an activity can be delayed without affecting the project completion date.

**Formula**

```
Slack Time = Latest Finish Time (LFT) - Earliest Finish Time (EFT)

Or:

Slack Time = Latest Start Time - Earliest Start Time
```

---
<!-- _footer: 'Slide 24' -->

# Types of Slack

**Free Float**
- Time an activity can be delayed without delaying the start of any subsequent activity

**Total Float**
- Time an activity can be delayed without delaying overall project completion

---
<!-- _footer: 'Slide 25' -->

# Slack Time Calculation Example

**Worked Example**

```
Activity J: Install ventilation system
- Earliest Start Time: Week 3
- Duration: 2 weeks
- Earliest Finish Time: Week 5
- Latest Finish Time: Week 7

Slack Time = 7 - 5 = 2 weeks
```

**Interpretation**: Activity J can be delayed by up to 2 weeks without impacting project completion date

---
<!-- _footer: 'Slide 26' -->

# Visual Representation of Slack

**Gantt Chart Notation**

```
         0   1   2   3   4   5   6   7   8
Activity K [====]////
           ^    ^^  ^
         EST  EFT LST

Where:
[====] = Activity duration
[////] = Slack time
EST = Earliest Start Time
EFT = Earliest Finish Time  
LST = Latest Start Time
```

---
<!-- _footer: 'Slide 27' -->

# Management Implications

**Using Critical Path and Slack Information**

1. **Prioritise resources** - focus on critical activities
2. **Manage risks** - identify where delays are most damaging
3. **Optimise schedules** - reschedule non-critical activities to address conflicts
4. **Communicate effectively** - explain which activities need urgent attention

---
<!-- _footer: 'Slide 28' -->

# Delays and Adjustments

**Impact of Delays**

**Critical Activities**
- Any delay directly extends project completion by same amount
- Requires corrective action

**Non-Critical Activities**
- Delays absorbed by slack time (up to float available)
- Once slack exhausted, activity becomes critical

---
<!-- _footer: 'Slide 29' -->

# Schedule Adjustment Techniques

**Five Key Methods**

1. **Activity duration changes** - update bars for revised estimates
2. **Dependency modifications** - alter relationships if requirements change
3. **Resource reallocation** - move resources from non-critical to critical activities
4. **Parallel scheduling** - convert sequential to concurrent where feasible
5. **Milestone adjustment** - reschedule key project milestones

---
<!-- _footer: 'Slide 30' -->

# Monitoring and Control

**Effective Gantt Chart Monitoring Requires**

- **Regular updates** - weekly or bi-weekly progress reviews
- **Variance analysis** - comparing actual vs planned timelines
- **Trend identification** - spotting patterns in delays or early completions
- **Corrective action** - implementing schedule recovery measures promptly

---
<!-- _footer: 'Slide 31' -->

# Conclusion

**Key Concepts to Remember**

1. **Gantt charts** provide visual representation of project schedules
2. **Sequential activities** must follow one after another; concurrent activities run simultaneously
3. **Critical activities** have zero slack and directly impact completion dates
4. **Slack time** provides scheduling flexibility for non-critical activities
5. **Dependencies** define relationships and constrain scheduling options
6. **Minimum completion time** calculated by summing durations along critical path

---
<!-- _footer: 'Slide 32' -->

# Real-World Application

**Industry Usage**

Major UK engineering organisations require engineers to demonstrate competency in Gantt chart interpretation:

- Arup
- Balfour Beatty
- BAE Systems

*This fundamental skill opens pathways to project leadership positions across the engineering sector*

---
<!-- _footer: 'Slide 33' -->

# Next Week Preview

**Week 12: Gantt Chart Practice**

- Creating Gantt charts using project management software
- Slack time analysis techniques
- Resource levelling on Gantt charts
- Schedule compression methods (crashing and fast-tracking)
- Handling delays and adjustments in complex projects

**Preparation**: Review this week's content and ensure understanding of basic concepts

---
<!-- _footer: 'Slide 34' -->

# Summary

**What We Covered Today**

- Definition and purpose of Gantt charts
- Components and structure of Gantt charts
- Activity sequencing: sequential, concurrent, and dependent
- Critical activities and critical path
- Slack time calculation and interpretation
- Impact of delays and schedule adjustments

**Remember**: Gantt charts are foundational to understanding CPA and PERT techniques in upcoming weeks