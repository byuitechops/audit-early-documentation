# Project Capture Document for Audit: _Participation Between Dates_ 
#### *Author: Evgeniy Bekker & Seth Bolander*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 17:55*

## Background

This "Participation Between Dates" audit is part of a big audit project that BYUI IT department is working on.
The purpose of the Participation Between Dates audit is to test whether a given course has restricted enrollments to course dates.
    
-----

## Definition of Done

The audit needs to be able to successfully test whether a given course restricts enrollments and participation to course dates.

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->

Pass: `restrict_enrollments_to_course_dates` is `true` or `1`.

Fail: `restrict_enrollments_to_course_dates` is `false` or `0`.

Warn: Not sure yet

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

## Questions/Concerns

Is the only key we should be looking at `restrict_enrollments_to_course_dates` or are there other keys that we need to test for participation?
-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By:* 
#### *Approval Date:*
