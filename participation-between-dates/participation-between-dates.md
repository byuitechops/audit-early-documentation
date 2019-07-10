# Project Capture Document for Audit: _Participation Between Dates_ 
#### *Author:* Evgeniy Bekker
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 17:55*

## Background

    This "Participation Between Dates" audit is part of a big audit project that BYUI IT department is working on.
    The purpose of the Participation Between Dates audit is to test whether a given course has all of its enrolled students participate in between the dates that the course is offered.
    
-----

## Definition of Done

    The audit needs to be able to successfully test whether a given course is has all of its participation being in between the dates that the course is offered in.

-----

# Requirements

### General Requirements
<!-- What counts as pass/fail/warn? -->

    Pass: All of the course's participation occured in between the dates that the course was offered in.

    Fail: There was at least one participation outside of the range of dates in which the course was offered.

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

    I'm not sure if I have the right understanding of this audits purpose.
    What constitutes participation? (Maybe submitting any assignments/files? posting/responding in discussion boards?)
-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By:* 
#### *Approval Date:*
