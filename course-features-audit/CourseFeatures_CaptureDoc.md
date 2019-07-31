# Project Capture Document for Audit: New Gradebook
#### *Author: John Reiley*
#### *Stakeholder(s): Dan Gordon*
#### *Start Date: 2019 July 8, 15:55*
#### *Modified: 2019 July 31, 11:00*

## Background

This audit combined two sub-aduits: new_gradebook and late_policy_is_copied_correctly.

Courses need to have "new gradebook" enabled.  Without it turned on, certain features, like late-policy, are not enabled.
Sometimes late policies may not be copied correctly at the start of a semester, allowing students to submit late homework.

-----

## Definition of Done

We are creating an audit that will check if a canvas course has the "new gradebook" feature enabled and make sure the late policy is copied and copied correctly from the course blueprint.

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->
#### New Gradebook Audit
The audit will pass when: 
- "new gradebook" is enabled.

The audit will fail when:
- "new gradebook" is disabled.
#### Late Policy is Copied Correctly Audit
The audit will pass when: 
- The late policy matches the semester blueprint  

The audit will fail when: 
- The late policy does not match the semester blueprint    
- New grade book is not on  
- There is no late policy  

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
