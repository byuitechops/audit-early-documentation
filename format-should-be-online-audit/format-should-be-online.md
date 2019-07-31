# Project Capture Document for Audit: _Format Should Be Online_ 
#### *Author:* Evgeniy Bekker
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 17:35*

## Background

This "Format should be online" audit is part of a big audit project that BYUI IT department is working on.
The purpose of the Format should be online audit is to test whether a given course has the correct format based on its subaccount. 
    
-----

## Definition of Done

The audit needs to be able to successfully test whether a given course is set to be "online."

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->

**Pass**: The "course_format" key of the course is set to "online" for sub-account "BYUI Scaled" and "campus" for anything else.
**Fail**: The "course_format" key of the course is not set or is not correct.
**Warn**: None?

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

-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By:* 
#### *Approval Date:*
