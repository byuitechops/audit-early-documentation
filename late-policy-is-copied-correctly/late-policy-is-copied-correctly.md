# Project Capture Document for Audit: Late Policy Is Copied Correctly
#### *Author: John Reiley*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 15:55*

## Background

Sometimes late policies may not be copied correctly at the start of a semester, allowing students to submit late homework.

-----

## Definition of Done

We are creating an audit that will check to make sure the late policy is copied and copied correctly from the course blueprint.

-----

# Requirements

### General Requirements
The audit will pass when: The late policy matches the semester blueprint

The audit will fail when: The late policy does not match the semester blueprint 
 
The audit will warn when: "Auto apply" is enabled but there is no point deduction for late or unsubmitted work

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
#### *Approval Date: 23 July 2019*
