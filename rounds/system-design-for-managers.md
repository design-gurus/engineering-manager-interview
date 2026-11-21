# System Design for Engineering Managers

The system design round asks a manager to design a large system in 45 to 60 minutes, as it does for an engineer. The question is usually the same, but the grading is different. An engineer is graded mainly on the design itself. A manager is graded on technical judgment: which trade-offs were chosen, which risks were named, and how the work would be delivered by a team.

## What changes for a manager

| Area | Engineer candidate | Manager candidate |
|---|---|---|
| Component detail | Expected to go deep on two or three components | Expected to go deep on one, and to know where the others become hard |
| Trade-offs | States them | States them, and ties each to a business or team cost |
| Delivery | Rarely asked | Often asked: phases, team split, first milestone |
| Operations | Mentions monitoring | Explains who is on call and what would page them |
| Unknowns | Makes an assumption | Says who would be asked and how the answer changes the plan |

On call means being the person responsible for responding to production alerts during a set period.

## A 45-minute plan

| Minutes | Step | Output |
|---|---|---|
| 0 to 5 | Requirements | Three functional requirements and two measurable targets, such as latency and availability |
| 5 to 10 | Estimation | Requests per second, storage per year, read and write ratio |
| 10 to 25 | High-level design | Six to ten components, the data model, the main request path |
| 25 to 35 | One deep dive | The hardest component, with two options compared |
| 35 to 42 | Delivery plan | Three phases, team split, the main risk |
| 42 to 45 | Summary | The two trade-offs you would revisit |

The delivery plan is the step that most manager candidates skip, and it is the step that distinguishes them.

## Example: the delivery step for a notification service

Suppose the design must deliver 50 million notifications a day through push, email, and text message.

- **Phase 1, six weeks:** one channel (push), one queue, no user preferences. Two engineers. Goal: 5 million a day with a 99.9 percent delivery rate.
- **Phase 2, six weeks:** email and text message, user preferences, rate limits per user. Four engineers in two pairs.
- **Phase 3, four weeks:** retries with priority levels, and a dashboard for the support team.
- **Main risk:** the text message vendor limits throughput. Mitigation: a second vendor is contracted in phase 2.

Four sentences of this kind take two minutes and show that the candidate thinks about sequencing, staffing, and risk.

## Questions that are asked only of managers

- "How many engineers would this need, and how would you split them?"
- "What would you build first, and what would you postpone?"
- "Which part would you give to your most senior engineer?"
- "How would you know in week four that the project is late?"
- "Which decision here would you escalate, and to whom?"

## Common mistakes

- Staying at the level of boxes and arrows, so that the engineers on the panel doubt the candidate's depth.
- Going so deep on one component that there is no time for delivery.
- Saying "my team would decide that" for every technical question.
- Skipping estimation, which removes the basis for every later trade-off.

## Go deeper

- [Grokking the System Design Interview](https://www.designgurus.io/course/grokking-the-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=engineering-manager-interview&utm_content=rounds-system-design-for-managers) teaches the design questions that manager loops reuse, with full worked solutions.
- [Grokking the Engineering Manager Interview](https://www.designgurus.io/course/grokking-the-engineering-manager-interview?utm_source=github&utm_medium=repo&utm_campaign=engineering-manager-interview&utm_content=rounds-system-design-for-managers) covers the technical and project management skills the round expects from a manager.
- The free [grokking-system-design](https://github.com/design-gurus/grokking-system-design) repository has pattern pages and question outlines for practice.
- Free answer: [The system design interview for engineering managers](https://www.designgurus.io/answers/detail/what-is-the-system-design-interview-for-engineering-managers?utm_source=github&utm_medium=repo&utm_campaign=engineering-manager-interview&utm_content=rounds-system-design-for-managers)
