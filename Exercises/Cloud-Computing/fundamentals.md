# Cloud computing fundamentals

Work in groups of 2–4. These exercises let you practice capacity planning, cloud architecture, shared responsibilities, and risk assessment.

Show your reasoning, state any assumptions, and use the concepts covered in the chapter.

## Exercise 1: Scale a Registration Platform

### Scenario

A university’s registration platform experiences the following demand during one 24-hour day. The three periods do not overlap.

| Period | Duration | Requests per minute |
| --- | ---: | ---: |
| Normal activity | 18 hours | 300 |
| Busy period | 4 hours | 900 |
| Registration peak | 2 hours | 1,800 |

Use these assumptions:

- Each application-server instance safely handles **300 requests per minute**.
- Each instance costs **€0.10 per running hour**.
- New instances take **five minutes** to become ready.
- Requests can be distributed evenly across instances, and the database has sufficient capacity.
- Ignore other costs and startup overlap for the cost calculations. Account for startup time when explaining your scaling plan.

### Tasks

1. Calculate the minimum number of instances needed in each period.
2. Calculate the daily cost of keeping enough instances for peak demand running for all 24 hours.
3. Calculate the daily cost of adjusting capacity exactly to each period’s demand. Calculate the savings in euros and as a percentage of the fixed-capacity cost.
4. Explain whether these adjustments represent horizontal or vertical scaling. Identify when scaling out and scaling in occur.
5. Propose a scaling plan that accounts for the five-minute startup delay. Explain how it uses a lead, lag, or match strategy. State whether you assume the busy periods are predictable.
6. Explain what changes if the platform must handle peak demand even after one instance fails. Calculate the required instance count before the failure and identify the mechanisms needed to keep serving requests.

### What to submit

- Capacity and cost calculations, with units clearly labeled.
- A short scaling plan explaining when capacity changes and why.
- Your proposed approach to handling one instance failure.



## Exercise 2: Design and Assess a University Cloud Solution

### Scenario

A university plans to modernize its learning platform. It has these requirements:

- Student records must remain in an approved location.
- Demand rises sharply during examinations.
- The IT team has limited staff.
- A single-server failure should not stop assignment submissions.
- The university must be able to export its data if it changes providers.

Treat the approved-location requirement as a given organizational constraint. You do not need to research legislation or select a real cloud provider. Label the approved location in your design and state any additional assumptions.

### Tasks

1. Draw a simple architecture showing users, the application, its database, backup or redundant resources, and network connections. Label the main data flows.
2. Explain how your solution handles increased demand during examinations and releases extra capacity afterward. Identify which resources change, whether scaling is horizontal or vertical, and which measurements could trigger adjustments.
3. Mark the university’s organizational boundary and where it relies on external services or operators. Explain what is trusted and for which purpose.
4. Assign responsibilities to the **provider, consumer, resource administrator, auditor, and carrier**. Identify who owns the learning service. One organization may perform more than one role.
5. Complete the risk table below with examples specific to your design. Name who implements each control; identify shared responsibilities where appropriate.
6. Describe what happens when the main application server fails: how the failure is detected, how requests are redirected, and how the replacement accesses current submission data.
7. Propose **two measurable service requirements**. For each, specify what is measured, its target, and how you would check it. Describe **one practical test of the university’s exit plan** that checks whether exported data can be used elsewhere.

### Risk assessment table

| Risk | Example in your design | Proposed control | Responsible party |
| --- | --- | --- | --- |
| Security or incorrect access | | | |
| Provider outage or reduced operational control | | | |
| Difficult migration to another provider | | | |
| Data stored or processed outside approved locations | | | |

### What to submit

- One labeled architecture diagram, drawn digitally or by hand.
- The completed risk assessment table.
- Brief notes covering scaling, role assignments, failure handling, measurable service requirements, and the exit-plan test.
- A three-minute presentation explaining your design and its main tradeoffs.

There is no single required architecture. Your choices should be consistent with the scenario and supported by clear reasoning.
