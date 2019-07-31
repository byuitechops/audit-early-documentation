# Project Capture Document for Audit: _Format Should Be Online_ 
#### *Author:* Evgeniy Bekker & Seth Bolander
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 17:35*

## Background

This "Format should be online" audit is part of a big audit project that BYUI IT department is working on. The purpose of the Format should be online audit is to test whether a given course has the correct format. This format is to differentiate between Online, Campus, and Hybrid Canvas courses.
    
-----

## Definition of Done

The audit needs to be able to successfully test whether a given course has the `course_format` key set the same as CX. This key can be found on course object by making an API call to `/api/v1/courses/{courseCode}`.

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->
#### Pass
The `course_format` key of the course is set to the same as CX. `Online` for Online courses, `Campus` for Campus courses, and `Hybrid` for Hybrid courses.

#### Fail
The `course_format` key of the course is `Not Set` or is not correct.

#### Warn
None?

-----

## Questions/Concerns

-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By: Jake Schwantes* 
#### *Approval Date: 31 July 2019*
