# Project Capture Document for Audit: _Availability After Start Date_ 
#### *Author: Kaylee Hartzog*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 17:54*
## Background
Sometimes, after a semester begins, students are not able to view a course because it has not been made available to them, even if they are enrolled in the course. This audit will check to see if the courses no longer restrict students from viewing them after the start date has passed.

-----
## Definition of Done
We will create an audit that checks the course to see if the students are no longer restricted from viewing the course after the course start date has passed.

-----
# Requirements
### General Requirements
- **Pass:** Students are able to access the course after the start date
- **Fail:** Students cannot access the course after the start date
 
<!-- What counts as pass/fail/warn? -->
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
**Deadline:** 2019 Sep 1

**Priority:** High

-----
#### *Approved By:* Aaron Shiffler
#### *Approval Date:* 16 July 2019