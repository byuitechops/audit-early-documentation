# Project Capture Document for Audit: AssignmentAssociations 
#### *Author:* Lucas Wargha (updated by John Reiley)
#### *Stakeholder(s): Dan Gordon*
#### *Date: 2019 July 15*

## Background

Incorrectly copied assignment associations can result in a mess if not caught early enough, creating confusion for group assignments. 

-----

## Definition of Done

   The audit will test if there is correct association between the course's group categories and assignments by comparing the BP (blueprint) against the CC (copied course).

-----

# Requirements

### General Requirements
**Pass:** 
- Both BP and CC have null values for the `group_category_id` member of the **`assignment`** object.  
- Both BP and CC have values for the `group_category_id` AND same values for `name`, `role`, `self_signup`, `auto_leader`, and `group_limit` members of the **`group_category`** object.  

**Fail:**
- Only BP or CC have a null value for the `group_category_id` OR unmatching values for `name`, `role`, `self_signup`, `auto_leader`, and `group_limit` members of the **`group_category`** object.  

**Warn:** N/A ?

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

  Are we testing the assignment against the course blueprint? Which elements of each assignment's configuration should be checked? (Ex: time limit, availability, etc).
-----

## Expectations
### Timeline
<!-- What is the deadline? 2019 Sep 1? -->
<!-- What priority is this audit? -->

    Currently the plan is to finish this audit by September 1st 2019
-----

#### *Approved By:* 
#### *Approval Date:*
