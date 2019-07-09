# Project Capture Document for Audit: Only One Person With Teacher Role
#### *Author: Jake Schwantes*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 4:46*
## Background
Some classes after their conversion could have a problem with not having any teachers enrolled or having multiple teachers enrolled. This could be a problem because most courses should have only one teacher and having two or none could be harmful to the class. We want to avoid this issue. This audit will get the api call for all given course codes and will ensure that only one teacher exists.

-----
## Definition of Done
We are creating this audit so we can check whether teachers are enrolled in given courses. We will be making the API call to get all the teachers in the given course. If there are teachers, we will make sure there is only one. If there are none or there are more than one, this audit will fail. We will also be seeing to make sure that there are students, and we will warn if there is a teacher but no students.

-----

# Requirements
### General Requirements
<!-- What counts as pass/fail/warn? -->
Pass: If there is only one user with teacher role.

Warning: If there is only one teacher but no students it will warn.

Fail: If there are no teachers or there are multiple teachers. The message will populate with how many teachers there were. And with the expected teacher, if that information is available.

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
The priority is high?
#### *Approved By:* 
#### *Approval Date:*
