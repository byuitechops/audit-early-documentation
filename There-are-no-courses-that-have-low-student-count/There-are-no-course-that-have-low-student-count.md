# Project Capture Document for Audit: _There-are-no-courses-that-have-low-student-count_ 
#### *Author: Matt Wyndham*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 15:55*
## Background
Sometimes after enrollments have happened a course is left incomplete. This means students who should be registered in a course will not be able to see it.

-----
## Definition of Done
We will create an audit that checks every completed course after enrollments to see if there are more than 10 students (or that there is the exact correct number of students if we have that information)

-----
# Requirements
### General Requirements
- **Pass:** If the course has 10 or more students (or has the exact number of students expected)
- **Fail:** If the course has less than 10 students (or has anything other than the exact number of students expected)
- **Warn:** If the number of teachers is greater than 1.
- **Warn:** If there are no teachers.
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

**Priority:** Low

-----
#### *Approved By:* 
#### *Approval Date:*