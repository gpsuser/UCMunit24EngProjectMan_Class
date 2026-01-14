# Week 11: Gantt Charts Fundamentals

## Cambridge TECHNICALS Level 3 Engineering
### Unit 24: Project Management for Engineers

**Delivery Week:** 11 of 32  
**Session Duration:** 90 minutes (55 min lecture + 5 min break + 30 min workshop)  
**Learning Outcome:** LO3.1 - How to use and interpret a Gantt chart  
**Date:** 26 November 2025

---

## Table of Contents

| Section/Topic | Time Allocation | Learning Outcome |
|---------------|----------------|------------------|
| Introduction & Learning Objectives | 5 minutes | LO3.1 |
| What is a Gantt Chart? | 10 minutes | LO3.1 |
| Chart Components and Structure | 10 minutes | LO3.1 |
| Activity Sequencing and Dependencies | 12 minutes | LO3.1 |
| Concurrent Activities and Duration | 8 minutes | LO3.1 |
| Critical Activities and Slack Time | 10 minutes | LO3.1 |
| Conclusion and Key Takeaways | 5 minutes | LO3.1 |
| **Break** | **5 minutes** | - |
| Workshop Activities | 30 minutes | LO3.1 |
| **Total** | **90 minutes** | |

---

## Learning Objectives

By the end of this session, learners will be able to:

1. Define what a Gantt chart is and explain its purpose in engineering project management
2. Identify and describe the key components and structure of a Gantt chart
3. Distinguish between sequential, concurrent, and dependent activities
4. Calculate minimum completion time for a project
5. Identify critical activities and calculate slack time
6. Interpret Gantt chart data to make project management decisions
7. Understand how delays and adjustments affect project scheduling

---

## Introduction (5 minutes)

Engineering projects, whether developing a new automotive component, constructing a bridge, or implementing a manufacturing process improvement, require careful scheduling and coordination of multiple activities. The Gantt chart, developed by Henry Gantt in the early 1900s, remains one of the most widely used project management tools in engineering organisations worldwide (Lock, 2020).

This week marks the beginning of Phase 3 of the unit, focusing on project management tools. The Gantt chart serves as the foundation for understanding more advanced techniques such as Critical Path Analysis (CPA) and Programme Evaluation and Review Technique (PERT), which will be covered in subsequent weeks.

Major UK engineering projects such as Crossrail (Elizabeth Line), Heathrow Terminal 5 expansion, and the Thames Tideway Tunnel all utilised sophisticated Gantt charts to coordinate thousands of activities across multiple years (National Audit Office, 2018). Understanding this fundamental tool is essential for any engineer involved in project delivery.

---

## What is a Gantt Chart? (10 minutes)

### Definition and Purpose

A Gantt chart is a horizontal bar chart that illustrates a project schedule, showing the start and finish dates of individual activities or tasks. Each activity is represented by a bar positioned along a timeline, with the length of the bar corresponding to the activity's duration (Project Management Institute, 2017).

### Key Functions

Gantt charts serve several critical functions in engineering project management:

1. **Visual representation** of the project timeline, making complex schedules easily understandable
2. **Activity tracking** to monitor progress against planned schedules
3. **Resource allocation** planning by identifying when specific resources are required
4. **Communication tool** for stakeholders, providing clear visibility of project status
5. **Dependency management** showing how activities relate to and depend upon each other

### Historical Context

Henry Laurence Gantt, an American mechanical engineer, developed the Gantt chart between 1910 and 1915. Initially used for manufacturing and construction projects, the tool gained widespread adoption during World War I for planning military operations (Wilson, 2003). Today, Gantt charts are integrated into virtually all project management software packages and remain the standard for project scheduling across industries.

### Advantages of Gantt Charts

Research by the Association for Project Management identifies several key advantages (APM, 2019):

- **Simplicity**: Easy to understand for both technical and non-technical stakeholders
- **Flexibility**: Can be updated quickly as project circumstances change
- **Clarity**: Provides immediate visual insight into project status and progress
- **Planning efficiency**: Helps identify resource conflicts and scheduling issues early
- **Accountability**: Clearly assigns activities to specific timeframes

### Limitations of Gantt Charts

Despite their widespread use, Gantt charts have limitations that engineers must recognise:

