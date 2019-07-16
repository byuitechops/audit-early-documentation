# Project Capture Document for Audit: Only One Person With Teacher Role
#### *Author: Jake Schwantes*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 4:46*
## Background

Classes could have a problem with not having any teachers enrolled or having multiple teachers enrolled. We want to avoid this issue, especially because having the teacher role assigned correctly is high priority before the semesters start. This audit will get a list of teachers for the given course codes and will ensure that only one teacher role exists. (This is not the same audit as making sure the teachers have the correct enrollments).

-----
## Definition of Done
We are creating this audit so we can check whether the correct number of teachers are enrolled in given courses (one teacher only). We will be making the `/api/v1/courses/:course_id/users?enrollment_type[]=teacher` call to get all the users with the teacher role in the given course. If there are teachers, we will make sure there is only one. If there are none or there are more than one, this audit will fail.

-----

# Requirements
### General Requirements
<!-- What counts as pass/fail/warn? -->
- Pass: If there is only one user with teacher role.

- Fail: If there are no teachers

- Fail: If there are multiple teachers

The message will populate with how many teachers there were.

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
The priority is high
#### *Approved By:* Aaron Shiffler
#### *Approval Date:* 16 July 2019
