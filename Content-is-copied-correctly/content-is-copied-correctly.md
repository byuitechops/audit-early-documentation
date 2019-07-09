# Project Capture Document for Audit: _Content-is-copied-correctly_ 
#### *Author: Matt Wyndham*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 15:55*
## Background
Sometimes when course setup is done the course content does not copy, copies incompletely, or misses an item or two. This prevents students from completing assignments.

-----
## Definition of Done
We will create an audit that checks every completed course after setup to see if the content matches the reference course's content.

-----
# Requirements
### General Requirements
- **Pass:** If the course content matches the reference course content.
- **Fail:** If the course content differs from the reference course content in any way.
- **Warn:** If the reference course has no content.
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