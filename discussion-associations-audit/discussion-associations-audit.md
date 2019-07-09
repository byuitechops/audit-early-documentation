# Project Capture Document for Audit:Discussion_Associations_Audit 
#### *Author:* Lucas Wargha
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 10:03*

## Background

    The "Discussion Associations" audit is part of a big audit project that BYUI IT department is working on. 
    The purpose of this audit is to assure that all discussions were set up properly in a given course/set of courses. The test should also involve the accuracy of configurations agains the blueprint of a given course. (Ex: Allow threads, etc) 

-----

## Definition of Done

   This test has the objective of testing discussion boards throughout canvas courses. This test should go over different configurations for each discussion board. 

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

  Are we testing the discussion boards against the course blueprint? Which elements of each discussion's configuration should be checked? (Ex: threaded discussion, visualization pre/post initial reply, etc).
-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By:* 
#### *Approval Date:*
