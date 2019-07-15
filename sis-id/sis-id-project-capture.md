# Project Capture Document for Audit: _SIS ID_ 
#### *Author:* Evgeniy Bekker
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 17:35*

## Background

    This "SIS ID" audit is part of a big audit project that BYUI IT department is working on.
    The purpose of the SIS ID audit is to test whether a given course has a correct SIS ID set. 
    
-----

## Definition of Done

    The audit needs to be able to successfully test whether a given course has a correct SIS ID set
    and that the SIS ID is in the correct format.

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->

    Pass: The "sis_course_id" key of the course is set properly and is in the correct format. 
    SIS ID has a specific format:
        "campus/online.YEAR.Semester.ClassCode.duration.instructor_email" 
        ex. "Campus.2019.Fall.FAML 120.Block1.denniss@byui.edu"

    Fail: The "sis_course_id" key of the course isn't set, isn't set to what we expect,
        or isn't in the correct format.

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

    Some additional info:
        The API call will be to https://byui.instructure.com//api/v1/courses/course_id
        which will return a course JSON string(which we can turn into a course object) and 
        then use the "sis_course_id" to test it. 

        I'm not sure against what data do I need to test that key. 
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
