---
name: 🐛 Eove bug issue 🐛
about: Report a bug/regression concerning end-user
title: "[Bug]: "
labels: ""
assignees: ""
---

## Origin
  
- Technician
- Physician
- Marketing
- RD
- After Sales Service
- Manufacturing
- QA

_keep only the necessary lines_

## Criticality questions

~Strike~ the wrong answer

- Can the patient suffer damage due to defective ventilation? **(ventilation)** YES/NO
- Does this cause misinterpretation of the ventilation data? **(settings/monitoring)** YES/NO
- Does this cause a lack of prevention to the patient's entourage? **(alarms)** YES/NO
- Does this cause a malfunction of the product or one of its assemblies? **(hardware)** YES/NO

### Labelling

```mermaid
graph TD
    DANGER_QUESTION{"Is it dangerous for the patient?<br/>(One of the 4 questions is checked)"}
    DANGER_QUESTION --NO--> MINOR_BUG[bug:minor]
    DANGER_QUESTION --YES--> RISK(Risk analysis)
    RISK --> RISK_QUESTION{Is the remaining<br/>risk acceptable?}
    RISK_QUESTION --YES--> CRITICAL_BUG[bug:critical]
    RISK_QUESTION --NO--> NON_CONFORM_BUG[bug:nc]

classDef Tag stroke:#333,color:#000, stroke-width:4px, font-weight: bold
class MINOR_BUG,CRITICAL_BUG,NON_CONFORM_BUG,FEATURE Tag;
style MINOR_BUG fill:#FFFF00
style CRITICAL_BUG fill:#FFC300
style NON_CONFORM_BUG fill:#FF0000
```

_Complete labelling regarding the [workflow result](https://github.com/eove/.github/) (visualise it in preview) and erase this chapter once labelling done_

## Description

### What is the problem to solve?

```
  Feature: ...
    Scenario: ...
      Given ...
      When ...
      Then ... ....... PASS [ ] / FAIL [ ]
```

## Proposal _optionnal_

_Complete with your idea, the feedback from the field, ask for help, etc..._
