# Project Capture Document for Audit: Instructor Roles Are Correct
#### *Author: Jake Schwantes*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 4:46*
## Background

Some classes after their conversion could have a problem with not having instructor roles correct. This audit will ensure that instructors are enrolled with the right role. 

-----

## Definition of Done

We are creating this audit so we can check whether instructors have the right role in given courses. We will be making the API call to get the instructors and their roles, then making sure that the roles are correct. If there is an intructor with an incorrect role, it will fail.

-----

### General Requirements
<!-- What counts as pass/fail/warn? -->
Pass: Instructors have the the correct role

Warning:

Fail: If a instructor doesn't have the correct roll.
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
