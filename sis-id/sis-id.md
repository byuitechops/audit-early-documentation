# Project Capture Document for Audit: _SIS ID_ 
#### *Author:* Evgeniy Bekker
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 17:35*

## Background

    This "SIS ID" audit is part of a big audit project that BYUI IT department is working on.
    The purpose of the SIS ID audit is to test whether a given course has a correct SIS ID set. 
    
-----

## Definition of Done

    The audit needs to be able to successfully test whether a given course has a correct SIS ID set.

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->

    Pass: The "sis_course_id" key of the course is set properly.

    Fail: The "sis_course_id" key of the course isn't set or is not set to what we expect.

    Warn: It's set and is partially correct.

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

    I'm not sure if I have the right idea about what this audit is supposed to check.
        
-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By:* 
#### *Approval Date:*
