# Project Capture Document for Audit: _Instructor-has-correct-role_ 
#### *Author: Jake Schwantes*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 22, 9:09*
## Background
Sometimes when course setup is done students will accidentally be enrolled as something else in their course, or not enrolled in their course entirely. This could be an issue if students have more permissions than they should.

-----
## Definition of Done
We will create an audit that checks every completed course after setup to see if the students enrolled in a given course, and if the students for the course is properly enrolled as students.

-----
# Requirements
### General Requirements
- **Pass:** If the students are enrolled in the course as an students.
- **Fail:** If a student is not enrolled.
- **Fail:** If all students are enrolled with the correct roles.

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