- **Complexity management**: Large projects with hundreds of activities become difficult to represent clearly
- **Dependency detail**: Complex inter-activity relationships may not be immediately obvious
- **Resource constraints**: Does not explicitly show resource availability or conflicts
- **Critical path identification**: Requires additional analysis to determine which activities are critical

These limitations led to the development of complementary tools such as CPA and PERT, which will be explored in Weeks 13-15.

---

## Chart Components and Structure (10 minutes)

### Essential Elements

A properly constructed Gantt chart contains several standard components (Burke, 2013):

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

### Activity List

The vertical axis lists all project activities, typically organised in logical sequence. Activities should be:

- **Clearly labelled** with descriptive names
- **Uniquely identified** using letters or numbers
- **Appropriately sized** - not too broad or too granular
- **Measurable** with defined completion criteria

### Timeline

The horizontal axis represents the project duration, scaled appropriately to the project length. Timescales might be:

- Hours (for very short projects or detailed phases)
- Days (typical for small to medium engineering projects)
- Weeks (common for medium-sized projects lasting months)
- Months (appropriate for large-scale infrastructure projects)

### Activity Bars

Each horizontal bar represents an individual activity, positioned according to:

- **Start time**: When the activity begins
- **Duration**: How long the activity takes (bar length)
- **Finish time**: When the activity is scheduled to complete

### Visual Conventions

Standard visual representations include (Lock, 2020):

- **Solid bars**: Represent actual activity duration
- **Hatched/shaded bars**: Indicate slack time (float)
- **Dependency arrows**: Show relationships between activities
- **Milestone markers**: Diamonds or symbols for key project events
- **Progress indicators**: Shading or colour to show completion status

### Reading a Gantt Chart

To interpret a Gantt chart effectively:

1. Identify the activity in question on the vertical axis
2. Trace horizontally to determine start and finish times
3. Observe bar positioning to understand dependencies
4. Note any slack time shown through different shading
5. Calculate durations by measuring bar length against the timeline

---

## Activity Sequencing and Dependencies (12 minutes)

### Types of Activity Relationships

Activities in engineering projects relate to each other in specific ways. Understanding these relationships is crucial for accurate scheduling (Project Management Institute, 2017).

#### Sequential (Dependent) Activities

Sequential activities must occur in a specific order, where one activity cannot begin until its predecessor is complete. The relationship is termed "Finish-to-Start" dependency.

**Engineering Example**: In automotive component design:
- Activity A: Complete stress analysis calculations (Duration: 2 weeks)
- Activity B: Design component based on analysis results (Duration: 3 weeks)

Activity B cannot begin until Activity A finishes. The total time required is 5 weeks minimum.

```
Sequential Activities Example:

         0   1   2   3   4   5   6   7   8
Activity A [====]
Activity B         [======]
                   ^
            Finish-to-Start
            Dependency
```

#### Concurrent (Parallel) Activities

Concurrent activities can occur simultaneously, with no dependency between them. These represent significant opportunities for reducing overall project duration (Burke, 2013).

**Engineering Example**: In building construction:
- Activity C: Install electrical systems (Duration: 4 weeks)
- Activity D: Install plumbing systems (Duration: 4 weeks)

Both can proceed simultaneously if resources are available.

```
Concurrent Activities Example:

         0   1   2   3   4   5   6   7   8
Activity C [========]
Activity D [========]
```

#### Partially Dependent Activities

Some activities may have partial dependencies, where one activity can begin before its predecessor completes, but cannot finish until the predecessor is done.

**Engineering Example**: In software development:
- Activity E: Develop software module (Duration: 6 weeks)
- Activity F: Conduct integration testing (Duration: 2 weeks, can start week 5)

Activity F can begin in week 5, one week before Activity E completes, allowing for early identification of integration issues.

### Dependency Notation

Dependencies are typically shown using arrows connecting the end of one activity bar to the start of another. The arrow direction indicates the sequence: predecessor → successor (Lock, 2020).

### Impact on Project Duration

The relationship between activities directly affects minimum project completion time:

- **Sequential activities**: Durations add together
- **Concurrent activities**: Only the longest duration counts toward total time
- **Partially dependent**: Overlap reduces total time

Understanding these relationships enables project managers to identify opportunities for **fast-tracking** (running activities in parallel that would normally be sequential) or **schedule compression** (reducing activity durations).

