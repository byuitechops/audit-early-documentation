# Project Capture Document for Audit: _Participation Between Dates_ 
#### *Author: Evgeniy Bekker & Seth Bolander*
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 17:55*

## Background

This "Participation Between Dates" audit is part of a big audit project that BYU-I IT department is working on.
The purpose of the Participation Between Dates audit is to test whether a given course has restricted enrollments to course dates; meaning students cannot participate or be enrolled to the course until the start date.
    
-----
## Definition of Done

The audit needs to be able to successfully test whether a given course restricts enrollments and participation to course dates. An API call to the course (`/api/v1/courses/{courseCode}`) gives you this information on the `restrict_enrollments_to_course_dates` key, which should be `true`.

-----
## Requirements

#### Pass:
Course object has `restrict_enrollments_to_course_dates` set to `true` or `1`.

#### Fail:
Course object has `restrict_enrollments_to_course_dates` set to `false` or `0`.

#### Warn:
Not sure yet

-----
## Questions/Concerns

- Are there any courses that should have this set to false? I am thinking no because the Majors courses and other courses that are available year round do not have a term or start/end date set. This restriction only effects courses that have a start and end date or a term; so it shouldn't matter whether or not this key is true or not, right?

-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By: Jake Schwantes* 
#### *Approval Date: 30 July 2019*
