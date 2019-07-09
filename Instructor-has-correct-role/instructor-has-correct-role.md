# Project Capture Document for Audit: _Instructor-has-correct-role_ 
#### *Author: Matt Wyndham*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 15:55*
## Background
Sometimes when course setup is done an instructor will accidentally be enrolled as something else in their course. This prevents them from fulfilling their duties and provides a poor experience for students.

-----
## Definition of Done
We will create an audit that checks every completed course after setup to see if the instructor for the course is properly enrolled as an instructor.

-----
# Requirements
### General Requirements
- **Pass:** If the sis instructor is enrolled in the course as an Instructor.
- **Fail:** If the sis instructor is not enrolled, or enrolled as a student or TA.
- **Warn:** If the sis instructor is enrolled as an alternate type of Instructor.
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

**Dealine:** 2019 Sep 1

**Priority:** High

-----
#### *Approved By:* 
#### *Approval Date:*