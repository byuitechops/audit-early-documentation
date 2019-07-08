# Project Capture Document for Audit: _Start Date_ 
#### *Author: * Evgeniy Bekker
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 16:55*

## Background

    This "Start Date" audit is part of a big audit project that BYUI IT department is working on.
    The purpose of the Start Date audit is to test whether the start date of a given course is correct, meaning that it is in the correct format, is set correctly for the semester the course is offered in, etc. 
    
-----

## Definition of Done

    The audit needs to be able to successfully test the start date for any give course.

-----

# Requirements

### General Requirements
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

## Questions/Concerns

    Against what are we testing the start date? We probably don't to hard code any dates. 
    Every course has a start date in this format: "start_at": "2019-01-11T21:55:24Z".
    There is also a property "enrollment_term_id": 10. What does this number represent?
-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

-----

#### *Approved By:* 
#### *Approval Date:*
