# Project Capture Document for Audit: _Still Can See After End Date_ 
#### *Author: Kaylee Hartzog*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 10, 13:52*
## Background
After a course ends, students want to be able to still access the course even when they are not taking it anymore. Not being able to go back to that course would mean that the student would not be able to look back and see what they did and learned in the course. This audit will make it so that a course will remain visable to a student after the course ends.

-----
## Definition of Done
We will create an audit that checks that every course is visible to students afte the course's end date.

-----
# Requirements
### General Requirements
- **Pass:** If the student is able to see the course after the end date.
- **Fail:** If the student is unable to see the course after the end date.
- **Warn:** If a student did not finish the course (droped the course), do not let them see the course after the end date(?).

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
### Questions/Concerns
- If a student doesn't compleate a course, does that mean they are not allowed to see the course after the course ends?
---
### User Interface
An extension of the base Audit class from `namespace Byui.CourseAudits.Business.Model.Audits`.
#### Type:
Audit Project class
-----
## Expectations
### Timeline
**Deadline:** 2019 Sep 1

**Priority:** Low

-----
#### *Approved By:* 
#### *Approval Date:*