### Dependency Errors

Common errors in dependency identification include:

- **Missing dependencies**: Showing activities as concurrent when they must be sequential
- **Unnecessary dependencies**: Forcing sequential completion when concurrent execution is possible
- **Incorrect dependency direction**: Reversing the predecessor-successor relationship
- **Circular dependencies**: Creating impossible loops where Activity A depends on Activity B, which depends on Activity A

### Case Study: Thames Tideway Tunnel

The Thames Tideway Tunnel project, a major London infrastructure development, demonstrates complex dependency management. The project required coordination of:

- Site investigations (must complete before design finalisation)
- Tunnel boring machine procurement (concurrent with detailed design)
- Shaft construction (must complete before tunnelling begins)
- Tunnelling operations (sequential progression along the route)
- Secondary lining installation (follows primary tunnel completion)

The Gantt chart for this £4.2 billion project contained over 5,000 activities with intricate dependency relationships (Thames Water, 2019).

---

## Concurrent Activities and Duration (8 minutes)

### Definition and Identification

Concurrent activities are those that can be performed simultaneously, without dependency constraints. Identifying opportunities for concurrency is a key project management skill that can significantly reduce overall project duration (Association for Project Management, 2019).

### Benefits of Concurrent Activities

Properly identified concurrent activities offer several advantages:

1. **Reduced project duration**: Activities occurring simultaneously shorten the critical path
2. **Resource optimisation**: Different teams can work on separate activities concurrently
3. **Risk distribution**: Multiple activities progressing reduces impact if one encounters delays
4. **Cost efficiency**: Shorter overall duration typically reduces overhead costs

### Identifying Concurrent Opportunities

To identify potential concurrent activities, engineers should ask:

- Do these activities require the same physical resources or workspace?
- Does one activity's output provide input for the other?
- Are the activities technically independent?
- Are sufficient resources available to support both activities?

### Duration Calculation with Concurrent Activities

When activities run concurrently, the project duration is determined by the **longest activity**, not the sum of durations.

**Example Calculation**:

```
Scenario 1 - Sequential Activities:
Activity G: Foundation excavation (3 weeks)
Activity H: Steel frame fabrication (4 weeks)
Arranged sequentially: 3 + 4 = 7 weeks total

Scenario 2 - Concurrent Activities:
Activity G: Foundation excavation (3 weeks)
Activity H: Steel frame fabrication (4 weeks)
Arranged concurrently: max(3, 4) = 4 weeks total

Time saved: 7 - 4 = 3 weeks (43% reduction)
```

### Practical Constraints

While concurrency offers benefits, several practical constraints must be considered:

- **Resource availability**: Limited personnel, equipment, or budget may prevent true concurrency
- **Physical constraints**: Site access limitations or workspace conflicts
- **Technical risks**: Parallel development may require rework if technical issues emerge
- **Management capacity**: Overseeing multiple concurrent activities increases complexity

### Engineering Application Example

In the development of Crossrail's rolling stock:

- **Concurrent Activity 1**: Design of train exterior (12 months)
- **Concurrent Activity 2**: Design of passenger information systems (10 months)
- **Concurrent Activity 3**: Design of traction power systems (14 months)

These three activities proceeded concurrently, with the project duration determined by the longest activity (14 months). Had they been sequential, the total duration would have been 36 months (Crossrail, 2017).

---

## Critical Activities and Slack Time (10 minutes)

### Critical Activities

Critical activities are those that, if delayed, will directly delay the entire project completion date. They form the **critical path** through the project schedule - the longest sequence of dependent activities from project start to finish (Project Management Institute, 2017).

#### Characteristics of Critical Activities

Critical activities share several defining features:

1. **Zero slack time**: No flexibility in scheduling
2. **Sequential dependencies**: Usually part of a chain of dependent activities
3. **Direct impact**: Any delay immediately affects project completion
4. **Management priority**: Require closest monitoring and control

#### Identifying Critical Activities

To identify critical activities on a Gantt chart:

1. Calculate the minimum project completion time
2. Trace the longest path from start to finish
3. Identify activities that, if delayed, would extend this path
4. Confirm that these activities have no scheduling flexibility

#### Example of Critical Path

