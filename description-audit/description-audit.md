# Project Capture Document for Audit: _Description_ 
#### *Author: Kaylee Hartzog*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 10, 12:52*
## Background
Many of the courses have a short course description in order to help students understand a bit more about the course. The description is optional for a course to have. This audit will check to see if a course has a description, and if it does, it will return it.

-----
## Definition of Done
This audit will check the courses to see if they contain a course description, and if they do, it will return the description.

-----
# Requirements
### General Requirements
- **Pass:** Audit returns a course description.
- **Fail:** Audit does not return a course description (because there is none).
- **Warn:** Description may not be formatted correctly.
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

**Priority:** Low
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->
-----
#### *Approved By:* 
#### *Approval Date:*
