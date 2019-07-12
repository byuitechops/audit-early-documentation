# Project Capture Document for Audit: _Start Date_ 
#### *Author:* Evgeniy Bekker
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 8, 16:55*

## Background

    This "Start Date" audit is part of a big audit project that BYUI IT department is working on.
    The purpose of the Start Date audit is to test whether the start date of a given course is correct, 
    meaning that it is in the correct format, is set correctly for the semester the course is offered in, etc. 
    
-----

## Definition of Done

    The audit needs to be able to successfully test the start date for any give course.

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->

    Pass: The start date is set in the correct format and it is set correctly according to the expected semester.

    Fail: The start date is not in the correct format, isn't set at all, or isn't the date we expect.

    Warn: Some of the parts of the date are set correctly but at least one of them isn't.

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
    What should I put in the warn section.

    Some additional info:
        The API call will be to https://byui.instructure.com//api/v1/courses/course_id
        which will return a course JSON string(which we can turn into a course object) and 
        then use the "start_at" to test it. 

        as said above, I'm not sure against what data do I need to test that key. 
        I believe Aaron is going to talk with Dan Gordon about that(or maybe he already knows).
-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By:* 
#### *Approval Date:*