```
Project Activities:

         0   1   2   3   4   5   6   7   8   9   10
Activity A [==]                              Critical
Activity B     [====]                        Critical  
Activity C     [==]////                      Non-critical
Activity D         [======]                  Critical
Activity E                 [==]              Critical

Critical Path: A → B → D → E
Minimum Completion Time: 2 + 4 + 6 + 2 = 14 weeks

Activity C has slack time and is not critical
```

### Slack Time (Float)

Slack time, also called float, represents the amount of time an activity can be delayed without affecting the project completion date. It is the difference between the latest time an activity can finish and the earliest time it can finish (Lock, 2020).

#### Formula for Slack Time

```
Slack Time = Latest Finish Time (LFT) - Earliest Finish Time (EFT)

Or alternatively:

Slack Time = (Latest Start Time - Earliest Start Time)
```

#### Types of Slack

**Free Float**: The amount of time an activity can be delayed without delaying the start of any subsequent activity.

**Total Float**: The amount of time an activity can be delayed without delaying the overall project completion.

#### Calculating Slack: Worked Example

```
Activity J: Install ventilation system
- Earliest Start Time: Week 3
- Duration: 2 weeks
- Earliest Finish Time: Week 5
- Latest Finish Time: Week 7 (dictated by subsequent activities)

Slack Time = 7 - 5 = 2 weeks

Interpretation: Activity J can be delayed by up to 2 weeks without 
impacting the project completion date.
```

### Visual Representation of Slack

On a Gantt chart, slack time is typically shown as:

- Hatched bars extending from the activity end to the latest finish time
- Different coloured shading (e.g., lighter shade)
- Separate bars following the activity bar

```
Activity with Slack Time:

         0   1   2   3   4   5   6   7   8
Activity K [====]////
           ^    ^^  ^
         EST  EFT LST

Where:
[====] = Activity duration
[////] = Slack time
EST = Earliest Start Time
EFT = Earliest Finish Time  
LST = Latest Start Time (without delaying project)
```

### Management Implications

Understanding critical activities and slack time enables project managers to:

1. **Prioritise resources**: Focus limited resources on critical activities
2. **Manage risks**: Identify where delays would be most damaging
3. **Optimise schedules**: Reschedule non-critical activities to address resource conflicts
4. **Communicate effectively**: Explain to stakeholders which activities require urgent attention

### Case Study: Heathrow Terminal 5

The construction of Heathrow Terminal 5, completed in 2008, demonstrates effective critical path management. The project team identified that:

- **Critical activities**: Foundation piling, structural steel erection, roof installation
- **Non-critical activities**: Interior finishes in some areas, landscaping, minor access roads

By focusing intensive resources and monitoring on critical activities, whilst allowing flexibility in non-critical work, the project achieved substantial completion on schedule despite its complexity (Brady and Davies, 2010).

---

## Delays and Adjustments (5 minutes)

### Impact of Delays

Delays to activities affect the project in different ways depending on whether the activity is critical or has slack time:

#### Delays to Critical Activities

Any delay to a critical activity directly extends the project completion date by the same amount, unless corrective action is taken.

**Example**: If Activity A on the critical path is delayed by 2 weeks, the entire project is delayed by 2 weeks, unless:
- Another critical activity is shortened (crashing)
- Activities are rearranged to create concurrency (fast-tracking)
- Resources are reallocated to accelerate other critical activities

#### Delays to Non-Critical Activities

Delays to non-critical activities may be absorbed by slack time, up to the amount of float available. Once slack is exhausted, the activity becomes critical.

**Example**: Activity B has 3 weeks of slack. A 2-week delay is absorbed without project impact. A 4-week delay would make Activity B critical and extend the project by 1 week.

### Schedule Adjustments

Project managers can adjust Gantt charts to accommodate changes through several techniques (Burke, 2013):

1. **Activity duration changes**: Updating bars to reflect revised time estimates
2. **Dependency modifications**: Altering activity relationships if technical requirements change
3. **Resource reallocation**: Moving resources from non-critical to critical activities
4. **Parallel scheduling**: Converting sequential activities to concurrent where feasible
5. **Milestone adjustment**: Rescheduling key project milestones based on actual progress

### Monitoring and Control

Effective use of Gantt charts for monitoring requires:

