---
name: 🐛 Eove bug issue 🐛
about: Report a reproducible bug or regression
title: "[Bug]: "
labels: ""
assignees: ""
---

#### Origin

- [ ] Technician
- [ ] Physician
- [ ] Marketing
- [ ] RD
- [ ] After Sales Service

#### Context

_[Indicate version(s) where the bug has been found]_

#### Criticality questions

Tick the box(es) only if the answer is YES.

- [ ] Can the patient suffer damage due to defective ventilation? **(ventilation)**
- [ ] Does this cause misinterpretation of the ventilation data? **(settings/monitoring)**
- [ ] Does this cause a lack of prevention to the patient's entourage? **(alarms)**
- [ ] Does this cause a malfunction of the product or one of its assemblies? **(hardware)**

#### Labelling

```mermaid
graph TD
    D{Is it dangerous for the patient? (On of the 4 questions is checked)}
    D --> |NO| E[<b>LABEL BUG]
    D --> |YES| G(Risk analysis)
    G --> H{Is the remaining<br />risk acceptable?}
    H --> |YES|I[<b>LABEL CRITICAL]
    H --> |NO| J[<b>LABEL NC]
style E fill:#FF0,stroke:#333,color:#000, stroke-width:4px
style I fill:#FFC300,stroke:#333,color:#000, stroke-width:4px
style J fill:#FF0000,stroke:#333,color:#000, stroke-width:4px
```

_(Complete labelling regarding the workflow result and erase this chapter once labelling done)_

## Description

#### What is the problem to solve?

_(Describe as best as you can the bug or regression to be fixed)_

#### Proposal

_(Complete with your idea, the feedback from the field, ask for help, etc...)_

#### Test

_(Complete with as much use cases as possible to describe exactly the expected behavior. Use 'Given When Then' format to allow the export of the test directly to the official documentation)_
