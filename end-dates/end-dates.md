# Project Capture Document for Audit: End Dates
#### *Author: Jake Schwantes*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 3:21*
## Background
-----
Some classes after their conversion could have a problem with not having the right end date. (e.g. A fall course should have its end date be in December. If it were in July, which is a spring end date, it would be incorrect and would need to be changed). This could be a problem because not having the right end dates could be a big issue for students. This is a high priority audit. This audit will make an api call to get all of the end dates, and make sure that they are correct.

## Definition of Done
-----
We are creating this audit so we can check whether the end dates for courses are set up correctly. We will be making the API call to get all the end dates for the course. If the end dates match the times set by BYU-I, The audit will pass. If they do not match, this audit will fail.
# Requirements
### General Requirements
- **Pass:** If the end dates are the correct date for the course.
- **Fail:** If the end dates are incorrect (e.g. July date when it needs to be a December date).

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

#### *Approved By:* 
#### *Approval Date:*
