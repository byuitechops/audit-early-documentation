# Project Capture Document for Audit: Hidden Courses Don't Have Enrollments
#### *Author: Jake Schwantes*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 4:46*

---

## Background
Some classes after their conversion could want to remain hidden. This means that the course is not public for academic learning, so there should be no enrollments in these courses. If there are, that could lead to problems and we would have to fix them. This audit will check for that and fail if there are enrollments in hidden courses.

-----

## Definition of Done

We are creating an audit that will pass only if hidden courses have no enrollments. We will do this by making the api call to get enrollments and determining whether a course is hidden, then making sure that there are no enrollments.
# Requirements
### General Requirements
<!-- What counts as pass/fail/warn? -->
Pass: If a course is hidden and has no enrollments.

Warning: If a course is not hidden and has no enrollments

Fail: If a hidden course has enrollments.
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
<!-- What priority is this audit? -->
-----
The deadline is Sep 1, 2019.
The priority is medium-low?
#### *Approved By:* 
#### *Approval Date:*
