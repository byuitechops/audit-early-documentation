# Project Capture Document for Audit: Groups 
#### *Author:* Lucas Wargha
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 9, 09:30*

## Background

    The "Groups" audit is part of a big audit project that BYUI IT department is working on. 
    The purpose for this audit is to test that groups were set up correctly during each semester. Meaning that groups with their names and all pertaining information were allocated accuratedely to assignments.

-----

## Definition of Done

   This audit is able to test that groups were correctly set up or transferred from semester to semester in a given course/array of courses. 

-----

# Requirements

### General Requirements
- **Pass:** If groups match blueprint.
- **Fail:** If groups do not match blueprint.
- **Warn:** N/A ?
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

    Against what are we testing the groups? What properties should we be checking when checking groups and what defines a warn/pass/error in this audit? 
    -Properties that would be evalulated in this audit.
    1)name
    2)max_membership
    3)join_level
    4)is_public
    5)description
    6)member_count
    7)context type ?
    8)leader == NULL
    9)concluded == false
-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By:* 
#### *Approval Date:*
