# Project Capture Document for Audit: New Gradebook
#### *Author: John Reiley*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 15:55*

## Background

Courses need to have "new gradebook" enabled.  Without it turned on, certain features, like late-policy, are not enabled.

-----

## Definition of Done

We are creating an audit that will check if a canvas course has the "new gradebook" feature enabled.

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->
The audit will pass when: "new gradebook" is enabled.  
The audit will fail when: "new gradebook" is disabled.  
The audit will warn when: ...?
### Input Requirements
#### Source of Inputs
All inputs will be received via the encompassing Audit Project.

#### Definition of Inputs
<!-- TBD: do not fill out just yet -->
- Course Id(s) to run this audit on.
---

### Output Requirements
#### Destination
Returned to the invoked method from the Audit Project.

#### Definition of Outputs
<!-- TBD: do not fill out just yet -->
- Results of the Pass/Fail/Warn status of this audit and associated messages.
---

### User Interface
An extension of the base Audit class from `namespace Byui.CourseAudits.Business.Model.Audits`.
#### Type:
Audit Project class

-----

## Expectations
### Timeline
Deadline: September 1, 2019  
Priority: 
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

-----

#### *Approved By: Jake Schwantes* 
#### *Approval Date: 19 July 2019*
