# Project Capture Document for Audit: Hidden courses have correct status- maybe don't make till have real instructor
#### *Author: Cameron Thompson*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 15:55*
## Background

Some courses durring copy could run into an issue where the hidden courses that should be hidden are no longer hidden and courses that shouldn't be hidden are now hidden. 

-----
## Definition of Done
This audit will check that a course has the right status based on if it is supposed to be hidden or not. 

-----
# Requirements
### General Requirements
<!-- What counts as pass/fail/warn? -->
A course will pass when: *A course that is supposed to be hidden is hidden*

A course will fail when: *A course that is supposed to be hidden is not hidden or a course that is not supposed to be hidden is hidden*

A course will warn when:
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
<!-- What is the deadline? 2019 Sep 1? -->
2019 Sep 1
<!-- What priority is this audit? -->
Low
-----
#### *Approved By:* 
#### *Approval Date:*
