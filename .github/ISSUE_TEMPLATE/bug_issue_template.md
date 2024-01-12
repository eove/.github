---
name: 🐛 Eove bug issue 🐛
about: Report a reproducible bug or regression
title: "[Bug]: "
labels: ""
assignees: ""
---

#### Origin
  
- Technician
- Physician
- Marketing
- RD
- After Sales Service

_keep only the necessary lines_

#### Criticality questions

~Strike~ the wrong answer

- Can the patient suffer damage due to defective ventilation? **(ventilation)** YES/NO
- Does this cause misinterpretation of the ventilation data? **(settings/monitoring)** YES/NO
- Does this cause a lack of prevention to the patient's entourage? **(alarms)** YES/NO
- Does this cause a malfunction of the product or one of its assemblies? **(hardware)** YES/NO

#### Labelling

```mermaid
graph TD
    D{"Is it dangerous for the patient?<br/>(the answer is YES to one of the 4 questions)"}
    D --NO--> E[LABEL BUG]
    D --YES--> G(Risk analysis)
    --> H{Is the remaining<br/>risk acceptable?}
    H --YES--> I[LABEL CRITICAL]
    H --NO--> J[LABEL NC]

classDef Tag stroke:#333,color:#000, stroke-width:4px, font-weight: bold
class E,I,J Tag;
style E fill:#FFFF00
style I fill:#FFC300
style J fill:#FF0000
```

_Complete labelling regarding the [workflow result](https://github.com/eove/.github/) (visualise it in preview) and erase this chapter once labelling done_

## Description

#### What is the problem to solve?

```
Given
When
Then
```

#### Proposal _optionnal_

_Complete with your idea, the feedback from the field, ask for help, etc..._