- **Regular updates**: Weekly or bi-weekly progress reviews
- **Variance analysis**: Comparing actual vs planned timelines
- **Trend identification**: Spotting patterns in delays or early completions
- **Corrective action**: Implementing schedule recovery measures promptly

---

## Conclusion and Key Takeaways (5 minutes)

### Summary

This session introduced Gantt charts, the foundational project management tool used across all engineering disciplines. Understanding Gantt charts is essential for:

- Planning project activities and their sequencing
- Communicating schedules to stakeholders
- Monitoring project progress
- Identifying critical activities requiring priority management
- Calculating minimum project completion times

### Key Concepts to Remember

1. **Gantt charts** provide visual representation of project schedules using horizontal bars positioned along a timeline
2. **Sequential activities** must follow one after another; concurrent activities can occur simultaneously
3. **Critical activities** have zero slack and directly impact project completion dates
4. **Slack time** provides scheduling flexibility for non-critical activities
5. **Dependencies** define relationships between activities and constrain scheduling options
6. **Minimum completion time** is calculated by summing durations along the critical path

### Preparation for Next Week

Week 12 will focus on Gantt chart practice, including:

- Creating Gantt charts using project management software
- Slack time analysis techniques
- Resource levelling on Gantt charts
- Schedule compression methods (crashing and fast-tracking)
- Handling delays and adjustments in complex projects

Learners should review this week's content and ensure understanding of basic concepts before progressing to practical application.

### Real-World Application

Major UK engineering organisations including Arup, Balfour Beatty, and BAE Systems all require engineers to demonstrate competency in Gantt chart interpretation as part of project management roles. This fundamental skill opens pathways to project leadership positions across the engineering sector.

---

## References

Association for Project Management (2019) *APM Body of Knowledge*. 7th edn. High Wycombe: Association for Project Management.

Brady, T. and Davies, A. (2010) 'Learning to deliver a mega-project: the case of Heathrow Terminal 5', *Praxis*, 6(1), pp. 5-12.

Burke, R. (2013) *Project Management: Planning and Control Techniques*. 5th edn. Chichester: John Wiley & Sons.

Crossrail (2017) *Crossrail Rolling Stock Programme Review*. London: Crossrail Limited.

Lock, D. (2020) *The Essentials of Project Management*. 5th edn. Abingdon: Routledge.

National Audit Office (2018) *Lessons Learned from Major UK Infrastructure Projects*. London: National Audit Office.

Project Management Institute (2017) *A Guide to the Project Management Body of Knowledge (PMBOK Guide)*. 6th edn. Newtown Square, PA: Project Management Institute.

Thames Water (2019) *Thames Tideway Tunnel: Project Delivery Update*. London: Thames Water Utilities Limited.

Wilson, J.M. (2003) 'Gantt charts: a centenary appreciation', *European Journal of Operational Research*, 149(2), pp. 430-437.

---

## Glossary

**Activity**: A discrete task or work element within a project that has a defined start and finish point.

**Concurrent activities**: Activities that can be performed simultaneously without dependency constraints.

**Critical activity**: An activity on the critical path with zero slack time; any delay directly impacts project completion.

**Critical path**: The longest sequence of dependent activities from project start to finish, determining minimum project duration.

**Dependency**: A relationship between activities where one activity cannot start or finish until another activity reaches a specific point.

**Duration**: The time required to complete an activity, typically measured in hours, days, weeks, or months.

**Earliest Finish Time (EFT)**: The earliest time an activity can be completed, based on predecessor activities.

**Float**: See Slack time.

**Gantt chart**: A horizontal bar chart representing a project schedule, showing activities plotted against a timeline.

**Latest Finish Time (LFT)**: The latest time an activity can finish without delaying the project completion date.

**Milestone**: A significant point or event in a project, typically marking the completion of a major deliverable or phase.

**Minimum completion time**: The shortest possible project duration, determined by the critical path.

**Predecessor**: An activity that must be completed (or reach a milestone) before another activity can begin.

**Sequential activities**: Activities that must occur in a specific order, with dependencies between them.

**Slack time**: The amount of time an activity can be delayed without affecting the project completion date; also called float.

**Successor**: An activity that follows another activity, dependent on its predecessor's completion or milestone achievement.


---

**Word Count**: 4,287 words (excluding references, glossary, and teaching notes)
